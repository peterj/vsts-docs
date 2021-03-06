---
title: Publish To Azure Service Bus task 
description: Build and release task to send a message to an Azure Service Bus with a build or release pipeline in Azure Pipelines and TFS.
ms.assetid: 81D73795-0171-434F-AE37-5386F4E71915
ms.prod: devops
ms.technology: devops-cicd
ms.topic: reference
ms.manager: douge
ms.author: ahomer
author: alexhomer1
ms.date: 08/24/2018
monikerRange: 'vsts'
---

# Utility: Publish To Azure Service Bus

![icon](_img/publish-to-azure-service-bus.png) Send a message to an Azure Service Bus using a service connection and without using an agent.

## Demands

Can be used in only an [agentless job](../../process/server-phases.md) of a release pipeline.

::: moniker range="> tfs-2018"
## YAML snippet
[!INCLUDE [temp](../_shared/yaml/PublishToAzureServiceBusV1.md)]
::: moniker-end

## Arguments

| Parameter | Comments |
| --- | --- |
| **Display name** | Required. The name to display for this task. |
| **Azure Service Bus Connection** | Required. An existing service connection to an Azure Service Bus. |
| **Message body** | Required. The text of the message body to send to the Service Bus. |
| **Wait for Task Completion** | Optional. Set this option to force the task to halt until a response is received. |
| **Control options** | See [Control options](../../process/tasks.md#controloptions) |

Also see this task on [GitHub](https://github.com/Microsoft/vsts-tasks/tree/master/Tasks/PublishToAzureServiceBusV1).

## Open source

This task is open source [on GitHub](https://github.com/Microsoft/vsts-tasks). Feedback and contributions are welcome.

## Q & A

<!-- BEGINSECTION class="md-qanda" -->

[!INCLUDE [temp](../../_shared/qa-agents.md)]

<!-- ENDSECTION -->
