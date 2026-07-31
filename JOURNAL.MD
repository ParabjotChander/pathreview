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

## Week 8 — Reproduction & solution planning

**Reproduction commit link:** 
<!-- [link to commit documenting the reproduced issue] -->
https://github.com/ParabjotChander/pathreview/commit/872088b9d7f3089c33b7e60c9def4975a47b2458 

**Reproduction summary:**
<!-- [1–2 sentences: How did you reproduce the issue? What did you observe?] -->
I reproduced the bug by opening the api md file in the path pathreview/docs/API.md. I observed that curl commands for the API endpoints are missing, so developers setting up the project for the first time can't quickly verify the API is working.

**PLAN.md link:** 
<!-- [link to PLAN.md in your fork] -->
https://github.com/ParabjotChander/pathreview/blob/docs/117-update-api-guide/PLAN.md

**Walkthrough video (recommended):** 
<!-- [link to your Loom video, ≤2 min — recommended, not graded] -->
https://youtu.be/MFJTEtYZdf4 

**Blockers or open questions:**
<!--[Anything you're still uncertain about going into Week 9, or leave blank] -->

## Week 9 — Solution building & PR submission

### Check-in 1 (mid-week)

**Current progress:**
[What have you implemented so far? Which sub-tasks from PLAN.md are done?]

I have implemented the solution, meaning the sub-tasks are done from the PLAN.md file. Each api endpoint in the docs/API.md file has a sample curl command. I tested each curl command by manually entering it in the terminal and conducted CLI tests.

**Next steps:**
[What are you working on for the rest of the week?]

For the rest of the week, I have to create a demo video where I will run a sample curl command as an example to show my work. Next, I will create a draft PR, receive feedback from my draft. Lastly, I will create and submit my final pull request.

**Blockers:**
[Anything slowing you down? Or leave blank.]

Nothing is slowing me down currently.

### Check-in 2 (end of week)

**PR link:** [link to your submitted pull request]

https://github.com/ascherj/pathreview/pull/411 

**Branch:** [the branch name you worked on, e.g. `fix/123-short-description`]

`docs/117-update-api-guide`

**What you built:**
[1–3 sentences summarizing what your fix does and how it works]

Updated docs/API.md to include sample curl commands and expected HTTP response codes for each API endpoint. This provides developers with ready-to-use commands and necessary context to quickly verify that the API is functioning properly on port 8000.

**Tests added or updated:**
[Which test files did you touch? What do they cover?]

I didn't touch any test files but manually checked my work on the terminal and through the logs. I started the Docker containers and executed test requests against the application across two CLI sessions. Confirmed successful endpoint functionality by observing 2xx HTTP response codes in the application logs for each curl command executed. I ran `make check` and `make test-unit` to note which failures exist before I started the fix. After my changes, I ran both commands again and confirmed my changes didn't introduce any new failures.

**Self-review confirmation:** [X] make check passes  [X] make test-unit passes

**Draft PR feedback received from:** [name or Slack handle, or "none"]

none