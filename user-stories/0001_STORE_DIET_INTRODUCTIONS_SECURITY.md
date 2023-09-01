# (AI Generated) Security Related Acceptance Criteria
**API Gateway**
- **AC1:** The API Gateway must implement rate limiting per client to prevent denial of service attacks
- **AC2:** The API Gateway must validate all inputs and sanitize against injection attacks before passing requests to backend
- **AC3:** The API Gateway must require TLS 1.2 or higher for all connections

**API Application**
- **AC4:** The API Application must validate and sanitize all inputs from API Gateway before querying database
- **AC5:** The API Application must scrub any sensitive data from prompts sent to ChatGPT
- **AC6:** The API Application must implement rate limiting on ChatGPT requests

**API Database**
- **AC7:** The API Database must require strong authentication for all access
- **AC8:** The API Database must encrypt all sensitive data at rest

