---
title: Ressourcentyp teamsApp
description: Eine app in den Microsoft-Teams, app-Katalog.
author: nkramer
ms.openlocfilehash: 207974800e44e0db29b8c42f260a1ac16a18902f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359584"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="41e93-103">Ressourcentyp teamsApp</span><span class="sxs-lookup"><span data-stu-id="41e93-103">teamsApp resource type</span></span>



<span data-ttu-id="41e93-104">Eine app in den [Microsoft-Teams,](teams-api-overview.md) app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="41e93-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="41e93-105">Benutzer können diese apps im Microsoft-Teams Store anzeigen, und diese apps in [Teams](team.md) mithilfe der [Add-app an das Team](../api/teamsappinstallation-add.md) -Methode installiert werden können.</span><span class="sxs-lookup"><span data-stu-id="41e93-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="41e93-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="41e93-106">Methods</span></span>

| <span data-ttu-id="41e93-107">Methode</span><span class="sxs-lookup"><span data-stu-id="41e93-107">Method</span></span>       | <span data-ttu-id="41e93-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="41e93-108">Return Type</span></span>  |<span data-ttu-id="41e93-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41e93-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41e93-110">Liste der veröffentlichten apps</span><span class="sxs-lookup"><span data-stu-id="41e93-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="41e93-111">[TeamsApp](teamsapp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="41e93-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="41e93-112">Veröffentlichte apps aus dem Microsoft-Teams, apps Katalog aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="41e93-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="41e93-113">Veröffentlichen einer app</span><span class="sxs-lookup"><span data-stu-id="41e93-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="41e93-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="41e93-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="41e93-115">Veröffentlichen einer app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="41e93-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="41e93-116">Aktualisieren einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="41e93-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="41e93-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="41e93-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="41e93-118">Aktualisieren einer veröffentlichten-app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="41e93-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="41e93-119">Entfernen einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="41e93-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="41e93-120">Keines</span><span class="sxs-lookup"><span data-stu-id="41e93-120">None</span></span> | <span data-ttu-id="41e93-121">Entfernen Sie eine veröffentlichte app aus Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="41e93-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="41e93-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="41e93-122">Properties</span></span>

| <span data-ttu-id="41e93-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41e93-123">Property</span></span>            | <span data-ttu-id="41e93-124">Typ</span><span class="sxs-lookup"><span data-stu-id="41e93-124">Type</span></span>     | <span data-ttu-id="41e93-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41e93-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="41e93-126">id</span><span class="sxs-lookup"><span data-stu-id="41e93-126">id</span></span>                  | <span data-ttu-id="41e93-127">string</span><span class="sxs-lookup"><span data-stu-id="41e93-127">string</span></span>   | <span data-ttu-id="41e93-128">Der app Katalog generierte app-ID (andere Entwickler bereitgestellter ID in der [Microsoft-Teams, Zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="41e93-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="41e93-129">externalId</span><span class="sxs-lookup"><span data-stu-id="41e93-129">externalId</span></span>          | <span data-ttu-id="41e93-130">string</span><span class="sxs-lookup"><span data-stu-id="41e93-130">string</span></span>   | <span data-ttu-id="41e93-131">Die ID des Katalogs von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="41e93-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="41e93-132">displayName</span><span class="sxs-lookup"><span data-stu-id="41e93-132">displayName</span></span>                | <span data-ttu-id="41e93-133">string</span><span class="sxs-lookup"><span data-stu-id="41e93-133">string</span></span>   | <span data-ttu-id="41e93-134">Der Name der Katalog app von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="41e93-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="41e93-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="41e93-135">distributionMethod</span></span>  | <span data-ttu-id="41e93-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="41e93-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="41e93-137">Die Methode der Verteilung für die app.</span><span class="sxs-lookup"><span data-stu-id="41e93-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="41e93-138">TeamsAppDistributionMethod Werte</span><span class="sxs-lookup"><span data-stu-id="41e93-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="41e93-139">Member</span><span class="sxs-lookup"><span data-stu-id="41e93-139">Member</span></span>|<span data-ttu-id="41e93-140">Wert</span><span class="sxs-lookup"><span data-stu-id="41e93-140">Value</span></span>|<span data-ttu-id="41e93-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41e93-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41e93-142">Speichern</span><span class="sxs-lookup"><span data-stu-id="41e93-142">store</span></span>|<span data-ttu-id="41e93-143">0</span><span class="sxs-lookup"><span data-stu-id="41e93-143">0</span></span>| <span data-ttu-id="41e93-144">Die app ist für alle Mandanten über Microsoft-Teams app Store verfügbar.</span><span class="sxs-lookup"><span data-stu-id="41e93-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="41e93-145">Organisation</span><span class="sxs-lookup"><span data-stu-id="41e93-145">organization</span></span>|<span data-ttu-id="41e93-146">1</span><span class="sxs-lookup"><span data-stu-id="41e93-146">1</span></span>|<span data-ttu-id="41e93-147">Die app ist nur in diesen Mandanten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="41e93-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="41e93-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="41e93-148">sideloaded</span></span>|<span data-ttu-id="41e93-149">2</span><span class="sxs-lookup"><span data-stu-id="41e93-149">2</span></span>|<span data-ttu-id="41e93-150">Die app steht nur für die Benutzer/Team seine installierten an.</span><span class="sxs-lookup"><span data-stu-id="41e93-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41e93-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="41e93-151">Relationships</span></span>

| <span data-ttu-id="41e93-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="41e93-152">Relationship</span></span> | <span data-ttu-id="41e93-153">Typ</span><span class="sxs-lookup"><span data-stu-id="41e93-153">Type</span></span>   | <span data-ttu-id="41e93-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41e93-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="41e93-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="41e93-155">appDefinitions</span></span>|<span data-ttu-id="41e93-156">[TeamsAppDefinition](teamsappdefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="41e93-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="41e93-157">Die Details für jede Version der app.</span><span class="sxs-lookup"><span data-stu-id="41e93-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41e93-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="41e93-158">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a><span data-ttu-id="41e93-159">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="41e93-159">See also</span></span>

- [<span data-ttu-id="41e93-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="41e93-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="41e93-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="41e93-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="41e93-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="41e93-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

