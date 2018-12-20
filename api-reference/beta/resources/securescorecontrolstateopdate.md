---
title: " Ressourcentyp secureScoreControlStateUpdate"
description: Diese Ressource enthält Verlauf von Zustände des Steuerelements durch Benutzer aktualisiert (Steuerelementzustände gehören Standard, ignoriert, ThirdParty, überprüft).
ms.openlocfilehash: ba98f2fc85f3f8e12355f9acf5d232599a7f29f7
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380966"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="079b2-103">Ressourcentyp secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="079b2-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="079b2-104">Enthält den Verlauf der vom Benutzer aktualisiert Steuerelementzustände (Steuerelementzustände gehören Standard, ignoriert, ThirdParty, überprüft).</span><span class="sxs-lookup"><span data-stu-id="079b2-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="079b2-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="079b2-105">Property</span></span> |<span data-ttu-id="079b2-106">Typ</span><span class="sxs-lookup"><span data-stu-id="079b2-106">Type</span></span> |<span data-ttu-id="079b2-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="079b2-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="079b2-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="079b2-108">assignedTo</span></span> | <span data-ttu-id="079b2-109">string</span><span class="sxs-lookup"><span data-stu-id="079b2-109">string</span></span> | <span data-ttu-id="079b2-110">Weisen Sie das Steuerelement dem Benutzer, die die Aktion</span><span class="sxs-lookup"><span data-stu-id="079b2-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="079b2-111">Kommentar</span><span class="sxs-lookup"><span data-stu-id="079b2-111">comment</span></span> | <span data-ttu-id="079b2-112">string</span><span class="sxs-lookup"><span data-stu-id="079b2-112">string</span></span> | <span data-ttu-id="079b2-113">Enthält Informationen zum Steuerelement optionalen Kommentar</span><span class="sxs-lookup"><span data-stu-id="079b2-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="079b2-114">state</span><span class="sxs-lookup"><span data-stu-id="079b2-114">state</span></span> | <span data-ttu-id="079b2-115">string</span><span class="sxs-lookup"><span data-stu-id="079b2-115">string</span></span> | <span data-ttu-id="079b2-116">Zustand des Steuerelements mit PATCH-Befehl geändert werden kann (Ex: ignoriert, ThirdParty usw.)</span><span class="sxs-lookup"><span data-stu-id="079b2-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="079b2-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="079b2-117">updatedBy</span></span> | <span data-ttu-id="079b2-118">string</span><span class="sxs-lookup"><span data-stu-id="079b2-118">string</span></span> |<span data-ttu-id="079b2-119">ID des Benutzers, der Mandant Status aktualisiert</span><span class="sxs-lookup"><span data-stu-id="079b2-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="079b2-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="079b2-120">updatedDateTime</span></span> | <span data-ttu-id="079b2-121">DateTimeOffset?</span><span class="sxs-lookup"><span data-stu-id="079b2-121">DateTimeOffset?</span></span> |<span data-ttu-id="079b2-122">Uhrzeit, an welches Steuerelement Zustand aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="079b2-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="079b2-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="079b2-123">JSON representation</span></span>
 <span data-ttu-id="079b2-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="079b2-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->