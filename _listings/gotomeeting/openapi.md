swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: SCIM
  description: the-scim-api-lets-you-manage-users-in-your-organization--you-can-then-automate-the-provisioning-of-product-licenses-for-these-users-and-they-can-use-your-companys-single-signon-solution-through-an-identity-provider-
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: N/A
host: api.citrixonline.com
basePath: /identity/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizers/{organizerKey}/webinars/{webinarKey}/panelists:
    get:
      summary: Get webinar panelists
      description: Retrieves all the panelists for a specific webinar.
      operationId: getPanelists
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeypanelists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Panelists
    post:
      summary: Create Panelists
      description: Create panelists for a specified webinar
      operationId: createPanelists
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeypanelists-post
      parameters:
      - in: body
        name: body
        description: Array of panelists
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Panelists
  /organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}:
    delete:
      summary: Delete webinar panelist
      description: Removes a webinar panelist.
      operationId: deleteWebinarPanelist
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeypanelistspanelistkey-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Panelists
      - PanelistKey
  /organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}/resendInvitation:
    post:
      summary: Resend panelist invitation
      description: Resend the panelist invitation email.
      operationId: resendPanelistInvitation
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeypanelistspanelistkeyresendinvitation-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Panelists
      - PanelistKey
      - ResendInvitation