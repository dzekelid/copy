---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Copy provisional grade
  description: Copy provisional grade.
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