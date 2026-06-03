**Issue URL:** 

**Environment:** Local / Staging / Production

**Platform(s):** Web / iOS / Android / Desktop / mWeb

**Version Number:** 

---

### Action Performed
1. 
2. 
3. 

### Expected Result


### Actual Result


---

### Environment Results
| Environment | Reproducible? | Notes |
| ----------- | ------------- | ----- |
| Production  | Yes / No      |       |
| Local       | Yes / No      |       |

### Evidence
<screenshots / recordings / logs>

---

### Note:
**How I'll reproduce locally** — once you give me the steps, I'll launch the app with the `/playwright-app-testing` skill (browser automation against the local dev server) and walk through your "Action Performed" steps, comparing what I see against your "Expected" vs "Actual".

- **If it reproduces** — I'll capture evidence (screenshots/logs) and you can ask me to re-run it as many times as you need to understand it.
- **If it does NOT reproduce** — I'll investigate why: check whether it was already fixed by another PR, whether it's backend-dependent (and therefore not reproducible against a local-only frontend), environment/feature-flag specific, or data-dependent. I'll report my findings either way.

One thing worth flagging up front: per the project's `CLAUDE.md`, the local dev server runs on the host machine, not in this container, and the local web build talks to backend services that may not be available here. Some bugs (especially backend-driven ones) may only be reproducible against staging/production. If your bug looks backend-dependent, I'll recommend we also try staging.
