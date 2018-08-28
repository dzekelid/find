---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API Describe Findings
  version: 1.0.0
  description: Describes the findings that are specified by the ARNs of the findings.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddAttributesToFindings:
    get:
      summary: Add Attributes To Findings
      description: |-
        Assigns attributes (key and value pairs) to the findings that are specified by the
                 ARNs of the findings.
      operationId: addAttributesToFindings
      x-api-path-slug: actionaddattributestofindings-get
      parameters:
      - in: query
        name: attributes
        description: The array of attributes that you want to assign to specified
          findings
        type: string
      - in: query
        name: findingArns
        description: The ARNs that specify the findings that you want to assign attributes
          to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes To Findings
  /?Action=DescribeFindings:
    get:
      summary: Describe Findings
      description: Describes the findings that are specified by the ARNs of the findings.
      operationId: describeFindings
      x-api-path-slug: actiondescribefindings-get
      parameters:
      - in: query
        name: findingArns
        description: The ARN that specifies the finding that you want to describe
        type: string
      - in: query
        name: locale
        description: The locale into which you want to translate a finding description,
          recommendation,         and the short description that identifies the finding
        type: string
      responses:
        200:
          description: OK
      tags:
      - Findings
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