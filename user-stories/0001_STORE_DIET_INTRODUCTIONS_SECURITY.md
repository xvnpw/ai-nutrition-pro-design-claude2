# (AI Generated) Security Related Acceptance Criteria
**API Gateway**
- **AC1:** The API Gateway must implement input validation and sanitization on all external requests before sending them to backend services
- **AC2:** The API Gateway must use OAuth2 tokens or short-lived API keys instead of long-lived API keys for authentication
- **AC3:** The API Gateway must enforce rate limiting to prevent denial of service attacks

**API Application**
- **AC1:** The API Application must undergo secure code review, static analysis, dynamic analysis and fuzz testing to identify and remediate vulnerabilities
- **AC2:** The API Application must use TLS 1.2+ to encrypt network traffic between itself and the API Database

**API Database**
- **AC1:** The API Database must enforce role-based access control and least privilege permissions
- **AC2:** The API Database must require strong authentication for access

