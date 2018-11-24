# <a name="teammembersettings-resource-type"></a><span data-ttu-id="ede3f-101">Ressourcentyp teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="ede3f-101">teamMemberSettings resource type</span></span>



<span data-ttu-id="ede3f-102">Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="ede3f-102">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ede3f-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ede3f-103">Properties</span></span>
| <span data-ttu-id="ede3f-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ede3f-104">Property</span></span>     | <span data-ttu-id="ede3f-105">Typ</span><span class="sxs-lookup"><span data-stu-id="ede3f-105">Type</span></span>   |<span data-ttu-id="ede3f-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ede3f-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ede3f-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="ede3f-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="ede3f-108">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ede3f-108">Boolean</span></span>|<span data-ttu-id="ede3f-109">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen und Aktualisieren von Kanäle kann.</span><span class="sxs-lookup"><span data-stu-id="ede3f-109">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="ede3f-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="ede3f-110">allowDeleteChannels</span></span>|<span data-ttu-id="ede3f-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ede3f-111">Boolean</span></span>|<span data-ttu-id="ede3f-112">Bei Festlegung auf "true" Mitglieder Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="ede3f-112">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="ede3f-113">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="ede3f-113">allowAddRemoveApps</span></span>|<span data-ttu-id="ede3f-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ede3f-114">Boolean</span></span>|<span data-ttu-id="ede3f-115">Wenn es sich bei Festlegung auf "true" Mitglieder hinzufügen und Entfernen von apps.</span><span class="sxs-lookup"><span data-stu-id="ede3f-115">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="ede3f-116">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="ede3f-116">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="ede3f-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ede3f-117">Boolean</span></span>|<span data-ttu-id="ede3f-118">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Registerkarten.</span><span class="sxs-lookup"><span data-stu-id="ede3f-118">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="ede3f-119">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="ede3f-119">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="ede3f-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ede3f-120">Boolean</span></span>|<span data-ttu-id="ede3f-121">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Connectors.</span><span class="sxs-lookup"><span data-stu-id="ede3f-121">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ede3f-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ede3f-122">JSON representation</span></span>

<span data-ttu-id="ede3f-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ede3f-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
