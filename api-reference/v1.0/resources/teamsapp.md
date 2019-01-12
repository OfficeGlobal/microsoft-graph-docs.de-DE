---
title: Ressourcentyp teamsApp
description: Eine app in den Microsoft-Teams, app-Katalog.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2493b7f6adee51e5c5622585055cbd3cf2778656
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937446"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="0a878-103">Ressourcentyp teamsApp</span><span class="sxs-lookup"><span data-stu-id="0a878-103">teamsApp resource type</span></span>



<span data-ttu-id="0a878-104">Eine app in den [Microsoft-Teams,](teams-api-overview.md) app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="0a878-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="0a878-105">Benutzer können diese apps im Microsoft-Teams Store anzeigen, und diese apps in [Teams](team.md) mithilfe der [Add-app an das Team](../api/teamsappinstallation-add.md) -Methode installiert werden können.</span><span class="sxs-lookup"><span data-stu-id="0a878-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="0a878-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="0a878-106">Methods</span></span>

| <span data-ttu-id="0a878-107">Methode</span><span class="sxs-lookup"><span data-stu-id="0a878-107">Method</span></span>       | <span data-ttu-id="0a878-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0a878-108">Return Type</span></span>  |<span data-ttu-id="0a878-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a878-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a878-110">Liste der veröffentlichten apps</span><span class="sxs-lookup"><span data-stu-id="0a878-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="0a878-111">[TeamsApp](teamsapp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0a878-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="0a878-112">Veröffentlichte apps aus dem Microsoft-Teams, apps Katalog aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="0a878-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="0a878-113">Veröffentlichen einer app</span><span class="sxs-lookup"><span data-stu-id="0a878-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="0a878-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0a878-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="0a878-115">Veröffentlichen einer app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="0a878-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="0a878-116">Aktualisieren einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a878-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="0a878-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0a878-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="0a878-118">Aktualisieren einer veröffentlichten-app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="0a878-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="0a878-119">Entfernen einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a878-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="0a878-120">Keine</span><span class="sxs-lookup"><span data-stu-id="0a878-120">None</span></span> | <span data-ttu-id="0a878-121">Entfernen Sie eine veröffentlichte app aus Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="0a878-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="0a878-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a878-122">Properties</span></span>

| <span data-ttu-id="0a878-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a878-123">Property</span></span>            | <span data-ttu-id="0a878-124">Typ</span><span class="sxs-lookup"><span data-stu-id="0a878-124">Type</span></span>     | <span data-ttu-id="0a878-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a878-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="0a878-126">id</span><span class="sxs-lookup"><span data-stu-id="0a878-126">id</span></span>                  | <span data-ttu-id="0a878-127">string</span><span class="sxs-lookup"><span data-stu-id="0a878-127">string</span></span>   | <span data-ttu-id="0a878-128">Der app Katalog generierte app-ID (andere Entwickler bereitgestellter ID in der [Microsoft-Teams, Zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="0a878-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="0a878-129">externalId</span><span class="sxs-lookup"><span data-stu-id="0a878-129">externalId</span></span>          | <span data-ttu-id="0a878-130">string</span><span class="sxs-lookup"><span data-stu-id="0a878-130">string</span></span>   | <span data-ttu-id="0a878-131">Die ID des Katalogs von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="0a878-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="0a878-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0a878-132">displayName</span></span>                | <span data-ttu-id="0a878-133">string</span><span class="sxs-lookup"><span data-stu-id="0a878-133">string</span></span>   | <span data-ttu-id="0a878-134">Der Name der Katalog app von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="0a878-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="0a878-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="0a878-135">distributionMethod</span></span>  | <span data-ttu-id="0a878-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="0a878-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="0a878-137">Die Methode der Verteilung für die app.</span><span class="sxs-lookup"><span data-stu-id="0a878-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="0a878-138">TeamsAppDistributionMethod Werte</span><span class="sxs-lookup"><span data-stu-id="0a878-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="0a878-139">Element</span><span class="sxs-lookup"><span data-stu-id="0a878-139">Member</span></span>|<span data-ttu-id="0a878-140">Wert</span><span class="sxs-lookup"><span data-stu-id="0a878-140">Value</span></span>|<span data-ttu-id="0a878-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a878-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a878-142">Speichern</span><span class="sxs-lookup"><span data-stu-id="0a878-142">store</span></span>|<span data-ttu-id="0a878-143">0</span><span class="sxs-lookup"><span data-stu-id="0a878-143">0</span></span>| <span data-ttu-id="0a878-144">Die app ist für alle Mandanten über Microsoft-Teams app Store verfügbar.</span><span class="sxs-lookup"><span data-stu-id="0a878-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="0a878-145">Organisation</span><span class="sxs-lookup"><span data-stu-id="0a878-145">organization</span></span>|<span data-ttu-id="0a878-146">1</span><span class="sxs-lookup"><span data-stu-id="0a878-146">1</span></span>|<span data-ttu-id="0a878-147">Die app ist nur in diesen Mandanten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="0a878-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="0a878-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="0a878-148">sideloaded</span></span>|<span data-ttu-id="0a878-149">2</span><span class="sxs-lookup"><span data-stu-id="0a878-149">2</span></span>|<span data-ttu-id="0a878-150">Die app steht nur für die Benutzer/Team seine installierten an.</span><span class="sxs-lookup"><span data-stu-id="0a878-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a878-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0a878-151">Relationships</span></span>

| <span data-ttu-id="0a878-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0a878-152">Relationship</span></span> | <span data-ttu-id="0a878-153">Typ</span><span class="sxs-lookup"><span data-stu-id="0a878-153">Type</span></span>   | <span data-ttu-id="0a878-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a878-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0a878-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="0a878-155">appDefinitions</span></span>|<span data-ttu-id="0a878-156">[TeamsAppDefinition](teamsappdefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0a878-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="0a878-157">Die Details für jede Version der app.</span><span class="sxs-lookup"><span data-stu-id="0a878-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0a878-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0a878-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="0a878-159">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0a878-159">See also</span></span>

- [<span data-ttu-id="0a878-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="0a878-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="0a878-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0a878-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="0a878-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0a878-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

