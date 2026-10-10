# ● Kalt — Index

This project is a polyrepo containing applications, shared packages, and domain-, integration-, and core-services.


```mermaid
block-beta
  columns 15
  Web["Web"]:2 Native["Native"]:2 Agents["Agents"]:2 space OtsA["Off-the-shelf A"]:2 OtsB["Off-the-shelf B"]:2 OtsC["Off-the-shelf C"]:2 OtsD["Off-the-shelf D"]:2
  Catalogue["API &amp; MCP Catalogue"]:6 space:9
  DS1["Domain Service"]:2 space:2 DS2["Domain Service"]:2 space IS1(["Integration Service"]):2 IS2(["Integration Service"]):2 IS3(["Integration Service"]):2 IS4(["Integration Service"]):2
  P1["PUB"] S1["SUB"] space:2 P2["PUB"] S2["SUB"] space P3["PUB"] S3["SUB"] P4["PUB"] S4["SUB"] P5["PUB"] S5["SUB"] P6["PUB"] S6["SUB"]
  Streams["Message Streams"]:15

  Web -- "REST" --> Catalogue
  Native -- "REST" --> Catalogue
  Agents -- "REST" --> Catalogue

  OtsA -- "REST" --> IS1
  OtsB -- "REST" --> IS2
  OtsC -- "BLOB" --> IS3
  OtsD -- "SQL" --> IS4

  DS1 --> P1
  DS1 --> S1
  DS2 --> P2
  DS2 --> S2
  IS1 --> P3
  IS1 --> S3
  IS2 --> P4
  IS2 --> S4
  IS3 --> P5
  IS3 --> S5
  IS4 --> P6
  IS4 --> S6

  P1 --> Streams
  S1 --> Streams
  P2 --> Streams
  S2 --> Streams
  P3 --> Streams
  S3 --> Streams
  P4 --> Streams
  S4 --> Streams
  P5 --> Streams
  S5 --> Streams
  P6 --> Streams
  S6 --> Streams

  style P1,S1,P2,S2,P3,S3,P4,S4,P5,S5,P6,S6 fill:transparent,stroke:transparent
```



## Apps

### [app.web](https://github.com/k-lt/app.web)
________
## Services
### Domain services:
### → svc.applications
Overview of the preferred applications on the website, that are scored against criteria. [ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/svc.applications)

### → svc.companies
Overview of all the companies in the system. [ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/svc.companies)

### → svc.communications

[ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/svc.communications)

### → svc.clients

Clients is the . [ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/svc.clients)
### → [svc.countries](https://github.com/k-lt/svc.countries)
### → [svc.direction](https://github.com/k-lt/svc.direction)
### → svc.dm

The DM service is a super lightweight and minimal chatting service that support both agents and real humans to talk together in threads, it pull together both external and internal people into the same chat rooms. [ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/svc.dm)

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
All domain and integration services communicate using event carried state transfers [⁰¹](https://github.com/k-lt/index/blob/main/concepts.md#-event-carried-state-transfers) on redis streams through the shared HA. [ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/core.channels)

### [core.gateway](https://github.com/k-lt/core.gateway)
### [core.node](https://github.com/k-lt/core.node)
### [pkg.auth](https://github.com/k-lt/pkg.auth)
### [pkg.psql](https://github.com/k-lt/pkg.psql)
### [pkg.gateway](https://github.com/k-lt/pkg.gateway)
### [pkg.contracts](https://github.com/k-lt/pkg.contracts)
### [pkg.channels](https://github.com/k-lt/pkg.channels)
### [pkg.observe](https://github.com/k-lt/pkg.observe)



⁰¹²³⁴⁵⁶⁷⁸⁹