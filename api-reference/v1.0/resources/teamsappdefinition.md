# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="696fb-101">Ressourcentyp teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="696fb-101">teamsAppDefinition resource type</span></span>



<span data-ttu-id="696fb-102">Die Details einer Version von einer [TeamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="696fb-102">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="696fb-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="696fb-103">Properties</span></span>

| <span data-ttu-id="696fb-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="696fb-104">Property</span></span>            | <span data-ttu-id="696fb-105">Typ</span><span class="sxs-lookup"><span data-stu-id="696fb-105">Type</span></span>     | <span data-ttu-id="696fb-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="696fb-106">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="696fb-107">id</span><span class="sxs-lookup"><span data-stu-id="696fb-107">id</span></span>                  | <span data-ttu-id="696fb-108">string</span><span class="sxs-lookup"><span data-stu-id="696fb-108">string</span></span>   | <span data-ttu-id="696fb-109">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="696fb-109">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="696fb-110">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="696fb-110">teamsAppId</span></span>          | <span data-ttu-id="696fb-111">string</span><span class="sxs-lookup"><span data-stu-id="696fb-111">string</span></span>   | <span data-ttu-id="696fb-112">Die Id von Teams App-Manifest.</span><span class="sxs-lookup"><span data-stu-id="696fb-112">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="696fb-113">displayName</span><span class="sxs-lookup"><span data-stu-id="696fb-113">displayName</span></span>         | <span data-ttu-id="696fb-114">string</span><span class="sxs-lookup"><span data-stu-id="696fb-114">string</span></span>   | <span data-ttu-id="696fb-115">Der Name der app bereitgestellt von der app-Entwickler.</span><span class="sxs-lookup"><span data-stu-id="696fb-115">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="696fb-116">Version</span><span class="sxs-lookup"><span data-stu-id="696fb-116">version</span></span>             | <span data-ttu-id="696fb-117">string</span><span class="sxs-lookup"><span data-stu-id="696fb-117">string</span></span>   | <span data-ttu-id="696fb-118">Die Versionsnummer der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="696fb-118">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="696fb-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="696fb-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="696fb-120">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="696fb-120">See also</span></span>

- [<span data-ttu-id="696fb-121">teamsApp</span><span class="sxs-lookup"><span data-stu-id="696fb-121">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="696fb-122">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="696fb-122">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="696fb-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="696fb-123">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

