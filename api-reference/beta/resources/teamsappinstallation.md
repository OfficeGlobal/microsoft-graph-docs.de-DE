---
title: Ressourcentyp teamsAppInstallation
description: 'Eine TeamsApp in einem Team installiert. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4cf14c36fc0ab0b33f88d4b330e76957e65164a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512836"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="9848f-103">Ressourcentyp teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="9848f-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9848f-104">Eine [TeamsApp](teamsapp.md) in einem [Team](team.md)installiert.</span><span class="sxs-lookup"><span data-stu-id="9848f-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="9848f-105">Alle Bots, die Teil der app sind wird in jedem Team aufgenommen, die, denen die app hinzugefügt wird.</span><span class="sxs-lookup"><span data-stu-id="9848f-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="9848f-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="9848f-106">Methods</span></span>

| <span data-ttu-id="9848f-107">Methode</span><span class="sxs-lookup"><span data-stu-id="9848f-107">Method</span></span>       | <span data-ttu-id="9848f-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9848f-108">Return Type</span></span>  |<span data-ttu-id="9848f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9848f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9848f-110">Liste apps</span><span class="sxs-lookup"><span data-stu-id="9848f-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="9848f-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="9848f-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="9848f-112">Listet die apps in einem Team installiert.</span><span class="sxs-lookup"><span data-stu-id="9848f-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="9848f-113">Hinzufügen der app</span><span class="sxs-lookup"><span data-stu-id="9848f-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="9848f-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="9848f-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="9848f-115">Fügt (installiert) einer app zu einem Team.</span><span class="sxs-lookup"><span data-stu-id="9848f-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="9848f-116">Entfernen der app</span><span class="sxs-lookup"><span data-stu-id="9848f-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="9848f-117">Keine</span><span class="sxs-lookup"><span data-stu-id="9848f-117">None</span></span> | <span data-ttu-id="9848f-118">Entfernt (deinstalliert) einer app aus einem Team.</span><span class="sxs-lookup"><span data-stu-id="9848f-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="9848f-119">Aktualisieren der app</span><span class="sxs-lookup"><span data-stu-id="9848f-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="9848f-120">Keine</span><span class="sxs-lookup"><span data-stu-id="9848f-120">None</span></span> | <span data-ttu-id="9848f-121">Upgrades auf die neueste Version der app.</span><span class="sxs-lookup"><span data-stu-id="9848f-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="9848f-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9848f-122">Properties</span></span>

| <span data-ttu-id="9848f-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9848f-123">Property</span></span>            | <span data-ttu-id="9848f-124">Typ</span><span class="sxs-lookup"><span data-stu-id="9848f-124">Type</span></span>     | <span data-ttu-id="9848f-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9848f-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="9848f-126">id</span><span class="sxs-lookup"><span data-stu-id="9848f-126">id</span></span>                  | <span data-ttu-id="9848f-127">string</span><span class="sxs-lookup"><span data-stu-id="9848f-127">string</span></span>   | <span data-ttu-id="9848f-128">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="9848f-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="9848f-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9848f-129">Relationships</span></span>

| <span data-ttu-id="9848f-130">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9848f-130">Relationship</span></span>   | <span data-ttu-id="9848f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9848f-131">Type</span></span>    | <span data-ttu-id="9848f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9848f-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9848f-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9848f-133">teamsApp</span></span>|[<span data-ttu-id="9848f-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9848f-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="9848f-135">Die app, die installiert ist.</span><span class="sxs-lookup"><span data-stu-id="9848f-135">The app that is installed.</span></span> |
|<span data-ttu-id="9848f-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="9848f-136">teamsAppDefinition</span></span>|[<span data-ttu-id="9848f-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="9848f-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="9848f-138">Die Details dieser Version der app.</span><span class="sxs-lookup"><span data-stu-id="9848f-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9848f-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9848f-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="9848f-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9848f-140">See also</span></span>

- [<span data-ttu-id="9848f-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9848f-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="9848f-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="9848f-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="9848f-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9848f-143">teamsTab</span></span>](../resources/teamstab.md)


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

