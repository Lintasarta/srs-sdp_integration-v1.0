# Functional Requirements Table

| ID | Functional Requirements | Description |
|---|---|---|
|  | **Ticket Submission** |  |
| TIC-001 | Create Ticket Form Display | The system shall display a "Create Ticket" form for users to submit new support requests. |
| TIC-002 | Mandatory Fields | The "Create Ticket" form shall mark the following fields as mandatory: "Subject Ticket", "Project Name", "Request Type Ticket", "Priority Ticket", and "Product". |
| TIC-003 | Request Type Options | The "Request Type Ticket" field shall be a dropdown with options "Information Request" and "Problem Report". |
| TIC-004 | Priority Level Options | The "Priority Ticket" field shall be a dropdown with options "Minor", "Major", and "Critical". |
| TIC-005 | Product Selection | The "Product" field shall be a dropdown listing specific Cloudeka GPU product names. |
| TIC-006 | Submit Action | Upon clicking "Submit", the system shall validate the form and initiate ticket creation. |
| TIC-007 | Cancel Action | Upon clicking "Cancel", the system shall clear the form or navigate back to the previous screen. |
| TIC-008 | Submission Confirmation | The system shall display a confirmation message to the user upon successful ticket submission. |
|  | **Ticket Viewing & Monitoring** |  |
| TIC-009 | Ticket Dashboard Display | The system shall display a "Ticket" dashboard to users, listing all their submitted tickets in a table format. |
| TIC-010 | Dashboard Columns | The ticket dashboard table shall include columns for "Ticket Number", "Subject", "Priority", "Project", "Request Type", "Site", "Created Date", and "Status". |
| TIC-011 | Filtering Options | Users shall be able to filter the ticket list by "Project Name", "Request Type", and "Status". |
| TIC-012 | Pagination | The ticket dashboard shall support pagination with a configurable "Items per page" selector. |
| TIC-013 | Create Ticket Link | The dashboard shall include a "+ Create Ticket" button to navigate to the ticket submission form. |
| TIC-014 | Empty State Message | When no tickets are present, the dashboard shall display a message "Looks like you don't have any Ticket". |
| TIC-015 | Ticket Detail Access | Users shall be able to click on a ticket in the dashboard to view its full details. |
| TIC-016 | Current Status Display | The ticket detail view shall display the current status of the ticket as updated from the Service Desk Portal. |
| TIC-017 | Description Display | The ticket detail view shall display the initial "Description" provided during submission. |
| TIC-018 | Historical Tickets | All submitted tickets, including "Closed" tickets, shall remain visible in the user's dashboard for historical reference without any time limit on history maintained. |
|  | **Ticket Discussion** |  |
| TIC-019 | Discussion Section | The ticket detail view shall include a "Discussion" section for text-based communication. |
| TIC-020 | Post User Message | Users shall be able to type and post messages into the discussion section. |
| TIC-021 | Display Discussion History | The discussion section shall display all messages (from both user and operation team) in a chronological, chat-like format. |
|  | **Attachment Management** |  |
| TIC-022 | Attachment Tab | The ticket detail view shall include an "Attachment" tab or section. |
| TIC-023 | Upload Attachments | Users shall be able to upload files and images of any type to the ticket via the attachment tab. |
| TIC-024 | Attachment List Display | Attachments shall be displayed as a list of file names in the attachment tab; images will not be shown as full previews. |
| TIC-025 | Add New Attachments | New attachments from either user or operation team will be added to the existing list, without versioning. |

