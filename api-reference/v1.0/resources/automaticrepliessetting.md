---
title: Ressourcentyp automaticRepliesSetting
description: 'Konfigurationseinstellungen automatisch benachrichtigt den Absender einer eingehenden e-Mail mit einer Nachricht aus der '
localization_priority: Normal
ms.openlocfilehash: 81fb16a9124c60f43887150917f132579aa4f163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821406"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="ab938-103">Ressourcentyp automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="ab938-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="ab938-p101">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer. Beispiel: eine automatische Antwort, die darüber informiert, dass der angemeldete Benutzer zur Beantwortung von E-Mails nicht verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="ab938-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="ab938-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ab938-106">Properties</span></span>
| <span data-ttu-id="ab938-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ab938-107">Property</span></span>     | <span data-ttu-id="ab938-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ab938-108">Type</span></span>   |<span data-ttu-id="ab938-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab938-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab938-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="ab938-110">externalAudience</span></span>|<span data-ttu-id="ab938-111">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="ab938-111">externalAudienceScope</span></span>| <span data-ttu-id="ab938-112">Der Satz von außerhalb des angemeldeten Benutzers Unternehmens Benutzergruppe, die **ExternalReplyMessage**erhält, wenn **Status** `AlwaysEnabled` oder `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="ab938-112">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> <span data-ttu-id="ab938-113">Die möglichen Werte sind: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="ab938-113">The possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="ab938-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="ab938-114">externalReplyMessage</span></span>|<span data-ttu-id="ab938-115">string</span><span class="sxs-lookup"><span data-stu-id="ab938-115">string</span></span>|<span data-ttu-id="ab938-116">Die automatische Antwort an die angegebene externe Zielgruppe, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.</span><span class="sxs-lookup"><span data-stu-id="ab938-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="ab938-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="ab938-117">internalReplyMessage</span></span>|<span data-ttu-id="ab938-118">string</span><span class="sxs-lookup"><span data-stu-id="ab938-118">string</span></span>|<span data-ttu-id="ab938-119">Die automatische Antwort an die interne Zielgruppe in der Organisation des angemeldeten Benutzers, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.</span><span class="sxs-lookup"><span data-stu-id="ab938-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="ab938-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="ab938-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="ab938-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ab938-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="ab938-122">Datum und Uhrzeit, die zum Beenden der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="ab938-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="ab938-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="ab938-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="ab938-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ab938-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="ab938-125">Datum und Uhrzeit, die für den Beginn der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="ab938-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="ab938-126">status</span><span class="sxs-lookup"><span data-stu-id="ab938-126">status</span></span>|<span data-ttu-id="ab938-127">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="ab938-127">automaticRepliesStatus</span></span>|<span data-ttu-id="ab938-128">Status der Konfigurationen für automatische Antworten.</span><span class="sxs-lookup"><span data-stu-id="ab938-128">Configurations status for automatic replies.</span></span> <span data-ttu-id="ab938-129">Die möglichen Werte sind: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="ab938-129">The possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab938-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ab938-130">JSON representation</span></span>

<span data-ttu-id="ab938-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ab938-131">Here is a JSON representation of the resource.</span></span>

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
