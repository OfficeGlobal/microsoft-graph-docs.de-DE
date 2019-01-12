---
title: Ressourcentyp teamsAppInstallation
description: 'Eine TeamsApp in einem Team installiert. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 30a7f05d7b814fbb36c632a88f2f4e71f135d781
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955345"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="47374-103">Ressourcentyp teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="47374-103">teamsAppInstallation resource type</span></span>

> <span data-ttu-id="47374-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="47374-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47374-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="47374-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47374-106">Eine [TeamsApp](teamsapp.md) in einem [Team](team.md)installiert.</span><span class="sxs-lookup"><span data-stu-id="47374-106">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="47374-107">Alle Bots, die Teil der app sind wird in jedem Team aufgenommen, die, denen die app hinzugefügt wird.</span><span class="sxs-lookup"><span data-stu-id="47374-107">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="47374-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="47374-108">Methods</span></span>

| <span data-ttu-id="47374-109">Methode</span><span class="sxs-lookup"><span data-stu-id="47374-109">Method</span></span>       | <span data-ttu-id="47374-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="47374-110">Return Type</span></span>  |<span data-ttu-id="47374-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47374-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="47374-112">Liste apps</span><span class="sxs-lookup"><span data-stu-id="47374-112">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="47374-113">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="47374-113">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="47374-114">Listet die apps in einem Team installiert.</span><span class="sxs-lookup"><span data-stu-id="47374-114">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="47374-115">Hinzufügen der app</span><span class="sxs-lookup"><span data-stu-id="47374-115">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="47374-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="47374-116">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="47374-117">Fügt (installiert) einer app zu einem Team.</span><span class="sxs-lookup"><span data-stu-id="47374-117">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="47374-118">Entfernen der app</span><span class="sxs-lookup"><span data-stu-id="47374-118">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="47374-119">Keine</span><span class="sxs-lookup"><span data-stu-id="47374-119">None</span></span> | <span data-ttu-id="47374-120">Entfernt (deinstalliert) einer app aus einem Team.</span><span class="sxs-lookup"><span data-stu-id="47374-120">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="47374-121">Aktualisieren der app</span><span class="sxs-lookup"><span data-stu-id="47374-121">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="47374-122">Keine</span><span class="sxs-lookup"><span data-stu-id="47374-122">None</span></span> | <span data-ttu-id="47374-123">Upgrades auf die neueste Version der app.</span><span class="sxs-lookup"><span data-stu-id="47374-123">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="47374-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="47374-124">Properties</span></span>

| <span data-ttu-id="47374-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="47374-125">Property</span></span>            | <span data-ttu-id="47374-126">Typ</span><span class="sxs-lookup"><span data-stu-id="47374-126">Type</span></span>     | <span data-ttu-id="47374-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47374-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="47374-128">id</span><span class="sxs-lookup"><span data-stu-id="47374-128">id</span></span>                  | <span data-ttu-id="47374-129">string</span><span class="sxs-lookup"><span data-stu-id="47374-129">string</span></span>   | <span data-ttu-id="47374-130">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="47374-130">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="47374-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="47374-131">Relationships</span></span>

| <span data-ttu-id="47374-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="47374-132">Relationship</span></span>   | <span data-ttu-id="47374-133">Typ</span><span class="sxs-lookup"><span data-stu-id="47374-133">Type</span></span>    | <span data-ttu-id="47374-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47374-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="47374-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="47374-135">teamsApp</span></span>|[<span data-ttu-id="47374-136">teamsApp</span><span class="sxs-lookup"><span data-stu-id="47374-136">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="47374-137">Die app, die installiert ist.</span><span class="sxs-lookup"><span data-stu-id="47374-137">The app that is installed.</span></span> |
|<span data-ttu-id="47374-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="47374-138">teamsAppDefinition</span></span>|[<span data-ttu-id="47374-139">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="47374-139">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="47374-140">Die Details dieser Version der app.</span><span class="sxs-lookup"><span data-stu-id="47374-140">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="47374-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="47374-141">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="47374-142">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="47374-142">See also</span></span>

- [<span data-ttu-id="47374-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="47374-143">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="47374-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="47374-144">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="47374-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="47374-145">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

