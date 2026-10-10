# ● Kalt — Index

This project is a polyrepo containing applications, shared packages, and domain-, integration-, and core-services. Based on the principles from domain driven design, team topologies, and enterprise clean architecture.

<br/> <br/>


<img src="arch3.svg" alt="Web, native, and agents call core.gateway. Domain services sit behind the gateway. Off-the-shelf systems connect to integration services over REST, BLOB, or SQL. Domain and integration services publish and subscribe on Channels." width="100%">

<p align="center"> Illustration of architecture with some elements </p>

<br/> <br/>

## Contracts
`pkg.contracts`  – <a href="https://github.com/k-lt/pkg.contracts"><img alt="read more" src="pkg/contracts.svg" align="absmiddle"></a>

Everything in the platform is fully contract driven, even the source-aligned integrations has contracts they offer over the channels it distributes data on. This repository is editable by the owners of the contracts. The contracts, both for messages and for the API is versioned.

This allows us to introduce breaking changes and have the other services and applications gracefully migrate over to the next version.

This repository is made available as a GitHub Packages, and contain some minor helpers to consume some of the source-aligned events. But they never contain any domain logic or similar. 


```bash
npm install @k-lt/contracts@0.1.0
```

<br/> <br/>

## Gateway    <img src="core/infra.svg" align="absmiddle">
`core.gateway` – <a href="https://github.com/k-lt/core.gateway"><img alt="read more" src="m2.svg" align="absmiddle"></a> – <a href="https://github.com/k-lt/pkg.gw"><img alt="read more" src="pkg/gw.svg" align="absmiddle"></a>

The gateway is where all traffic inbound to the node goes through, it is based on Pingora and extended with MCP capabilites. All the domain services makes their APIs available on the gateway using the [@pkg.gw](https://github.com/k-lt/pkg.gw) library. 

That way all services' APIs feel and look the same across the board. It enforces conformity.


<br/><br/>


## Channels   <img src="core/infra.svg" align="absmiddle">
`core.channels` –  <a href="https://github.com/k-lt/core.channels"><img alt="read more" src="m2.svg" align="absmiddle"></a> – <a href="https://github.com/k-lt/pkg.ch"><img alt="read more" src="pkg/ch.svg" align="absmiddle"></a>

All domain and integration services communicate using event carried state transfers [⁰¹](https://github.com/k-lt/index/blob/main/concepts.md#-event-carried-state-transfers) on redis streams through the shared HA.

<br/><br/>


## [core.observe](https://github.com/k-lt/core.observe)

## Authentication
`core.auth`  –  <a href="https://github.com/k-lt/core.auth"><img alt="read more" src="m2.svg" align="absmiddle"></a> – <a href="https://github.com/k-lt/pkg.auth"><img alt="read more" src="pkg/auth.svg" align="absmiddle"></a>

<br/><br/>

## Blob storage
`core.blob` –  <a href="https://github.com/k-lt/core.blob"><img alt="read more" src="m2.svg" align="absmiddle"></a> – <a href="https://github.com/k-lt/core.blob"><img alt="read more" src="pkg/blob.svg" align="absmiddle"></a>


<br/> <br/>


## Bare metal nodes
`core.node` – 


[ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/core.node)


## Inference
`core.inference` – [ʀᴇᴀᴅ ᴍᴏʀᴇ ↗](https://github.com/k-lt/core.inference)

We're not building just another inference alternative, but we are hosting our own fine tuned and specialized models, and have a router to other inference providers at 0% fee.



<br/> <br/>


## Postgres databases   <img src="core/infra.svg" align="absmiddle">
`core.psql` –  <a href="https://github.com/k-lt/core.psql"><img alt="read more" src="m2.svg" align="absmiddle"></a> – <a href="https://github.com/k-lt/pkg.psql"><img alt="pkg/psql button" src="pkg/psql.svg" align="absmiddle"></a>

A centrally managed instance of Multigres that support all the services. Since everything is run on multiple nodes, we achieve HA.


<br/><br/>


## Applications
`svc.applications`  –  <a href="https://github.com/k-lt/svc.applications"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Overview of the preferred applications on the website, that are scored against a list of criteria. It is an opinionated exclusion driven list. 

<br/><br/>

## Companies
`svc.companies` – <a href="https://github.com/k-lt/svc.companies"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Overview of all the companies in the system.

<br/><br/>

## Communications
`svc.communications` – <a href="https://github.com/k-lt/svc.communications"><img alt="read more" src="m2.svg" align="absmiddle"></a>

<br/><br/>

## Clients
`svc.clients` – <a href="https://github.com/k-lt/svc.clients"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Clients is the 

<br/><br/>

## Countries
`svc.countries` – <a href="https://github.com/k-lt/svc.countries"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Overview of all countries in the world. Available via API, MCP and through domain messages to other services.

## Direction
`svc.direction` – <a href="https://github.com/k-lt/svc.direction"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Here goes the paragraph

<br/><br/>

## DM
 `svc.dm` – <a href="https://github.com/k-lt/svc.dm"><img alt="read more" src="m2.svg" align="absmiddle"></a>

The DM service is a super lightweight and minimal chatting service that support both agents and real humans to talk together in threads, it pull together both external and internal people into the same chat rooms.

<br/><br/>

## Doctrine
`svc.doctrine` – <a href="https://github.com/k-lt/svc.doctrine"><img alt="read more" src="m2.svg" align="absmiddle"></a>

## Geo
`svc.geo` – <a href="https://github.com/k-lt/svc.geo"><img alt="read more" src="m2.svg" align="absmiddle"></a>

### Roadmaps
`svc.roadmaps` – <a href="https://github.com/k-lt/svc.roadmaps"><img alt="read more" src="m2.svg" align="absmiddle"></a>

### Platform
`svc.platform` – <a href="https://github.com/k-lt/svc.platform"><img alt="read more" src="m2.svg" align="absmiddle"></a>

### Publications
`svc.publications` – <a href="https://github.com/k-lt/svc.publications"><img alt="read more" src="m2.svg" align="absmiddle"></a>

### Products
`svc.products` – <a href="https://github.com/k-lt/svc.products"><img alt="read more" src="m2.svg" align="absmiddle"></a>

### Search
`svc.search` – <a href="https://github.com/k-lt/svc.search"><img alt="read more" src="m2.svg" align="absmiddle"></a>

### Tasks
`svc.tasks` – <a href="https://github.com/k-lt/svc.tasks"><img alt="read more" src="m2.svg" align="absmiddle"></a>

### Workspaces
`svc.workspaces` – <a href="https://github.com/k-lt/svc.workspaces"><img alt="read more" src="m2.svg" align="absmiddle"></a>

### Workforce
`svc.workforce` – <a href="https://github.com/k-lt/svc.workforce"><img alt="read more" src="m2.svg" align="absmiddle"></a>

### Integration services:


<details>

<summary>Integration services</summary>


### Linear
`svc.int-linear` – <a href="https://github.com/k-lt/svc.int-linear"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### GitHub
`svc.int-github` – <a href="https://github.com/k-lt/svc.int-github"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### Google Workspace
`svc.int-google-workspace` – <a href="https://github.com/k-lt/svc.int-google-workspace"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### Notion
`svc.int-notion` – <a href="https://github.com/k-lt/svc.int-notion"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.

### Salesforce
`svc.int-salesforce` – <a href="https://github.com/k-lt/svc.int-salesforce"><img alt="read more" src="m2.svg" align="absmiddle"></a>

Publishes source-aligned events using [@pkg.channels](https://github.com/k-lt/pkg.channels) to a channel. Projects back whatever it should project back.


</details>

⁰¹²³⁴⁵⁶⁷⁸⁹