# Communication Interface

- **Cloudeka Service Portal to ServiceDesk Plus:** The service portal (ai.cloudeka.id and ai.cloudeka.id) communicates with the Deka Container Registry backend services using HTTPS REST API calls. This ensures secure transmission of data and commands between the user interface and the registry's core functionalities. The communication may also include authentication tokens or session identifiers for secure user interactions.
  - **Protocol:** HTTPS REST API calls.
  - **Purpose:** To create new tickets in SDP, add discussion entries from the user, and upload attachments from the user.
  - **Authentication:** Secure API authentication (e.g., API keys, OAuth tokens) as per ServiceDesk Plus requirements.
- **ServiceDesk Plus to Cloudeka Service Portal:**
  - **Protocol:** Webhooks (HTTPS POST requests initiated by ServiceDesk Plus).
  - **Purpose:** To notify the Cloudeka Service Portal of updates made in SDP, such as status changes, new discussion entries, or attachment uploads.
  - **Synchronization Logic:** Upon receiving a webhook notification, the Cloudeka Service Portal will pull the updated ticket details (status, discussion, attachments) from ServiceDesk Plus using its API.
- **Data Format:** JSON will be used for API request/response bodies.
