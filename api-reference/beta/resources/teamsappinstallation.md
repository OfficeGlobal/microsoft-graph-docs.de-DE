---
title: Ressourcentyp teamsAppInstallation
description: 'Eine TeamsApp in einem Team installiert. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 5eca63cb3385fa03f8dffadff0482dc79a1dcfe3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871512"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="751db-103">Ressourcentyp teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="751db-103">teamsAppInstallation resource type</span></span>

> <span data-ttu-id="751db-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="751db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="751db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="751db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="751db-106">Eine [TeamsApp](teamsapp.md) in einem [Team](team.md)installiert.</span><span class="sxs-lookup"><span data-stu-id="751db-106">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="751db-107">Alle Bots, die Teil der app sind wird in jedem Team aufgenommen, die, denen die app hinzugefügt wird.</span><span class="sxs-lookup"><span data-stu-id="751db-107">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="751db-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="751db-108">Methods</span></span>

| <span data-ttu-id="751db-109">Methode</span><span class="sxs-lookup"><span data-stu-id="751db-109">Method</span></span>       | <span data-ttu-id="751db-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="751db-110">Return Type</span></span>  |<span data-ttu-id="751db-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="751db-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="751db-112">Liste apps</span><span class="sxs-lookup"><span data-stu-id="751db-112">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="751db-113">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="751db-113">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="751db-114">Listet die apps in einem Team installiert.</span><span class="sxs-lookup"><span data-stu-id="751db-114">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="751db-115">Hinzufügen der app</span><span class="sxs-lookup"><span data-stu-id="751db-115">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="751db-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="751db-116">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="751db-117">Fügt (installiert) einer app zu einem Team.</span><span class="sxs-lookup"><span data-stu-id="751db-117">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="751db-118">Entfernen der app</span><span class="sxs-lookup"><span data-stu-id="751db-118">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="751db-119">Keine</span><span class="sxs-lookup"><span data-stu-id="751db-119">None</span></span> | <span data-ttu-id="751db-120">Entfernt (deinstalliert) einer app aus einem Team.</span><span class="sxs-lookup"><span data-stu-id="751db-120">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="751db-121">Aktualisieren der app</span><span class="sxs-lookup"><span data-stu-id="751db-121">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="751db-122">Keine</span><span class="sxs-lookup"><span data-stu-id="751db-122">None</span></span> | <span data-ttu-id="751db-123">Upgrades auf die neueste Version der app.</span><span class="sxs-lookup"><span data-stu-id="751db-123">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="751db-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="751db-124">Properties</span></span>

| <span data-ttu-id="751db-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="751db-125">Property</span></span>            | <span data-ttu-id="751db-126">Typ</span><span class="sxs-lookup"><span data-stu-id="751db-126">Type</span></span>     | <span data-ttu-id="751db-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="751db-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="751db-128">id</span><span class="sxs-lookup"><span data-stu-id="751db-128">id</span></span>                  | <span data-ttu-id="751db-129">string</span><span class="sxs-lookup"><span data-stu-id="751db-129">string</span></span>   | <span data-ttu-id="751db-130">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="751db-130">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="751db-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="751db-131">Relationships</span></span>

| <span data-ttu-id="751db-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="751db-132">Relationship</span></span>   | <span data-ttu-id="751db-133">Typ</span><span class="sxs-lookup"><span data-stu-id="751db-133">Type</span></span>    | <span data-ttu-id="751db-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="751db-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="751db-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="751db-135">teamsApp</span></span>|[<span data-ttu-id="751db-136">teamsApp</span><span class="sxs-lookup"><span data-stu-id="751db-136">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="751db-137">Die app, die installiert ist.</span><span class="sxs-lookup"><span data-stu-id="751db-137">The app that is installed.</span></span> |
|<span data-ttu-id="751db-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="751db-138">teamsAppDefinition</span></span>|[<span data-ttu-id="751db-139">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="751db-139">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="751db-140">Die Details dieser Version der app.</span><span class="sxs-lookup"><span data-stu-id="751db-140">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="751db-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="751db-141">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="751db-142">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="751db-142">See also</span></span>

- [<span data-ttu-id="751db-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="751db-143">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="751db-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="751db-144">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="751db-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="751db-145">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

