swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
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
  /courses/{course_id}/course_copy/id:
    get:
      summary: Get course copy status
      description: Get course copy status.
      operationId: get-course-copy-status
      x-api-path-slug: coursescourse-idcourse-copyid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Course
      - Copy
      - Id