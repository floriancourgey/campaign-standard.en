---
title: Union on two refined audiences
description: This use case shows the union of two Read audience activities.
page-status-flag: never-activated
uuid: 58c54e71-f4a7-4ae9-80a3-33c379ab1db9
contentOwner: sauviat
products: SG_CAMPAIGN/STANDARD
audience: automating
content-type: reference
topic-tags: targeting-activities
discoiquuid: 674684e5-8830-4d2f-ba97-59ed4ba7422f
context-tags: readAudience,main
internal: n
snippet: y
---

# Union on two refined audiences {#example--union-on-two-refined-audiences}

The workflow defined in this example shows the union of two **[!UICONTROL Read audience]** activities. The goal of this workflow is to send an email to Gold or Silver members that are between 18 and 30 years old. Specific audiences are already created in the system to keep track of Gold and Silver members.

The workflow is designed as follows:

![](assets/readaudience_activity_example1.png)

* A first [Read audience](../../automating/using/read-audience.md) activity that retrieves the Gold members audience and refines it by selecting only profiles that are between 18 and 30 years old.
* A second **[!UICONTROL Read audience]** activity that retrieves the Silver members audience and refines it by selecting only profiles that are between 18 and 30 years old.
* A [Union](../../automating/using/union.md) activity that unites populations from both **[!UICONTROL Read audiences]** activities into one final population.
* An [Email delivery](../../automating/using/email-delivery.md) activity that sends the email to the population coming from the **[!UICONTROL Union]** activity.