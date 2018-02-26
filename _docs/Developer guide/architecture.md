---
title: Platform architecture
category: Developer guide
order: 1
---

![Oasis UI and Platform architecture](/images/oasis_architecture_tiers.jpg)

| **Component** | **Description** | **Technology** |
| Oasis UI | Browser based application for managing exposure data and operating modelling workflows | R Shiny, ShinyProxy |
|Oasis | UI API Services for interacting with exposure and output data | Flask |
|Oasis UI Database | Storage for exposure data, workflow configurations and system data. | SQL Server |
|Oasis API | Services for uploading Oasis files, running analyses and retrieving outputs. | Flask, Celery |
|Message Queue | Queues for managing workload across multiple calculation back ends. | Rabbit MQ |
|Data store | Storage for transient analysis data. | File share |
|Keys Server | Model specific services for generating area peril and vulnerability keys for a particular set of exposures. | Flask, Python |
|Analysis Worker | Executes a model. | Celery, running as daemon, ktools, model data |
