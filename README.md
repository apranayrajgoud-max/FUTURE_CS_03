# API Security Risk Analysis

**Intern:** Alugani Pranay Raj Goud  
**Program:** Future Interns — Cybersecurity Internship (2026)  
**Task:** Task 3 — API Security Risk Analysis

---

## Target API
JSONPlaceholder — https://jsonplaceholder.typicode.com  
(Public REST API built for developer testing and learning)

---

## Tools Used
- Google Chrome Browser (address bar for GET requests)
- Chrome DevTools — Network Tab (header and response inspection)
- Chrome DevTools — Console Tab (POST and DELETE testing via Fetch API)

---

## Scope
- Read-only, ethical analysis
- No exploitation, no DoS, no data permanently modified
- Testing standard: OWASP API Security Top 10 (2023)

---

## Methodology
1. Reviewed JSONPlaceholder API documentation
2. Tested GET endpoints directly from the browser address bar
3. Inspected Response Headers for rate limiting controls
4. Used browser Console to test POST and DELETE requests without authentication
5. Identified risks and classified each by severity (High / Medium / Low)
6. Documented findings with business impact and remediation steps

---

## Findings Summary

| # | Risk | Severity | Endpoint |
|---|------|----------|----------|
| 1 | Unauthenticated user data listing | High | GET /users |
| 2 | IDOR — user enumeration | High | GET /users/{id} |
| 3 | Unauthenticated POST (write access) | High | POST /posts |
| 4 | Unauthenticated DELETE | High | DELETE /posts/1 |
| 5 | Missing rate limiting | Medium | All endpoints |

---

## Repository Contents
- `report.pdf` — Full API Security Risk Analysis Report
- `screenshots/` — Chrome DevTools screenshots from all tests

---

## References
- OWASP API Security Top 10: https://github.com/OWASP/API-Security
- API Security Checklist: https://github.com/shieldfy/API-Security-Checklist
```

3. Click **Commit changes**

---

## Step 5 — Upload Your Report PDF
1. In your repo, click **Add file** → **Upload files**
2. Drag and drop your `report.pdf`
3. Scroll down → click **Commit changes**

---

## Step 6 — Upload Screenshots
1. Click **Add file** → **Upload files**
2. Upload all your screenshots
3. In the commit message type: `Add DevTools screenshots`
4. Click **Commit changes**

---

## Step 7 — Copy Your Repo Link
Your repo link will look like:
```
https://github.com/YourUsername/api-security-risk-analysis
