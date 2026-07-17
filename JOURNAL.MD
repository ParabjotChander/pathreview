## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/117

**Issue title:** API docs don't include example curl commands #117

**Tier:** Tier 1 

**Problem summary:**
<!-- In 3–5 sentences, in your own words: what the issue is (not a copy-paste of
the title), what is currently broken or missing, and what a successful fix
would accomplish. Naming the part of the codebase it affects is helpful context.]
-->
The problem is that the API endpoints are stated but there are no sample curl commands for the user & developer to run to verify that the API is working. The docs/API.MD file is missing examples for each API endpoint stated. A successful fix would be having curl commands shown in the md file for GET /health, POST /auth/register, POST/auth/login, POST /profiles, GET /profiles/[profile id], DELETE /profiles/[profile id], POST /reviews, GET /reviews/[review id] and GET /reviews. This would help developers and users verify the API works by inserting the curl commands provided in their CLI. 

**Selection Notes**
I read the issue comments, the issue is recorded so the cohort can see what I am working on. The issue comment states the estimated time for completion is 2-3 hours, I can do this before the week 9 deadline. The scope for this issue is the docs/API.md file (where I will add the curl commands for the API endpoints) and api/routes/ folder (where the route files are located, to discover the routes, part of codebase to orient).

**Branch name:** docs/117-update-api-guide

**Setup confirmation:** App runs locally at localhost:5173

**Cohort ledger:** Issue added to cohort ledger