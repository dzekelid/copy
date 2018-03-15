---
swagger: "2.0"
info:
  title: Microsoft Office 365
  description: Office 365 is the brand name used by Microsoft for a group of software
    plus services subscriptions that provides productivity software and related services
    to its subscribers.
  version: 1.0.0
host: outlook.office365.com
basePath: /ews/odata/Me
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Messages{message_id}/Copy:
    parameters:
      summary: Parameters Messages Message Copy
      description: Parameters messages message  copy
      operationId: parametersMessagesMessageCopy
      responses:
        200:
          description: OK
      tags:
      - messages
      - message
      - ""
      - copy
definitions:
  calendar:
    properties:
      '@odata.id':
        description: This is a default description.
        type: get
      '@odata.editLink':
        description: This is a default description.
        type: get
      Id:
        description: This is a default description.
        type: get
      Name:
        description: This is a default description.
        type: get
      ChangeKey:
        description: This is a default description.
        type: get
      Events@odata.navigationLink:
        description: This is a default description.
        type: get
  forwardEmail:
    properties:
      Comment:
        description: This is a default description.
        type: get
      ToRecipients:
        description: This is a default description.
        type: get
  copyFolder:
    properties:
      DestinationId:
        description: This is a default description.
        type: get
  getFolderById:
    properties:
      '@odata.id':
        description: This is a default description.
        type: get
      '@odata.editLink':
        description: This is a default description.
        type: get
      Id:
        description: This is a default description.
        type: get
      ParentFolderId:
        description: This is a default description.
        type: get
      DisplayName:
        description: This is a default description.
        type: get
      ClassName:
        description: This is a default description.
        type: get
      TotalCount:
        description: This is a default description.
        type: get
      ChildFolderCount:
        description: This is a default description.
        type: get
      UnreadItemCount:
        description: This is a default description.
        type: get
      ChildFolders@odata.navigationLink:
        description: This is a default description.
        type: get
  addCalendarGroup:
    properties:
      '@odata.type':
        description: This is a default description.
        type: get
      Name:
        description: This is a default description.
        type: get
  newEvent:
    properties:
      '@odata.type':
        description: This is a default description.
        type: get
      Subject:
        description: This is a default description.
        type: get
      Body:
        description: This is a default description.
        type: get
      Start:
        description: This is a default description.
        type: get
      End:
        description: This is a default description.
        type: get
      Location:
        description: This is a default description.
        type: get
      ShowAs:
        description: This is a default description.
        type: get
  updateEmail:
    properties:
      Body:
        description: This is a default description.
        type: get
  addNewMailFolderRequest:
    properties:
      '@odata.type':
        description: This is a default description.
        type: get
      DisplayName:
        description: This is a default description.
        type: get
  updateEvent:
    properties:
      Location:
        description: This is a default description.
        type: get
  replyComment:
    properties:
      Comment:
        description: This is a default description.
        type: get
  updateNewMailFolderRequest:
    properties:
      DisplayName:
        description: This is a default description.
        type: get
  newAttachment:
    properties:
      '@odata.type':
        description: This is a default description.
        type: get
      Name:
        description: This is a default description.
        type: get
      Item:
        description: This is a default description.
        type: get
  createContact:
    properties:
      '@odata.type':
        description: This is a default description.
        type: get
      GivenName:
        description: This is a default description.
        type: get
      Surname:
        description: This is a default description.
        type: get
      EmailAddress1:
        description: This is a default description.
        type: get
      BusinessPhone1:
        description: This is a default description.
        type: get
      Birthday:
        description: This is a default description.
        type: get
  newEmail:
    properties:
      '@odata.type':
        description: This is a default description.
        type: get
      Subject:
        description: This is a default description.
        type: get
      Importance:
        description: This is a default description.
        type: get
      Body:
        description: This is a default description.
        type: get
  updateContact:
    properties:
      MobilePhone1:
        description: This is a default description.
        type: get
  updateCalendar:
    properties:
      Name:
        description: This is a default description.
        type: get
  calendarRepresentation:
    properties:
      '@odata.id':
        description: This is a default description.
        type: get
      '@odata.editLink':
        description: This is a default description.
        type: get
      Id:
        description: This is a default description.
        type: get
      Name:
        description: This is a default description.
        type: get
      ChangeKey:
        description: This is a default description.
        type: get
      ClassId:
        description: This is a default description.
        type: get
      Calendars@odata.navigationLink:
        description: This is a default description.
        type: get
  contacts:
    properties:
      '@odata.id':
        description: This is a default description.
        type: get
      '@odata.editLink':
        description: This is a default description.
        type: get
      Id:
        description: This is a default description.
        type: get
      ParentFolderId:
        description: This is a default description.
        type: get
      DisplayName:
        description: This is a default description.
        type: get
      Contacts@odata.navigationLink:
        description: This is a default description.
        type: get
      ChildFolders@odata.navigationLink:
        description: This is a default description.
        type: get
x-collection-name: Microsoft Office 365
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