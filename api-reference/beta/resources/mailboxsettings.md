---
title: mailboxSettings-Ressourcentyp
description: Einstellungen für das primäre Postfach des angemeldeten Benutzers.
ms.openlocfilehash: 79a01c59ec0a891c13107095a950a7cc8ae0b547
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058209"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="cab00-103">mailboxSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cab00-103">mailboxSettings resource type</span></span>

> <span data-ttu-id="cab00-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cab00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cab00-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cab00-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cab00-106">Einstellungen für das primäre Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cab00-106">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="cab00-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cab00-107">Properties</span></span>
| <span data-ttu-id="cab00-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cab00-108">Property</span></span>     | <span data-ttu-id="cab00-109">Typ</span><span class="sxs-lookup"><span data-stu-id="cab00-109">Type</span></span>   |<span data-ttu-id="cab00-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cab00-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cab00-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="cab00-111">archiveFolder</span></span>|<span data-ttu-id="cab00-112">string</span><span class="sxs-lookup"><span data-stu-id="cab00-112">string</span></span>|<span data-ttu-id="cab00-113">Ordner-ID eines Archivordners für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="cab00-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="cab00-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="cab00-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="cab00-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="cab00-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="cab00-116">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="cab00-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="cab00-117">language</span><span class="sxs-lookup"><span data-stu-id="cab00-117">language</span></span>|[<span data-ttu-id="cab00-118">localeInfo</span><span class="sxs-lookup"><span data-stu-id="cab00-118">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="cab00-119">Die Gebietsschemainformationen des Benutzers, einschließlich der bevorzugten Sprache und Land/Region.</span><span class="sxs-lookup"><span data-stu-id="cab00-119">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="cab00-120">timeZone</span><span class="sxs-lookup"><span data-stu-id="cab00-120">timeZone</span></span>|<span data-ttu-id="cab00-121">string</span><span class="sxs-lookup"><span data-stu-id="cab00-121">string</span></span>|<span data-ttu-id="cab00-122">Die Standardzeitzone für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cab00-122">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="cab00-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="cab00-123">workingHours</span></span>|[<span data-ttu-id="cab00-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="cab00-124">workingHours</span></span>](workinghours.md)|<span data-ttu-id="cab00-125">Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="cab00-125">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cab00-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cab00-126">JSON representation</span></span>

<span data-ttu-id="cab00-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cab00-127">Here is a JSON representation of the resource.</span></span>

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