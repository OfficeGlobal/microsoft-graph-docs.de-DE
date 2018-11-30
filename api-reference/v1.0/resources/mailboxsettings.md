---
title: mailboxSettings-Ressourcentyp
description: Einstellungen für das primäre Postfach des angemeldeten Benutzers.
ms.openlocfilehash: b8fb2c1f11f849a4633d6be4f4519b85b33923ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019218"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="b06fb-103">mailboxSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b06fb-103">mailboxSettings resource type</span></span>

<span data-ttu-id="b06fb-104">Einstellungen für das primäre Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b06fb-104">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="b06fb-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b06fb-105">Properties</span></span>
| <span data-ttu-id="b06fb-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b06fb-106">Property</span></span>     | <span data-ttu-id="b06fb-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b06fb-107">Type</span></span>   |<span data-ttu-id="b06fb-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b06fb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b06fb-109">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="b06fb-109">archiveFolder</span></span>|<span data-ttu-id="b06fb-110">string</span><span class="sxs-lookup"><span data-stu-id="b06fb-110">string</span></span>|<span data-ttu-id="b06fb-111">Ordner-ID eines Archivordners für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="b06fb-111">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="b06fb-112">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b06fb-112">automaticRepliesSetting</span></span>|[<span data-ttu-id="b06fb-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b06fb-113">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="b06fb-114">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="b06fb-114">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="b06fb-115">language</span><span class="sxs-lookup"><span data-stu-id="b06fb-115">language</span></span>|[<span data-ttu-id="b06fb-116">localeInfo</span><span class="sxs-lookup"><span data-stu-id="b06fb-116">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="b06fb-117">Die Gebietsschemainformationen des Benutzers, einschließlich der bevorzugten Sprache und Land/Region.</span><span class="sxs-lookup"><span data-stu-id="b06fb-117">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="b06fb-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="b06fb-118">timeZone</span></span>|<span data-ttu-id="b06fb-119">string</span><span class="sxs-lookup"><span data-stu-id="b06fb-119">string</span></span>|<span data-ttu-id="b06fb-120">Die Standardzeitzone für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b06fb-120">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="b06fb-121">workingHours</span><span class="sxs-lookup"><span data-stu-id="b06fb-121">workingHours</span></span>|[<span data-ttu-id="b06fb-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="b06fb-122">workingHours</span></span>](workinghours.md)|<span data-ttu-id="b06fb-123">Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="b06fb-123">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b06fb-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b06fb-124">JSON representation</span></span>

<span data-ttu-id="b06fb-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b06fb-125">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->