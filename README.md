# ● Kalt — Index

This project is a polyrepo containing applications, shared packages, and domain-, integration-, and core-services.


```mermaid
block-beta
  columns 8
  Web["Web"] Native["Native"] Agents["Agents"] space SAP["SAP"] Bigcommerce["Bigcommerce"] Relex["Relex"] Databricks["Databricks"]
  Catalogue["API &amp; MCP Catalogue"]:3 space:5
  DS1["Domain Service"] space DS2["Domain Service"] space IS1(["Integration Service"]) IS2(["Integration Service"]) IS3(["Integration Service"]) IS4(["Integration Service"])
  Streams["Message Streams"]:8

  Web -- "REST" --> Catalogue
  Native -- "REST" --> Catalogue
  Agents -- "REST" --> Catalogue

  SAP -- "REST" --> IS1
  Bigcommerce -- "REST" --> IS2
  Relex -- "BLOB" --> IS3
  Databricks -- "SQL" --> IS4

  DS1 -- "PUB" --> Streams
  DS1 -- "SUB" --> Streams
  DS2 -- "PUB" --> Streams
  DS2 -- "SUB" --> Streams
  IS1 -- "PUB" --> Streams
  IS1 -- "SUB" --> Streams
  IS2 -- "PUB" --> Streams
  IS2 -- "SUB" --> Streams
  IS3 -- "PUB" --> Streams
  IS3 -- "SUB" --> Streams
  IS4 -- "PUB" --> Streams
  IS4 -- "SUB" --> Streams
```



## Apps

### [app.web](https://github.com/k-lt/app.web)
________
## Services
### Domain services:
### → `svc.applications`
Overview of the preferred applications on the website, that are scored against criteria. [**𝚛𝚎𝚊𝚍 𝚖𝚘𝚛𝚎 ↗**](https://github.com/k-lt/svc.applications)

### → `svc.companies`
Overview of all the companies in the system. [**𝚛𝚎𝚊𝚍 𝚖𝚘𝚛𝚎 ↗**](https://github.com/k-lt/svc.companies)

### → [svc.communications](https://github.com/k-lt/svc.communications)
### → [svc.clients](https://github.com/k-lt/svc.clients)
### → [svc.countries](https://github.com/k-lt/svc.countries)
### → [svc.direction](https://github.com/k-lt/svc.direction)
### → [svc.dm](https://github.com/k-lt/svc.dm)
### → [svc.doctrine](https://github.com/k-lt/svc.doctrine)
### → [svc.geo](https://github.com/k-lt/svc.geo)
### → [svc.roadmaps](https://github.com/k-lt/svc.roadmaps)
### → [svc.platform](https://github.com/k-lt/svc.platform)
### → [svc.publications](https://github.com/k-lt/svc.publications)
### → [svc.products](https://github.com/k-lt/svc.products)
### → [svc.search](https://github.com/k-lt/svc.search)
### → [svc.tasks](https://github.com/k-lt/svc.tasks)
### → [svc.workspaces](https://github.com/k-lt/svc.workspaces)
### → [svc.workforce](https://github.com/k-lt/svc.workforce)

### Integration services: 
### → [svc.int-linear](https://github.com/k-lt/svc.int-linear)
Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

Read more ↗

### →[svc.int-github](https://github.com/k-lt/svc.int-github)
Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

Read more ↗

### → [svc.int-google-workspace](https://github.com/k-lt/svc.int-google-workspace)
Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

Read more ↗

### → [svc.int-notion](https://github.com/k-lt/svc.int-notion)
Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

Read more ↗

### → [svc.int-salesforce](https://github.com/k-lt/svc.int-salesforce)
Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

𝗿𝗲𝗮𝗱 𝗺𝗼𝗿𝗲 ↗
________
### [core.psql](https://github.com/k-lt/core.psql)
### [core.observe](https://github.com/k-lt/core.observe)
### [core.inference](https://github.com/k-lt/core.inference)
### [core.auth](https://github.com/k-lt/core.auth)
### [core.blob](https://github.com/k-lt/core.blob)
### core.channels
All domain and integration services communicate using event carried state transfers [⁰¹](https://github.com/k-lt/index/blob/main/concepts.md#-event-carried-state-transfers) on redis streams through the shared HA. [ʀᴇᴀᴅ ᴍᴏʀᴇ **↗**](https://github.com/k-lt/core.channels)

### [core.gateway](https://github.com/k-lt/core.gateway)
### [core.node](https://github.com/k-lt/core.node)
### [pkg.auth](https://github.com/k-lt/pkg.auth)
### [pkg.psql](https://github.com/k-lt/pkg.psql)
### [pkg.gateway](https://github.com/k-lt/pkg.gateway)
### [pkg.contracts](https://github.com/k-lt/pkg.contracts)
### [pkg.channels](https://github.com/k-lt/pkg.channels)
### [pkg.observe](https://github.com/k-lt/pkg.observe)



⁰¹²³⁴⁵⁶⁷⁸⁹