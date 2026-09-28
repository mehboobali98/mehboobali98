<picture>
  <source media="(prefers-color-scheme: dark)" srcset=".github/assets/header-dark.png">
  <img src=".github/assets/header-light.png" alt="Backend Engineer. Ruby on Rails, 5+ years. AI-assisted engineering with Claude Code and Cursor. Lines fan out to MySQL, AWS, React and TypeScript." width="100%">
</picture>

## Mehboob Ali

**Senior Backend Engineer** (Ruby on Rails) &nbsp;·&nbsp; Principal Software Engineer at 7Vals &nbsp;·&nbsp; Lahore, Pakistan &nbsp;·&nbsp; [mehboob.dev](https://mehboob.dev)

Five years at [7Vals](https://7vals.com) on Rails backends and IT-asset systems. I led the CMDB build
and I run our workflow automation program now. The tooling side got interesting along the way: a
Redmine CLI, and Claude Code skills built on it that estimate work against the real codebase. I've
also reviewed pull requests from 40+ engineers and interviewed about 100 candidates since 2022.

<p>
  <img alt="Ruby" src="https://img.shields.io/badge/Ruby-1f2328?style=flat-square&logo=ruby&logoColor=white"/>
  <img alt="Rails" src="https://img.shields.io/badge/Rails-1f2328?style=flat-square&logo=rubyonrails&logoColor=white"/>
  <img alt="Go" src="https://img.shields.io/badge/Go-1f2328?style=flat-square&logo=go&logoColor=white"/>
  <img alt="MySQL" src="https://img.shields.io/badge/MySQL-1f2328?style=flat-square&logo=mysql&logoColor=white"/>
  <img alt="React" src="https://img.shields.io/badge/React-1f2328?style=flat-square&logo=react&logoColor=white"/>
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-1f2328?style=flat-square&logo=typescript&logoColor=white"/>
</p>

### Open source

- **[rmine](https://github.com/mehboobali98/rmine)** &nbsp;`Go`<br>
  Redmine from a terminal, built for two callers from the start: me, and a coding agent. Structured output, profiles, time logging, an embedded Claude Code skill, tagged releases. My team at 7Vals uses it with rmine-skills.
- **[rmine-skills](https://github.com/mehboobali98/rmine-skills)** &nbsp;`Python`<br>
  Six workflows on top of rmine. `/estimate` refuses to price a spec it can't read, grounds each line item in the real codebase, then hands the result to a validator that never sees how it was derived. `/calibrate` checks the whole rubric against hours actually logged.
- **[bitwise_attributes](https://github.com/mehboobali98/bitwise_attributes)** &nbsp;`Ruby`<br>
  Packs boolean flag attributes into a single ActiveRecord integer column, with generated scopes, validations and inheritance behavior. An internal pattern I used for two years before publishing it.
- **[whatsapp-status-translator](https://github.com/mehboobali98/whatsapp-status-translator)** &nbsp;`JavaScript`<br>
  One-click translate for WhatsApp Web Status captions, the one surface WhatsApp's own translate feature leaves out. A Manifest V3 worker over a DOM I don't control and can't rely on.

### What I've shipped at work

Closed source, so here is what they were and what they had to solve.

**[The sync job that took half a day](https://mehboob.dev/blog/the-sync-job-that-took-half-a-day/)** &nbsp;·&nbsp; `Rails` `Delayed Job` `MySQL`
> A device sync was taking 12 to 15 hours to run, so new hardware wouldn't show up for most of a
> working day. N+1 queries and no batching, on a table that had been collecting devices for years.
> Rebuilt around batched writes: under an hour now, and the MDM integrations added since reuse the
> same pattern.

**Automation that could branch** &nbsp;·&nbsp; `Rails` `React Flow` `ITSM`
> Automation used to be one trigger paired with one sub-trigger. Fine for a one-step rule, out of
> room past that. It's a node canvas now: actions chain, each branches on success or failure, and
> every run writes a step-by-step log, so a rule that misfires can be read instead of guessed at.
> Led technical delivery with a team of about eight engineers, and built the HTTP request node,
> webhook triggers and branching myself. It's the program I still run.
> [Documented by EZO ↗](https://ezo.io/assetsonar/blog/automation-engine/)

**A CMDB that actually models relationships** &nbsp;·&nbsp; `Rails` `MySQL` `Graph modeling`
> Most CMDBs are static. An asset points at a user, maybe a location, and anything past that takes
> a support ticket. This one answers *everything touching this server, three hops out*: a data model
> with n-level traversal plus the ITSM-integrated UI on top. About seven months from architecture
> to production, leading a five-person team. I wrote the design RFCs and built the new module's backend.
> [Documented by EZO ↗](https://ezo.io/assetsonar/blog/visualize-cmdb-relationships-assetsonar-it-graph/)

**Telling devices apart when the serial is wrong** &nbsp;·&nbsp; `Rails` `MySQL`
> Asset records were keyed on the BIOS serial, and some devices report a junk one, so a single
> laptop could turn into several assets or two machines could merge into one. I built matching that
> spots invalid serials, falls back to the MAC address, and lets each company keep its own list of
> serials not to trust.

Four titles in five years, and what stayed behind after each one: [mehboob.dev/#trajectory](https://mehboob.dev/#trajectory).

### Writing

- [What changed when an agent started using my CLI](https://mehboob.dev/blog/designing-a-cli-for-agents/): rmine was built for two callers from the start: me at a terminal, and a coding agent.
- [Three agents that don't trust each other](https://mehboob.dev/blog/three-agents-that-dont-trust-each-other/): an effort estimator built from three subagents. What mattered was what to withhold from each one.
- [I used it internally for two years before publishing it](https://mehboob.dev/blog/two-years-before-i-published-it/): most of what makes something a library rather than a snippet lives in that gap.

More at [mehboob.dev/blog](https://mehboob.dev/blog/) &nbsp;·&nbsp; [RSS](https://mehboob.dev/rss.xml)

### Elsewhere

[mehboob.dev](https://mehboob.dev) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/mehboobali98/) &nbsp;·&nbsp; [mehboob@mehboob.dev](mailto:mehboob@mehboob.dev)

<sub>Earlier work, before Rails: Python, Java, Android, Spring. Mostly in the 2021 repos below.</sub>
