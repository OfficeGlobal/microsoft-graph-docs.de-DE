---
title: Ressourcentyp automaticRepliesSetting
description: 'Konfigurationseinstellungen automatisch benachrichtigt den Absender einer eingehenden e-Mail mit einer Nachricht aus der '
localization_priority: Normal
ms.openlocfilehash: 5ff16aa93042e0d66063cb62de7a8dcdf870c892
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641253"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="05cdb-103">Ressourcentyp automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="05cdb-103">automaticRepliesSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05cdb-p101">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer. Beispiel: eine automatische Antwort, die darüber informiert, dass der angemeldete Benutzer zur Beantwortung von E-Mails nicht verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="05cdb-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="05cdb-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="05cdb-106">Properties</span></span>
| <span data-ttu-id="05cdb-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="05cdb-107">Property</span></span>     | <span data-ttu-id="05cdb-108">Typ</span><span class="sxs-lookup"><span data-stu-id="05cdb-108">Type</span></span>   |<span data-ttu-id="05cdb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="05cdb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05cdb-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="05cdb-110">externalAudience</span></span>|<span data-ttu-id="05cdb-111">String</span><span class="sxs-lookup"><span data-stu-id="05cdb-111">String</span></span>| <span data-ttu-id="05cdb-p102">Die Zielgruppe außerhalb der Organisation des angemeldeten Benutzers, der **ExternalReplyMessage** erhält, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist. Mögliche Werte: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="05cdb-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="05cdb-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="05cdb-114">externalReplyMessage</span></span>|<span data-ttu-id="05cdb-115">string</span><span class="sxs-lookup"><span data-stu-id="05cdb-115">string</span></span>|<span data-ttu-id="05cdb-116">Die automatische Antwort an die angegebene externe Zielgruppe, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.</span><span class="sxs-lookup"><span data-stu-id="05cdb-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="05cdb-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="05cdb-117">internalReplyMessage</span></span>|<span data-ttu-id="05cdb-118">string</span><span class="sxs-lookup"><span data-stu-id="05cdb-118">string</span></span>|<span data-ttu-id="05cdb-119">Die automatische Antwort an die interne Zielgruppe in der Organisation des angemeldeten Benutzers, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.</span><span class="sxs-lookup"><span data-stu-id="05cdb-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="05cdb-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="05cdb-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="05cdb-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="05cdb-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="05cdb-122">Datum und Uhrzeit, die zum Beenden der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="05cdb-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="05cdb-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="05cdb-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="05cdb-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="05cdb-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="05cdb-125">Datum und Uhrzeit, die für den Beginn der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="05cdb-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="05cdb-126">status</span><span class="sxs-lookup"><span data-stu-id="05cdb-126">status</span></span>|<span data-ttu-id="05cdb-127">String</span><span class="sxs-lookup"><span data-stu-id="05cdb-127">String</span></span>|<span data-ttu-id="05cdb-p103">Konfigurationensstatus für automatische Antworten. Mögliche Werte: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="05cdb-p103">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05cdb-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="05cdb-130">JSON representation</span></span>

<span data-ttu-id="05cdb-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="05cdb-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliessetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
