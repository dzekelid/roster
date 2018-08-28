---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Software Cloud API Get conversation roster
  description: Authentication required, with scope participate:conversation
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/{conversationId}/roster:
    get:
      summary: Get conversation roster
      description: Authentication required, with scope participate:conversation
      operationId: ConversationRosterGetHandler
      x-api-path-slug: sitecloudidconversationconversationidroster-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      responses:
        200:
          description: OK
      tags:
      - Conversation
      - Roster
    patch:
      summary: Update a conversation roster
      description: Authentication required, with scope manage:conversation
      operationId: PatchRosterHandler
      x-api-path-slug: sitecloudidconversationconversationidroster-patch
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      responses:
        200:
          description: OK
      tags:
      - Conversation
      - Roster
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