---
title: Ressourcentyp teamsApp
description: Eine app in den Microsoft-Teams, app-Katalog.
ms.openlocfilehash: bb9081306cbcc5d8537c86e7f3f59afff89a03b0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061147"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="cf83c-103">Ressourcentyp teamsApp</span><span class="sxs-lookup"><span data-stu-id="cf83c-103">teamsApp resource type</span></span>

> <span data-ttu-id="cf83c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cf83c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf83c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cf83c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf83c-106">Eine app in den [Microsoft-Teams,](teams-api-overview.md) app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="cf83c-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="cf83c-107">Benutzer können diese apps im Microsoft-Teams Store anzeigen, und diese apps in [Teams](team.md) mithilfe der [Add-app an das Team](../api/teamsappinstallation-add.md) -Methode installiert werden können.</span><span class="sxs-lookup"><span data-stu-id="cf83c-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="cf83c-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="cf83c-108">Methods</span></span>

| <span data-ttu-id="cf83c-109">Methode</span><span class="sxs-lookup"><span data-stu-id="cf83c-109">Method</span></span>       | <span data-ttu-id="cf83c-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cf83c-110">Return Type</span></span>  |<span data-ttu-id="cf83c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf83c-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf83c-112">Liste der veröffentlichten apps</span><span class="sxs-lookup"><span data-stu-id="cf83c-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="cf83c-113">[TeamsApp](teamsapp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="cf83c-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="cf83c-114">Veröffentlichte apps aus dem Microsoft-Teams, apps Katalog aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="cf83c-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="cf83c-115">Veröffentlichen einer app</span><span class="sxs-lookup"><span data-stu-id="cf83c-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="cf83c-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cf83c-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="cf83c-117">Veröffentlichen einer app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="cf83c-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="cf83c-118">Aktualisieren einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf83c-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="cf83c-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cf83c-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="cf83c-120">Aktualisieren einer veröffentlichten-app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="cf83c-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="cf83c-121">Entfernen einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf83c-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="cf83c-122">Keines</span><span class="sxs-lookup"><span data-stu-id="cf83c-122">None</span></span> | <span data-ttu-id="cf83c-123">Entfernen Sie eine veröffentlichte app aus Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="cf83c-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf83c-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cf83c-124">Properties</span></span>

| <span data-ttu-id="cf83c-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cf83c-125">Property</span></span>            | <span data-ttu-id="cf83c-126">Typ</span><span class="sxs-lookup"><span data-stu-id="cf83c-126">Type</span></span>     | <span data-ttu-id="cf83c-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf83c-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="cf83c-128">id</span><span class="sxs-lookup"><span data-stu-id="cf83c-128">id</span></span>                  | <span data-ttu-id="cf83c-129">string</span><span class="sxs-lookup"><span data-stu-id="cf83c-129">string</span></span>   | <span data-ttu-id="cf83c-130">Der app Katalog generierte app-ID (andere Entwickler bereitgestellter ID in der [Microsoft-Teams, Zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="cf83c-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="cf83c-131">externalId</span><span class="sxs-lookup"><span data-stu-id="cf83c-131">externalId</span></span>          | <span data-ttu-id="cf83c-132">string</span><span class="sxs-lookup"><span data-stu-id="cf83c-132">string</span></span>   | <span data-ttu-id="cf83c-133">Die ID des Katalogs von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="cf83c-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="cf83c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cf83c-134">displayName</span></span>                | <span data-ttu-id="cf83c-135">string</span><span class="sxs-lookup"><span data-stu-id="cf83c-135">string</span></span>   | <span data-ttu-id="cf83c-136">Der Name der Katalog app von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="cf83c-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="cf83c-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="cf83c-137">distributionMethod</span></span>  | <span data-ttu-id="cf83c-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="cf83c-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="cf83c-139">Die Methode der Verteilung für die app.</span><span class="sxs-lookup"><span data-stu-id="cf83c-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="cf83c-140">TeamsAppDistributionMethod Werte</span><span class="sxs-lookup"><span data-stu-id="cf83c-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="cf83c-141">Element</span><span class="sxs-lookup"><span data-stu-id="cf83c-141">Member</span></span>|<span data-ttu-id="cf83c-142">Wert</span><span class="sxs-lookup"><span data-stu-id="cf83c-142">Value</span></span>|<span data-ttu-id="cf83c-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf83c-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf83c-144">Speichern</span><span class="sxs-lookup"><span data-stu-id="cf83c-144">store</span></span>|<span data-ttu-id="cf83c-145">0</span><span class="sxs-lookup"><span data-stu-id="cf83c-145">0</span></span>| <span data-ttu-id="cf83c-146">Die app ist für alle Mandanten über Microsoft-Teams app Store verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cf83c-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="cf83c-147">Organisation</span><span class="sxs-lookup"><span data-stu-id="cf83c-147">organization</span></span>|<span data-ttu-id="cf83c-148">1</span><span class="sxs-lookup"><span data-stu-id="cf83c-148">1</span></span>|<span data-ttu-id="cf83c-149">Die app ist nur in diesen Mandanten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cf83c-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="cf83c-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="cf83c-150">sideloaded</span></span>|<span data-ttu-id="cf83c-151">2</span><span class="sxs-lookup"><span data-stu-id="cf83c-151">2</span></span>|<span data-ttu-id="cf83c-152">Die app steht nur für die Benutzer/Team seine installierten an.</span><span class="sxs-lookup"><span data-stu-id="cf83c-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf83c-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cf83c-153">Relationships</span></span>

| <span data-ttu-id="cf83c-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="cf83c-154">Relationship</span></span> | <span data-ttu-id="cf83c-155">Typ</span><span class="sxs-lookup"><span data-stu-id="cf83c-155">Type</span></span>   | <span data-ttu-id="cf83c-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf83c-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cf83c-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="cf83c-157">appDefinitions</span></span>|<span data-ttu-id="cf83c-158">[TeamsAppDefinition](teamsappdefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="cf83c-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="cf83c-159">Die Details für jede Version der app.</span><span class="sxs-lookup"><span data-stu-id="cf83c-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cf83c-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cf83c-160">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="cf83c-161">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="cf83c-161">See also</span></span>

- [<span data-ttu-id="cf83c-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="cf83c-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="cf83c-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="cf83c-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="cf83c-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cf83c-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

