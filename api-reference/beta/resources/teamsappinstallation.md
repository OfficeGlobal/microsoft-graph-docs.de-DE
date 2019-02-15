---
title: teamsAppInstallation-Ressourcentyp
description: 'Ein teamsApp, das in einem Team installiert ist. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f6ff72ab99d20eba9880630248e4b61fca5c2521
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057015"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="2502d-103">teamsAppInstallation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2502d-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2502d-104">Ein [teamsApp](teamsapp.md) , das in einem [Team](team.md)installiert ist.</span><span class="sxs-lookup"><span data-stu-id="2502d-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="2502d-105">Alle Bots, die Teil der APP sind, werden Teil eines Teams, dem die app hinzugefügt wird.</span><span class="sxs-lookup"><span data-stu-id="2502d-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="2502d-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="2502d-106">Methods</span></span>

| <span data-ttu-id="2502d-107">Methode</span><span class="sxs-lookup"><span data-stu-id="2502d-107">Method</span></span>       | <span data-ttu-id="2502d-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2502d-108">Return Type</span></span>  |<span data-ttu-id="2502d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2502d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2502d-110">Apps aufListen</span><span class="sxs-lookup"><span data-stu-id="2502d-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="2502d-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2502d-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="2502d-112">Listet die in einem Team installierten apps auf.</span><span class="sxs-lookup"><span data-stu-id="2502d-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="2502d-113">App hinzufügen</span><span class="sxs-lookup"><span data-stu-id="2502d-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="2502d-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2502d-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="2502d-115">Hinzufügen (Installieren) einer App zu einem Team.</span><span class="sxs-lookup"><span data-stu-id="2502d-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="2502d-116">App entfernen</span><span class="sxs-lookup"><span data-stu-id="2502d-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="2502d-117">Keine</span><span class="sxs-lookup"><span data-stu-id="2502d-117">None</span></span> | <span data-ttu-id="2502d-118">Entfernt (deinstalliert) eine APP aus einem Team.</span><span class="sxs-lookup"><span data-stu-id="2502d-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="2502d-119">APP aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2502d-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="2502d-120">Keine</span><span class="sxs-lookup"><span data-stu-id="2502d-120">None</span></span> | <span data-ttu-id="2502d-121">Upgrades auf die neueste Version der app.</span><span class="sxs-lookup"><span data-stu-id="2502d-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="2502d-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2502d-122">Properties</span></span>

| <span data-ttu-id="2502d-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2502d-123">Property</span></span>            | <span data-ttu-id="2502d-124">Typ</span><span class="sxs-lookup"><span data-stu-id="2502d-124">Type</span></span>     | <span data-ttu-id="2502d-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2502d-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="2502d-126">id</span><span class="sxs-lookup"><span data-stu-id="2502d-126">id</span></span>                  | <span data-ttu-id="2502d-127">string</span><span class="sxs-lookup"><span data-stu-id="2502d-127">string</span></span>   | <span data-ttu-id="2502d-128">Eine eindeutige ID (nicht die Teams-Kennung).</span><span class="sxs-lookup"><span data-stu-id="2502d-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="2502d-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2502d-129">Relationships</span></span>

| <span data-ttu-id="2502d-130">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2502d-130">Relationship</span></span>   | <span data-ttu-id="2502d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2502d-131">Type</span></span>    | <span data-ttu-id="2502d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2502d-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2502d-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2502d-133">teamsApp</span></span>|[<span data-ttu-id="2502d-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2502d-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="2502d-135">Die installierte app.</span><span class="sxs-lookup"><span data-stu-id="2502d-135">The app that is installed.</span></span> |
|<span data-ttu-id="2502d-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2502d-136">teamsAppDefinition</span></span>|[<span data-ttu-id="2502d-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2502d-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="2502d-138">Die Details dieser Version der app.</span><span class="sxs-lookup"><span data-stu-id="2502d-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2502d-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2502d-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="2502d-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2502d-140">See also</span></span>

- [<span data-ttu-id="2502d-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2502d-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="2502d-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2502d-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="2502d-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2502d-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

