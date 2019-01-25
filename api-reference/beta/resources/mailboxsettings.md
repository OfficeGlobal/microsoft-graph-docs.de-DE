---
title: mailboxSettings-Ressourcentyp
description: Einstellungen für das primäre Postfach des angemeldeten Benutzers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 599447ff1006fcfa5b17cc320777b49f36576ad5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518653"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="667b9-103">mailboxSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="667b9-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="667b9-104">Einstellungen für das primäre Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="667b9-104">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="667b9-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="667b9-105">Properties</span></span>
| <span data-ttu-id="667b9-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="667b9-106">Property</span></span>     | <span data-ttu-id="667b9-107">Typ</span><span class="sxs-lookup"><span data-stu-id="667b9-107">Type</span></span>   |<span data-ttu-id="667b9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="667b9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="667b9-109">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="667b9-109">archiveFolder</span></span>|<span data-ttu-id="667b9-110">string</span><span class="sxs-lookup"><span data-stu-id="667b9-110">string</span></span>|<span data-ttu-id="667b9-111">Ordner-ID eines Archivordners für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="667b9-111">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="667b9-112">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="667b9-112">automaticRepliesSetting</span></span>|[<span data-ttu-id="667b9-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="667b9-113">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="667b9-114">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="667b9-114">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="667b9-115">language</span><span class="sxs-lookup"><span data-stu-id="667b9-115">language</span></span>|[<span data-ttu-id="667b9-116">localeInfo</span><span class="sxs-lookup"><span data-stu-id="667b9-116">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="667b9-117">Die Gebietsschemainformationen des Benutzers, einschließlich der bevorzugten Sprache und Land/Region.</span><span class="sxs-lookup"><span data-stu-id="667b9-117">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="667b9-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="667b9-118">timeZone</span></span>|<span data-ttu-id="667b9-119">string</span><span class="sxs-lookup"><span data-stu-id="667b9-119">string</span></span>|<span data-ttu-id="667b9-120">Die Standardzeitzone für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="667b9-120">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="667b9-121">workingHours</span><span class="sxs-lookup"><span data-stu-id="667b9-121">workingHours</span></span>|[<span data-ttu-id="667b9-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="667b9-122">workingHours</span></span>](workinghours.md)|<span data-ttu-id="667b9-123">Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="667b9-123">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="667b9-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="667b9-124">JSON representation</span></span>

<span data-ttu-id="667b9-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="667b9-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailboxsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
