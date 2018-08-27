swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/{id}/copy/:
    post:
      summary: Post Events Copy
      description: Creates a duplicate version of the event being copied. Returns
        the event object for the newly created event.
      operationId: postEventsCopy
      x-api-path-slug: eventsidcopy-post
      parameters:
      - in: query
        name: end_date
        description: The end time of the new event
        type: query
      - in: query
        name: name
        description: The name of the new event
        type: query
      - in: query
        name: start_date
        description: The start time of the new event
        type: query
      - in: query
        name: timezone
        description: timezone for the new event (Olson format)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Copy
  /event_copy:
    get:
      summary: Get Event Copy
      description: This method duplicates an existing event, returning the ID of the
        new event.
      operationId: Get_event_copy_
      x-api-path-slug: event-copy-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: event_id
        description: The ID of the existing event
      - in: query
        name: event_name
        description: A new name for this copy of the Event
      responses:
        200:
          description: OK
      tags:
      - Event
      - Copy