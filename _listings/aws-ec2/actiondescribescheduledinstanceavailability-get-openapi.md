---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Describe Scheduled Instance Availability
  version: 1.0.0
  description: Finds available schedules that meet the specified criteria.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeScheduledInstanceAvailability:
    get:
      summary: Describe Scheduled Instance Availability
      description: Finds available schedules that meet the specified criteria.
      operationId: describescheduledinstanceavailability
      x-api-path-slug: actiondescribescheduledinstanceavailability-get
      responses:
        200:
          description: OK
      tags:
      - Server Instance Availability
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