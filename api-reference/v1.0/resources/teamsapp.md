# <a name="teamsapp-resource-type"></a><span data-ttu-id="1ecf2-101">Ressourcentyp teamsApp</span><span class="sxs-lookup"><span data-stu-id="1ecf2-101">teamsApp resource type</span></span>



<span data-ttu-id="1ecf2-102">Eine app in den [Microsoft-Teams,](teams_api_overview.md) app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-102">An app in the [Microsoft Teams](teams_api_overview.md) app catalog.</span></span>

<span data-ttu-id="1ecf2-103">Benutzer können diese apps im Microsoft-Teams Store anzeigen, und diese apps in [Teams](team.md) mithilfe der [Add-app an das Team](../api/teamsappinstallation_add.md) -Methode installiert werden können.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-103">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation_add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="1ecf2-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="1ecf2-104">Methods</span></span>

| <span data-ttu-id="1ecf2-105">Methode</span><span class="sxs-lookup"><span data-stu-id="1ecf2-105">Method</span></span>       | <span data-ttu-id="1ecf2-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1ecf2-106">Return Type</span></span>  |<span data-ttu-id="1ecf2-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ecf2-108">Liste der veröffentlichten apps</span><span class="sxs-lookup"><span data-stu-id="1ecf2-108">List published apps</span></span>](../api/teamsapp_list.md) | <span data-ttu-id="1ecf2-109">[TeamsApp](teamsApp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-109">[teamsApp](teamsApp.md) collection</span></span> | <span data-ttu-id="1ecf2-110">Veröffentlichte apps aus dem Microsoft-Teams, apps Katalog aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-110">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="1ecf2-111">Veröffentlichen einer app</span><span class="sxs-lookup"><span data-stu-id="1ecf2-111">Publish an app</span></span>](../api/teamsapp_publish.md) | [<span data-ttu-id="1ecf2-112">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1ecf2-112">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="1ecf2-113">Veröffentlichen einer app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-113">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="1ecf2-114">Aktualisieren einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-114">Update a published app</span></span>](../api/teamsapp_update.md) | [<span data-ttu-id="1ecf2-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1ecf2-115">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="1ecf2-116">Aktualisieren einer veröffentlichten-app in Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-116">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="1ecf2-117">Entfernen einer veröffentlichten Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-117">Remove a published app</span></span>](../api/teamsapp_delete.md) | <span data-ttu-id="1ecf2-118">Keine</span><span class="sxs-lookup"><span data-stu-id="1ecf2-118">None</span></span> | <span data-ttu-id="1ecf2-119">Entfernen Sie eine veröffentlichte app aus Ihrer Organisation app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-119">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ecf2-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1ecf2-120">Properties</span></span>

| <span data-ttu-id="1ecf2-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ecf2-121">Property</span></span>            | <span data-ttu-id="1ecf2-122">Typ</span><span class="sxs-lookup"><span data-stu-id="1ecf2-122">Type</span></span>     | <span data-ttu-id="1ecf2-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1ecf2-124">id</span><span class="sxs-lookup"><span data-stu-id="1ecf2-124">id</span></span>                  | <span data-ttu-id="1ecf2-125">string</span><span class="sxs-lookup"><span data-stu-id="1ecf2-125">string</span></span>   | <span data-ttu-id="1ecf2-126">Der app Katalog generierte app-ID (andere Entwickler bereitgestellter ID in der [Microsoft-Teams, Zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="1ecf2-126">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="1ecf2-127">externalId</span><span class="sxs-lookup"><span data-stu-id="1ecf2-127">externalId</span></span>          | <span data-ttu-id="1ecf2-128">string</span><span class="sxs-lookup"><span data-stu-id="1ecf2-128">string</span></span>   | <span data-ttu-id="1ecf2-129">Die ID des Katalogs von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-129">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="1ecf2-130">displayName</span><span class="sxs-lookup"><span data-stu-id="1ecf2-130">displayName</span></span>                | <span data-ttu-id="1ecf2-131">string</span><span class="sxs-lookup"><span data-stu-id="1ecf2-131">string</span></span>   | <span data-ttu-id="1ecf2-132">Der Name der Katalog app von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-132">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="1ecf2-133">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="1ecf2-133">distributionMethod</span></span>  | <span data-ttu-id="1ecf2-134">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="1ecf2-134">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="1ecf2-135">Die Methode der Verteilung für die app.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-135">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="1ecf2-136">TeamsAppDistributionMethod Werte</span><span class="sxs-lookup"><span data-stu-id="1ecf2-136">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="1ecf2-137">Element</span><span class="sxs-lookup"><span data-stu-id="1ecf2-137">Member</span></span>|<span data-ttu-id="1ecf2-138">Wert</span><span class="sxs-lookup"><span data-stu-id="1ecf2-138">Value</span></span>|<span data-ttu-id="1ecf2-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ecf2-140">Speichern</span><span class="sxs-lookup"><span data-stu-id="1ecf2-140">store</span></span>|<span data-ttu-id="1ecf2-141">0</span><span class="sxs-lookup"><span data-stu-id="1ecf2-141">0</span></span>| <span data-ttu-id="1ecf2-142">Die app ist für alle Mandanten über Microsoft-Teams app Store verfügbar.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-142">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="1ecf2-143">Organisation</span><span class="sxs-lookup"><span data-stu-id="1ecf2-143">organization</span></span>|<span data-ttu-id="1ecf2-144">1</span><span class="sxs-lookup"><span data-stu-id="1ecf2-144">1</span></span>|<span data-ttu-id="1ecf2-145">Die app ist nur in diesen Mandanten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-145">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="1ecf2-146">sideloaded</span><span class="sxs-lookup"><span data-stu-id="1ecf2-146">sideloaded</span></span>|<span data-ttu-id="1ecf2-147">2</span><span class="sxs-lookup"><span data-stu-id="1ecf2-147">2</span></span>|<span data-ttu-id="1ecf2-148">Die app steht nur für die Benutzer/Team seine installierten an.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-148">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ecf2-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1ecf2-149">Relationships</span></span>

| <span data-ttu-id="1ecf2-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-150">Relationship</span></span> | <span data-ttu-id="1ecf2-151">Typ</span><span class="sxs-lookup"><span data-stu-id="1ecf2-151">Type</span></span>   | <span data-ttu-id="1ecf2-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1ecf2-153">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="1ecf2-153">appDefinitions</span></span>|<span data-ttu-id="1ecf2-154">[TeamsAppDefinition](teamsappdefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-154">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="1ecf2-155">Die Details für jede Version der app.</span><span class="sxs-lookup"><span data-stu-id="1ecf2-155">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1ecf2-156">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1ecf2-156">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="1ecf2-157">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="1ecf2-157">See also</span></span>

- [<span data-ttu-id="1ecf2-158">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1ecf2-158">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="1ecf2-159">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1ecf2-159">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="1ecf2-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1ecf2-160">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

