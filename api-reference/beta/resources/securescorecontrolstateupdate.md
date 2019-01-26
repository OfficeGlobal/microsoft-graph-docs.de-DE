---
title: " Ressourcentyp secureScoreControlStateUpdate"
description: Diese Ressource enthält Verlauf von Zustände des Steuerelements durch Benutzer aktualisiert (Steuerelementzustände gehören Standard, ignoriert, ThirdParty, überprüft).
localization_priority: Normal
ms.openlocfilehash: 4e626f67579e3dc35fe36f5dcc67b1512c5e7bbc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574390"
---
 ##  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="5a7f6-103">Ressourcentyp secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="5a7f6-103">secureScoreControlStateUpdate resource type</span></span>

> <span data-ttu-id="5a7f6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5a7f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a7f6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5a7f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a7f6-106">Enthält den Verlauf der vom Benutzer aktualisiert Steuerelementzustände (Steuerelementzustände gehören Standard, ignoriert, ThirdParty, überprüft).</span><span class="sxs-lookup"><span data-stu-id="5a7f6-106">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="5a7f6-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a7f6-107">Property</span></span>         | <span data-ttu-id="5a7f6-108">Typ</span><span class="sxs-lookup"><span data-stu-id="5a7f6-108">Type</span></span>           |<span data-ttu-id="5a7f6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a7f6-109">Description</span></span>                                                  |
|:----------------|:---------------|:------------------------------------------------------------|
| <span data-ttu-id="5a7f6-110">assignedTo</span><span class="sxs-lookup"><span data-stu-id="5a7f6-110">assignedTo</span></span>      | <span data-ttu-id="5a7f6-111">string</span><span class="sxs-lookup"><span data-stu-id="5a7f6-111">string</span></span>         | <span data-ttu-id="5a7f6-112">Weisen Sie das Steuerelement dem Benutzer, die die Aktion</span><span class="sxs-lookup"><span data-stu-id="5a7f6-112">Assign the control to the user who will take the action</span></span>     |
| <span data-ttu-id="5a7f6-113">Kommentar</span><span class="sxs-lookup"><span data-stu-id="5a7f6-113">comment</span></span>         | <span data-ttu-id="5a7f6-114">string</span><span class="sxs-lookup"><span data-stu-id="5a7f6-114">string</span></span>         | <span data-ttu-id="5a7f6-115">Enthält Informationen zum Steuerelement optionalen Kommentar</span><span class="sxs-lookup"><span data-stu-id="5a7f6-115">Provides optional comment about the control</span></span>                 |
| <span data-ttu-id="5a7f6-116">state</span><span class="sxs-lookup"><span data-stu-id="5a7f6-116">state</span></span>           | <span data-ttu-id="5a7f6-117">string</span><span class="sxs-lookup"><span data-stu-id="5a7f6-117">string</span></span>         | <span data-ttu-id="5a7f6-118">Zustand des Steuerelements mit PATCH-Befehl geändert werden kann (Ex: ignoriert, ThirdParty usw.)</span><span class="sxs-lookup"><span data-stu-id="5a7f6-118">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
| <span data-ttu-id="5a7f6-119">updatedBy</span><span class="sxs-lookup"><span data-stu-id="5a7f6-119">updatedBy</span></span>       | <span data-ttu-id="5a7f6-120">string</span><span class="sxs-lookup"><span data-stu-id="5a7f6-120">string</span></span>         |<span data-ttu-id="5a7f6-121">ID des Benutzers, der Mandant Status aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7f6-121">ID of the user who updated tenant state</span></span>                      |
| <span data-ttu-id="5a7f6-122">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a7f6-122">updatedDateTime</span></span> | <span data-ttu-id="5a7f6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a7f6-123">DateTimeOffset</span></span> |<span data-ttu-id="5a7f6-124">Uhrzeit, an welches Steuerelement Zustand aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="5a7f6-124">Time at which control state was updated</span></span>                      |
 

## <a name="json-representation"></a><span data-ttu-id="5a7f6-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5a7f6-125">JSON representation</span></span>
 <span data-ttu-id="5a7f6-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5a7f6-126">The following is a JSON representation of the resource.</span></span>

 <!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "DateTimeOffset"
}
```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
