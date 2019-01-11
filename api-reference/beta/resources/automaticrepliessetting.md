---
title: Ressourcentyp automaticRepliesSetting
description: 'Konfigurationseinstellungen automatisch benachrichtigt den Absender einer eingehenden e-Mail mit einer Nachricht aus der '
localization_priority: Normal
ms.openlocfilehash: 0160197a4fafe10b7f78be9124da3b6260bfcee6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820657"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="61a57-103">Ressourcentyp automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="61a57-103">automaticRepliesSetting resource type</span></span>

> <span data-ttu-id="61a57-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="61a57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61a57-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61a57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61a57-p102">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer. Beispiel: eine automatische Antwort, die darüber informiert, dass der angemeldete Benutzer zur Beantwortung von E-Mails nicht verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="61a57-p102">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="61a57-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61a57-108">Properties</span></span>
| <span data-ttu-id="61a57-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61a57-109">Property</span></span>     | <span data-ttu-id="61a57-110">Typ</span><span class="sxs-lookup"><span data-stu-id="61a57-110">Type</span></span>   |<span data-ttu-id="61a57-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61a57-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61a57-112">externalAudience</span><span class="sxs-lookup"><span data-stu-id="61a57-112">externalAudience</span></span>|<span data-ttu-id="61a57-113">String</span><span class="sxs-lookup"><span data-stu-id="61a57-113">String</span></span>| <span data-ttu-id="61a57-p103">Die Zielgruppe außerhalb der Organisation des angemeldeten Benutzers, der **ExternalReplyMessage** erhält, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist. Mögliche Werte: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="61a57-p103">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="61a57-116">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="61a57-116">externalReplyMessage</span></span>|<span data-ttu-id="61a57-117">string</span><span class="sxs-lookup"><span data-stu-id="61a57-117">string</span></span>|<span data-ttu-id="61a57-118">Die automatische Antwort an die angegebene externe Zielgruppe, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.</span><span class="sxs-lookup"><span data-stu-id="61a57-118">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="61a57-119">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="61a57-119">internalReplyMessage</span></span>|<span data-ttu-id="61a57-120">string</span><span class="sxs-lookup"><span data-stu-id="61a57-120">string</span></span>|<span data-ttu-id="61a57-121">Die automatische Antwort an die interne Zielgruppe in der Organisation des angemeldeten Benutzers, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.</span><span class="sxs-lookup"><span data-stu-id="61a57-121">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="61a57-122">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="61a57-122">scheduledEndDateTime</span></span>|[<span data-ttu-id="61a57-123">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="61a57-123">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="61a57-124">Datum und Uhrzeit, die zum Beenden der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="61a57-124">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="61a57-125">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="61a57-125">scheduledStartDateTime</span></span>|[<span data-ttu-id="61a57-126">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="61a57-126">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="61a57-127">Datum und Uhrzeit, die für den Beginn der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="61a57-127">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="61a57-128">status</span><span class="sxs-lookup"><span data-stu-id="61a57-128">status</span></span>|<span data-ttu-id="61a57-129">String</span><span class="sxs-lookup"><span data-stu-id="61a57-129">String</span></span>|<span data-ttu-id="61a57-p104">Konfigurationensstatus für automatische Antworten. Mögliche Werte: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="61a57-p104">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61a57-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61a57-132">JSON representation</span></span>

<span data-ttu-id="61a57-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61a57-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
