---
title: Ressourcentyp teamsApp
description: Eine app in den Microsoft-Teams, app-Katalog.
author: nkramer
ms.openlocfilehash: b0f3bb42bb90c2c3f0211c5a7092fa7fdb9b10b5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305327"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="2415a-103">Ressourcentyp teamsApp</span><span class="sxs-lookup"><span data-stu-id="2415a-103">teamsApp resource type</span></span>

> <span data-ttu-id="2415a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2415a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2415a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2415a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2415a-106">Eine app in den [Microsoft-Teams,](teams-api-overview.md) app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="2415a-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="2415a-107">Benutzer können diese apps im Microsoft-Teams Store anzeigen, und diese apps in [Teams](team.md) mithilfe der [Add-app an das Team](../api/teamsappinstallation-add.md) -Methode installiert werden können.</span><span class="sxs-lookup"><span data-stu-id="2415a-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="2415a-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="2415a-108">Methods</span></span>

| <span data-ttu-id="2415a-109">Methode</span><span class="sxs-lookup"><span data-stu-id="2415a-109">Method</span></span>       | <span data-ttu-id="2415a-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2415a-110">Return Type</span></span>  |<span data-ttu-id="2415a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2415a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2415a-112">Liste der veröffentlichten apps</span><span class="sxs-lookup"><span data-stu-id="2415a-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="2415a-113">[TeamsApp](teamsapp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="2415a-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="2415a-114">Veröffentlichte apps aus dem Microsoft-Teams, apps Katalog aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="2415a-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="2415a-115">Veröffentlichen einer app</span><span class="sxs-lookup"><span data-stu-id="2415a-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="2415a-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2415a-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="2415a-117">Veröffentlichen einer app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="2415a-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="2415a-118">Aktualisieren einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="2415a-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="2415a-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2415a-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="2415a-120">Aktualisieren einer veröffentlichten-app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="2415a-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="2415a-121">Entfernen einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="2415a-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="2415a-122">Keines</span><span class="sxs-lookup"><span data-stu-id="2415a-122">None</span></span> | <span data-ttu-id="2415a-123">Entfernen Sie eine veröffentlichte app aus Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="2415a-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="2415a-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2415a-124">Properties</span></span>

| <span data-ttu-id="2415a-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2415a-125">Property</span></span>            | <span data-ttu-id="2415a-126">Typ</span><span class="sxs-lookup"><span data-stu-id="2415a-126">Type</span></span>     | <span data-ttu-id="2415a-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2415a-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="2415a-128">id</span><span class="sxs-lookup"><span data-stu-id="2415a-128">id</span></span>                  | <span data-ttu-id="2415a-129">string</span><span class="sxs-lookup"><span data-stu-id="2415a-129">string</span></span>   | <span data-ttu-id="2415a-130">Der app Katalog generierte app-ID (andere Entwickler bereitgestellter ID in der [Microsoft-Teams, Zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="2415a-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="2415a-131">externalId</span><span class="sxs-lookup"><span data-stu-id="2415a-131">externalId</span></span>          | <span data-ttu-id="2415a-132">string</span><span class="sxs-lookup"><span data-stu-id="2415a-132">string</span></span>   | <span data-ttu-id="2415a-133">Die ID des Katalogs von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="2415a-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="2415a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2415a-134">displayName</span></span>                | <span data-ttu-id="2415a-135">string</span><span class="sxs-lookup"><span data-stu-id="2415a-135">string</span></span>   | <span data-ttu-id="2415a-136">Der Name der Katalog app von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="2415a-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="2415a-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="2415a-137">distributionMethod</span></span>  | <span data-ttu-id="2415a-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="2415a-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="2415a-139">Die Methode der Verteilung für die app.</span><span class="sxs-lookup"><span data-stu-id="2415a-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="2415a-140">TeamsAppDistributionMethod Werte</span><span class="sxs-lookup"><span data-stu-id="2415a-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="2415a-141">Member</span><span class="sxs-lookup"><span data-stu-id="2415a-141">Member</span></span>|<span data-ttu-id="2415a-142">Wert</span><span class="sxs-lookup"><span data-stu-id="2415a-142">Value</span></span>|<span data-ttu-id="2415a-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2415a-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2415a-144">Speichern</span><span class="sxs-lookup"><span data-stu-id="2415a-144">store</span></span>|<span data-ttu-id="2415a-145">0</span><span class="sxs-lookup"><span data-stu-id="2415a-145">0</span></span>| <span data-ttu-id="2415a-146">Die app ist für alle Mandanten über Microsoft-Teams app Store verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2415a-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="2415a-147">Organisation</span><span class="sxs-lookup"><span data-stu-id="2415a-147">organization</span></span>|<span data-ttu-id="2415a-148">1</span><span class="sxs-lookup"><span data-stu-id="2415a-148">1</span></span>|<span data-ttu-id="2415a-149">Die app ist nur in diesen Mandanten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2415a-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="2415a-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="2415a-150">sideloaded</span></span>|<span data-ttu-id="2415a-151">2</span><span class="sxs-lookup"><span data-stu-id="2415a-151">2</span></span>|<span data-ttu-id="2415a-152">Die app steht nur für die Benutzer/Team seine installierten an.</span><span class="sxs-lookup"><span data-stu-id="2415a-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2415a-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2415a-153">Relationships</span></span>

| <span data-ttu-id="2415a-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2415a-154">Relationship</span></span> | <span data-ttu-id="2415a-155">Typ</span><span class="sxs-lookup"><span data-stu-id="2415a-155">Type</span></span>   | <span data-ttu-id="2415a-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2415a-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2415a-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="2415a-157">appDefinitions</span></span>|<span data-ttu-id="2415a-158">[TeamsAppDefinition](teamsappdefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="2415a-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="2415a-159">Die Details für jede Version der app.</span><span class="sxs-lookup"><span data-stu-id="2415a-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2415a-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2415a-160">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="2415a-161">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2415a-161">See also</span></span>

- [<span data-ttu-id="2415a-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2415a-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="2415a-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2415a-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="2415a-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2415a-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

