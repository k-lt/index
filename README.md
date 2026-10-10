# ● Kalt — Index

This project is a polyrepo containing applications, shared packages, and domain-, integration-, and core-services.


<img src="architecture.svg" alt="Web, native, and agents call core.gateway. Domain services sit behind the gateway. Off-the-shelf systems connect to integration services over REST, BLOB, or SQL. Domain and integration services publish and subscribe on Channels." width="100%">

## Apps

### [app.web](https://github.com/k-lt/app.web)
________
## Services
### Domain services:
### Applications
`svc.applications` – <a href="https://github.com/k-lt/svc.applications"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

Overview of the preferred applications on the website, that are scored against criteria.

### Companies
`svc.companies` – <a href="https://github.com/k-lt/svc.companies"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

Overview of all the companies in the system.

### Communications
`svc.communications` – <a href="https://github.com/k-lt/svc.communications"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Clients
`svc.clients` – <a href="https://github.com/k-lt/svc.clients"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

Clients is the .

### Countries
`svc.countries` – <a href="https://github.com/k-lt/svc.countries"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

Overview of all countries in the world. Available via API, MCP and through domain messages to other services.

### Direction
`svc.direction` – <a href="https://github.com/k-lt/svc.direction"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### DM
#### `svc.dm` – <a href="https://github.com/k-lt/svc.dm"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

The DM service is a super lightweight and minimal chatting service that support both agents and real humans to talk together in threads, it pull together both external and internal people into the same chat rooms.

### Doctrine
`svc.doctrine` – <a href="https://github.com/k-lt/svc.doctrine"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Geo
`svc.geo` – <a href="https://github.com/k-lt/svc.geo"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Roadmaps
`svc.roadmaps` – <a href="https://github.com/k-lt/svc.roadmaps"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Platform
`svc.platform` – <a href="https://github.com/k-lt/svc.platform"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Publications
`svc.publications` – <a href="https://github.com/k-lt/svc.publications"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Products
`svc.products` – <a href="https://github.com/k-lt/svc.products"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Search
`svc.search` – <a href="https://github.com/k-lt/svc.search"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Tasks
`svc.tasks` – <a href="https://github.com/k-lt/svc.tasks"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Workspaces
`svc.workspaces` – <a href="https://github.com/k-lt/svc.workspaces"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Workforce
`svc.workforce` – <a href="https://github.com/k-lt/svc.workforce"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

### Integration services:
### Linear
`svc.int-linear` – <a href="https://github.com/k-lt/svc.int-linear"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### GitHub
`svc.int-github` – <a href="https://github.com/k-lt/svc.int-github"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### Google Workspace
`svc.int-google-workspace` – <a href="https://github.com/k-lt/svc.int-google-workspace"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### Notion
`svc.int-notion` – <a href="https://github.com/k-lt/svc.int-notion"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### Salesforce
`svc.int-salesforce` – <a href="https://github.com/k-lt/svc.int-salesforce"><img alt="read more" src="readmore.svg" height="20" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

________
### [core.psql](https://github.com/k-lt/core.psql)
### [core.observe](https://github.com/k-lt/core.observe)
### core.auth
[ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/core.auth)
### core.blob
[ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/core.blob)
### core.channels
All domain and integration services communicate using event carried state transfers [⁰¹](https://github.com/k-lt/index/blob/main/concepts.md#-event-carried-state-transfers) on redis streams through the shared HA. [ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/core.channels)

### core.gateway
[ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/core.gateway)
### core.node
[ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/core.node)

### core.inference
[ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/core.inference)
### [pkg.auth](https://github.com/k-lt/pkg.auth)
### [pkg.psql](https://github.com/k-lt/pkg.psql)
### [pkg.gateway](https://github.com/k-lt/pkg.gateway)
### [pkg.contracts](https://github.com/k-lt/pkg.contracts)
### [pkg.channels](https://github.com/k-lt/pkg.channels)
### [pkg.observe](https://github.com/k-lt/pkg.observe)



⁰¹²³⁴⁵⁶⁷⁸⁹