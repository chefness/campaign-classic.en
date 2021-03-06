---
solution: Campaign Classic
product: campaign
title: Event collection
description: Event collection
audience: message-center
content-type: reference
topic-tags: event-processing
---

# Event collection{#event-collection}

Events generated by the information system can be collected using two modes:

* Calls to SOAP methods let you push events in Adobe Campaign: the PushEvent method lets you send one event at a time, the PushEvents method lets you send several at once. Refer to [Event description](../../message-center/using/event-description.md).
* Creating a workflow lets you recover events by importing files or via an SQL gateway (with the **Federated Data Access** option).

Once they are collected, events are broken down - by technical workflows - between real time and batch queues of the execution instances, while waiting to be linked to a message template.

![](assets/messagecenter_events_queues_001.png)

>[!NOTE]
>
>On the execution instances, the **[!UICONTROL Real time events]** or **[!UICONTROL Batch events]** folders must not be set as views, as this could lead to [access right](../../platform/using/access-management.md#about-permissions) issues. For more on setting a folder as a view, see [About views](../../platform/using/access-management.md#about-views).
