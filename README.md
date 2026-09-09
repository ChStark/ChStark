# Jorge Garza

Backend & DevOps engineer in Apodaca, Nuevo León, México · UTC-6

**Go**, **Java**, **PostgreSQL**, **Kubernetes**, **CI/CD** — one person for both halves,
so there's no separate ops hire.

I also have an **Operations Research M.Sc. that I've actually put into production**: a
real-time delivery-routing optimizer (OptaPlanner) that took throughput from 2 to 5 orders
per driver-hour. Routing, scheduling, allocation and capacity problems are the ones I enjoy
most.

I'm comfortable building under regulation — four years at a licensed Mexican fintech
integrating **SPEI** and **STP** payment rails against CNBV requirements, and before that
SEC 13F/13G compliance regression testing at Goldman Sachs.

**Most of my work is in private GitLab repositories** — client and product code that isn't
mine to publish. What's here is the subset I can open source, plus the tooling I've built
around my own workflow.

### Public work

| | |
|---|---|
| **[agentctl](https://github.com/ChStark/agentctl)** · Go · Kubernetes | Turns GitLab milestones into merged merge requests. Isolated pods pick up *groups* of related issues, open MRs, and the ones that pass their project's own CI and touch no protected path merge themselves. Grouping is the point: two agents editing the same service produce two MRs that can't both merge, and you find out after paying for both. Ships with an explicit trust model — per-run tokens scoped to one project, no ServiceAccount in the pod, RFC1918 egress blocked, read-only rootfs. |
| **[aiwebcam](https://github.com/ChStark/aiwebcam)** · Flutter · Dart | Turns a phone into a networked camera and sensor server, with an **MCP endpoint so an AI agent can see through and control the camera**. Runs an HTTP/HTTPS server on the device; the TLS identity is generated on first launch rather than shipped, so no two installs share a key. |
| **[claude-approvals](https://github.com/ChStark/claude-approvals)** · Python · FastAPI | Resolves Claude Code permission prompts through Discord Allow/Deny buttons instead of blocking the terminal. In-memory state on purpose: a restart or timeout expires the request and the caller falls back to the normal interactive prompt rather than auto-allowing. |

### How I work

I use AI coding tools heavily — Claude Code daily — and I'm specific about what that means:
small diffs, I read every line that carries my name, and tests, linters and type-checks are
the gate before anything ships. The speed is real; the review discipline is what makes it
safe to use. `agentctl` is that opinion written down as software.

### Stack

Go · Java · Vue.js · Node.js · PostgreSQL · MySQL · Redis · Kubernetes · Docker ·
GitLab CI/CD · Jenkins · Cloudflare · AWS · Linux · Laravel · OptaPlanner

**Available for freelance and contract work**, part-time, remote — full overlap with US and
Canadian business hours. Bilingual (native Spanish, professional English).

📫 christopheriq@gmail.com · 🌐 [blackengine.com.mx](https://blackengine.com.mx)
