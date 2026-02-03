# Use Case Description

#### Action and Response

| Action by user | Response from system |
|---|---|
| User initiates creation of a new ticket via Service Portal form. | System displays ticket creation form. Upon submission, system validates form, creates ticket in ServiceDesk Plus via API, and displays confirmation message. |
| User views the list of existing tickets on their dashboard. | System displays a list of all accessible tickets with their key details, fetching current status from ServiceDesk Plus. |
| User clicks on a ticket in the dashboard. | System displays the full details of the selected ticket, including current status, discussion history, and attachment list, synchronized from ServiceDesk Plus. |
| User posts a new message in the ticket's discussion section. | System adds the new message to the local discussion view and sends it to ServiceDesk Plus via API as a new note/comment. |
| User uploads an attachment to a ticket. | System uploads the attachment to ServiceDesk Plus via API, and the attachment is listed in the ticket's attachment tab on both portals. |
| Administrator (in ServiceDesk Plus) updates ticket status. | ServiceDesk Plus triggers a webhook to Cloudeka Service Portal. System fetches updated status via API and updates the ticket display. |
| Administrator (in ServiceDesk Plus) adds a new note/comment in discussion. | ServiceDesk Plus triggers a webhook to Cloudeka Service Portal. System fetches the new note via API and adds it to the discussion section. |
| Administrator (in ServiceDesk Plus) uploads an attachment. | ServiceDesk Plus triggers a webhook to Cloudeka Service Portal. System fetches the new attachment details via API and adds it to the attachment list. |

