---
title: mailboxSettings-Ressourcentyp
description: Einstellungen für das primäre Postfach des angemeldeten Benutzers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 53ded2d60161d833f70a3b747e0ec35953d5bd39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937082"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="00a3e-103">mailboxSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="00a3e-103">mailboxSettings resource type</span></span>

<span data-ttu-id="00a3e-104">Einstellungen für das primäre Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="00a3e-104">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="00a3e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00a3e-105">Properties</span></span>
| <span data-ttu-id="00a3e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00a3e-106">Property</span></span>     | <span data-ttu-id="00a3e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="00a3e-107">Type</span></span>   |<span data-ttu-id="00a3e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00a3e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00a3e-109">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="00a3e-109">archiveFolder</span></span>|<span data-ttu-id="00a3e-110">string</span><span class="sxs-lookup"><span data-stu-id="00a3e-110">string</span></span>|<span data-ttu-id="00a3e-111">Ordner-ID eines Archivordners für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="00a3e-111">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="00a3e-112">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="00a3e-112">automaticRepliesSetting</span></span>|[<span data-ttu-id="00a3e-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="00a3e-113">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="00a3e-114">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="00a3e-114">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="00a3e-115">language</span><span class="sxs-lookup"><span data-stu-id="00a3e-115">language</span></span>|[<span data-ttu-id="00a3e-116">localeInfo</span><span class="sxs-lookup"><span data-stu-id="00a3e-116">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="00a3e-117">Die Gebietsschemainformationen des Benutzers, einschließlich der bevorzugten Sprache und Land/Region.</span><span class="sxs-lookup"><span data-stu-id="00a3e-117">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="00a3e-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="00a3e-118">timeZone</span></span>|<span data-ttu-id="00a3e-119">string</span><span class="sxs-lookup"><span data-stu-id="00a3e-119">string</span></span>|<span data-ttu-id="00a3e-120">Die Standardzeitzone für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="00a3e-120">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="00a3e-121">workingHours</span><span class="sxs-lookup"><span data-stu-id="00a3e-121">workingHours</span></span>|[<span data-ttu-id="00a3e-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="00a3e-122">workingHours</span></span>](workinghours.md)|<span data-ttu-id="00a3e-123">Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="00a3e-123">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00a3e-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00a3e-124">JSON representation</span></span>

<span data-ttu-id="00a3e-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00a3e-125">Here is a JSON representation of the resource.</span></span>

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
