# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="2471b-101">Ressourcentyp teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="2471b-101">teamGuestSettings resource type</span></span>



<span data-ttu-id="2471b-102">Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im [Team](team.md)können.</span><span class="sxs-lookup"><span data-stu-id="2471b-102">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2471b-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2471b-103">Properties</span></span>
| <span data-ttu-id="2471b-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2471b-104">Property</span></span>     | <span data-ttu-id="2471b-105">Typ</span><span class="sxs-lookup"><span data-stu-id="2471b-105">Type</span></span>   |<span data-ttu-id="2471b-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2471b-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2471b-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="2471b-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="2471b-108">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2471b-108">Boolean</span></span>|<span data-ttu-id="2471b-109">Wenn Festlegung auf "true" Gäste hinzufügen und Kanäle aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="2471b-109">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="2471b-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="2471b-110">allowDeleteChannels</span></span>|<span data-ttu-id="2471b-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2471b-111">Boolean</span></span>|<span data-ttu-id="2471b-112">Bei Festlegung auf "true" Gäste Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="2471b-112">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2471b-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2471b-113">JSON representation</span></span>

<span data-ttu-id="2471b-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2471b-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
