# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="81a29-101">Ressourcentyp teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="81a29-101">teamsAppInstallation resource type</span></span>



<span data-ttu-id="81a29-102">Eine [TeamsApp](teamsapp.md) in einem [Team](team.md)installiert.</span><span class="sxs-lookup"><span data-stu-id="81a29-102">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="81a29-103">Alle Bots, die Teil der app sind wird in jedem Team aufgenommen, die, denen die app hinzugefügt wird.</span><span class="sxs-lookup"><span data-stu-id="81a29-103">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="81a29-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="81a29-104">Methods</span></span>

| <span data-ttu-id="81a29-105">Methode</span><span class="sxs-lookup"><span data-stu-id="81a29-105">Method</span></span>       | <span data-ttu-id="81a29-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="81a29-106">Return Type</span></span>  |<span data-ttu-id="81a29-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81a29-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81a29-108">Liste apps</span><span class="sxs-lookup"><span data-stu-id="81a29-108">List apps</span></span>](../api/teamsappinstallation_list.md) | [<span data-ttu-id="81a29-109">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="81a29-109">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="81a29-110">Listet die apps in einem Team installiert.</span><span class="sxs-lookup"><span data-stu-id="81a29-110">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="81a29-111">Hinzufügen der app</span><span class="sxs-lookup"><span data-stu-id="81a29-111">Add app</span></span>](../api/teamsappinstallation_add.md) | [<span data-ttu-id="81a29-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="81a29-112">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="81a29-113">Fügt (installiert) einer app zu einem Team.</span><span class="sxs-lookup"><span data-stu-id="81a29-113">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="81a29-114">Entfernen der app</span><span class="sxs-lookup"><span data-stu-id="81a29-114">Remove app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="81a29-115">Keine</span><span class="sxs-lookup"><span data-stu-id="81a29-115">None</span></span> | <span data-ttu-id="81a29-116">Entfernt (deinstalliert) einer app aus einem Team.</span><span class="sxs-lookup"><span data-stu-id="81a29-116">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="81a29-117">Aktualisieren der app</span><span class="sxs-lookup"><span data-stu-id="81a29-117">Upgrade app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="81a29-118">Keine</span><span class="sxs-lookup"><span data-stu-id="81a29-118">None</span></span> | <span data-ttu-id="81a29-119">Upgrades auf die neueste Version der app.</span><span class="sxs-lookup"><span data-stu-id="81a29-119">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="81a29-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81a29-120">Properties</span></span>

| <span data-ttu-id="81a29-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81a29-121">Property</span></span>            | <span data-ttu-id="81a29-122">Typ</span><span class="sxs-lookup"><span data-stu-id="81a29-122">Type</span></span>     | <span data-ttu-id="81a29-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81a29-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="81a29-124">id</span><span class="sxs-lookup"><span data-stu-id="81a29-124">id</span></span>                  | <span data-ttu-id="81a29-125">string</span><span class="sxs-lookup"><span data-stu-id="81a29-125">string</span></span>   | <span data-ttu-id="81a29-126">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="81a29-126">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="81a29-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="81a29-127">Relationships</span></span>

| <span data-ttu-id="81a29-128">Beziehung</span><span class="sxs-lookup"><span data-stu-id="81a29-128">Relationship</span></span>   | <span data-ttu-id="81a29-129">Typ</span><span class="sxs-lookup"><span data-stu-id="81a29-129">Type</span></span>    | <span data-ttu-id="81a29-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81a29-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="81a29-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="81a29-131">teamsApp</span></span>|[<span data-ttu-id="81a29-132">teamsApp</span><span class="sxs-lookup"><span data-stu-id="81a29-132">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="81a29-133">Die app, die installiert ist.</span><span class="sxs-lookup"><span data-stu-id="81a29-133">The app that is installed.</span></span> |
|<span data-ttu-id="81a29-134">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="81a29-134">teamsAppDefinition</span></span>|[<span data-ttu-id="81a29-135">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="81a29-135">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="81a29-136">Die Details dieser Version der app.</span><span class="sxs-lookup"><span data-stu-id="81a29-136">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81a29-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81a29-137">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="81a29-138">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="81a29-138">See also</span></span>

- [<span data-ttu-id="81a29-139">teamsApp</span><span class="sxs-lookup"><span data-stu-id="81a29-139">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="81a29-140">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="81a29-140">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="81a29-141">teamsTab</span><span class="sxs-lookup"><span data-stu-id="81a29-141">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

