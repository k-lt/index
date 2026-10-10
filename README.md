# ● Kalt — Index

This project is a polyrepo containing applications, shared packages, and domain-, integration-, and core-services.


<img src="architecture.svg" alt="Web, native, and agents call core.gateway. Domain services sit behind the gateway. Off-the-shelf systems connect to integration services over REST, BLOB, or SQL. Domain and integration services publish and subscribe on Channels." width="100%">

## Apps

### [app.web](https://github.com/k-lt/app.web)
________
## Services
### Domain services:
### Applications
`svc.applications` – [![read more](readmore.svg)](https://github.com/k-lt/svc.applications)

Overview of the preferred applications on the website, that are scored against criteria.

### Companies
`svc.companies` – [![read more](readmore.svg)](https://github.com/k-lt/svc.companies)

Overview of all the companies in the system.

### Communications
`svc.communications` – [![read more](readmore.svg)](https://github.com/k-lt/svc.communications)

### Clients
`svc.clients` – [![read more](readmore.svg)](https://github.com/k-lt/svc.clients)

Clients is the .

### Countries
`svc.countries` – [![read more](readmore.svg)](https://github.com/k-lt/svc.countries)

Overview of all countries in the world. Available via API, MCP and through domain messages to other services.

### Direction
`svc.direction` – [![read more](readmore.svg)](https://github.com/k-lt/svc.direction)

### DM
`svc.dm` – [![read more](readmore.svg)](https://github.com/k-lt/svc.dm)

The DM service is a super lightweight and minimal chatting service that support both agents and real humans to talk together in threads, it pull together both external and internal people into the same chat rooms.

### Doctrine
`svc.doctrine` – [![read more](readmore.svg)](https://github.com/k-lt/svc.doctrine)

### Geo
`svc.geo` – [![read more](readmore.svg)](https://github.com/k-lt/svc.geo)

### Roadmaps
`svc.roadmaps` – [![read more](readmore.svg)](https://github.com/k-lt/svc.roadmaps)

### Platform
`svc.platform` – [![read more](readmore.svg)](https://github.com/k-lt/svc.platform)

### Publications
`svc.publications` – [![read more](readmore.svg)](https://github.com/k-lt/svc.publications)

### Products
`svc.products` – [![read more](readmore.svg)](https://github.com/k-lt/svc.products)

### Search
`svc.search` – [![read more](readmore.svg)](https://github.com/k-lt/svc.search)

### Tasks
`svc.tasks` – [![read more](readmore.svg)](https://github.com/k-lt/svc.tasks)

### Workspaces
`svc.workspaces` – [![read more](readmore.svg)](https://github.com/k-lt/svc.workspaces)

### Workforce
`svc.workforce` – [![read more](readmore.svg)](https://github.com/k-lt/svc.workforce)

### Integration services:
### Linear
`svc.int-linear` – [![read more](readmore.svg)](https://github.com/k-lt/svc.int-linear)

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### GitHub
`svc.int-github` – [![read more](readmore.svg)](https://github.com/k-lt/svc.int-github)

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### Google Workspace
`svc.int-google-workspace` – [![read more](readmore.svg)](https://github.com/k-lt/svc.int-google-workspace)

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### Notion
`svc.int-notion` – [![read more](readmore.svg)](https://github.com/k-lt/svc.int-notion)

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### Salesforce
`svc.int-salesforce` – [![read more](readmore.svg)](https://github.com/k-lt/svc.int-salesforce)

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