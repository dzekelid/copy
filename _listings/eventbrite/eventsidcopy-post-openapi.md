---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Post Events Copy
  description: Creates a duplicate version of the event being copied. Returns the
    event object for the newly created event.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---