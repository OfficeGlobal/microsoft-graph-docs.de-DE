# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="9101c-101">Ressourcentyp TeamsTabConfiguration (Open Type)</span><span class="sxs-lookup"><span data-stu-id="9101c-101">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="9101c-102">Die Einstellungen, die den Inhalt einer [Registerkarte](teamstab.md)bestimmen. Wenn eine Registerkarte interaktiv konfiguriert ist, wird diese Informationen von der Registerkarte Anbieter-Anwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="9101c-102">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="9101c-103">Abgesehen von den Eigenschaften geben Anwendungsbeispiele Anbieter Registerkarte zusätzliche benutzerdefinierte Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="9101c-103">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="9101c-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9101c-104">Properties</span></span>

|<span data-ttu-id="9101c-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9101c-105">Property</span></span>|<span data-ttu-id="9101c-106">Typ</span><span class="sxs-lookup"><span data-stu-id="9101c-106">Type</span></span>|<span data-ttu-id="9101c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9101c-107">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="9101c-108">%EntityID</span><span class="sxs-lookup"><span data-stu-id="9101c-108">entityId</span></span>   |   <span data-ttu-id="9101c-109">string</span><span class="sxs-lookup"><span data-stu-id="9101c-109">string</span></span> |  <span data-ttu-id="9101c-110">Der Bezeichner für die Entität, die von der Registerkarte Anbieter gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="9101c-110">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="9101c-111">contentUrl</span><span class="sxs-lookup"><span data-stu-id="9101c-111">contentUrl</span></span> |   <span data-ttu-id="9101c-112">string</span><span class="sxs-lookup"><span data-stu-id="9101c-112">string</span></span> |  <span data-ttu-id="9101c-113">URL für das rendering von Inhalt in Teams Registerkarten verwendet.</span><span class="sxs-lookup"><span data-stu-id="9101c-113">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="9101c-114">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9101c-114">Required.</span></span>    |
|  <span data-ttu-id="9101c-115">removeUrl</span><span class="sxs-lookup"><span data-stu-id="9101c-115">removeUrl</span></span>  |   <span data-ttu-id="9101c-116">string</span><span class="sxs-lookup"><span data-stu-id="9101c-116">string</span></span> |  <span data-ttu-id="9101c-117">URL von Teams Client aufgerufen, wenn eine Registerkarte mithilfe des Teams Clients entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="9101c-117">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="9101c-118">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="9101c-118">websiteUrl</span></span> |   <span data-ttu-id="9101c-119">string</span><span class="sxs-lookup"><span data-stu-id="9101c-119">string</span></span> |  <span data-ttu-id="9101c-120">URL für die Anzeige der Registerkarte Inhalt außerhalb von Teams.</span><span class="sxs-lookup"><span data-stu-id="9101c-120">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="9101c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9101c-121">JSON representation</span></span>

<span data-ttu-id="9101c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9101c-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
