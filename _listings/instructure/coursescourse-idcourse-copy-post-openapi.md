---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Copy course content
  description: Copy course content.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/assignments/assignment_id/provisional_grades/{provisional_grade_id}/copy_to_final_mark:
    post:
      summary: Copy provisional grade
      description: Copy provisional grade.
      operationId: copy-provisional-grade
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idcopy-to-final-mark-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Provisional
      - Grade
      - Id
      - Copy
      - To
      - Final
      - Mark
  /courses/{course_id}/course_copy:
    post:
      summary: Copy course content
      description: Copy course content.
      operationId: copy-course-content
      x-api-path-slug: coursescourse-idcourse-copy-post
      parameters:
      - in: query
        name: except[]
        description: A list of the course content types to exclude, all areas not
          listed will bencopied
      - in: query
        name: only[]
        description: A list of the course content types to copy, all areas not listed
          will notnbe copied
      - in: query
        name: source_course
        description: ID or SIS-ID of the course to copy the content from
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Course
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