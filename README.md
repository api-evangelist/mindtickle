# Mindtickle

Mindtickle is an AI-powered revenue productivity platform that unifies sales enablement, training, coaching, conversation intelligence, and digital sales rooms into a single solution for customer-facing revenue teams.

## APIs

- **REST API** — Core platform API for users, groups, modules, learner analytics, and reporting (`https://api.mindtickle.com`). Authenticated via JWT Bearer token (API Key + Secret Key + Client ID obtained from the Mindtickle admin console).
- **Call AI GraphQL API** — Public GraphQL API for call recordings, transcriptions, coaching scores, and conversation intelligence (`https://api-gateway.callai.www.mindtickle.com/public/graphapi`). Authenticated via OAuth 2.0.

## Authentication

- JWT Bearer token (REST API): Generate credentials under Settings > API Access in the Mindtickle admin console. Tokens expire after 1 hour.
- OAuth 2.0 (Call AI GraphQL API): Pass the access token in the Authorization header of GraphQL requests.

## Rate Limits

- 4 requests per second per account
- 60 requests per minute per account
- HTTP 429 returned when limits are exceeded; implement exponential backoff.

## Key Platform Capabilities

- Sales readiness and onboarding programs
- Content management and assignment
- Call AI: recording, transcription, coaching, and scoring
- Digital sales rooms for buyer engagement
- Revenue intelligence and forecasting
- 100+ pre-built integrations (Salesforce, Microsoft, Google, Workday, Slack, and more)
- SCIM, SAML, OpenID Connect, JWT SSO support

## Links

- Website: https://www.mindtickle.com/
- Platform: https://www.mindtickle.com/platform/
- Integrations: https://www.mindtickle.com/platform/integrations/
- Blog: https://www.mindtickle.com/blog/
- Status: https://status.mindtickle.com
- Support: https://help.mindtickle.com/
