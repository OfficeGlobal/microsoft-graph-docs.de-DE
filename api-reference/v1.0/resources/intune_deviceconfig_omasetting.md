# <a name="omasetting-resource-type"></a><span data-ttu-id="a05e5-101">omaSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a05e5-101">omaSetting resource type</span></span>

> <span data-ttu-id="a05e5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a05e5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a05e5-103">Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="a05e5-103">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="a05e5-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a05e5-104">Properties</span></span>
|<span data-ttu-id="a05e5-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a05e5-105">Property</span></span>|<span data-ttu-id="a05e5-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a05e5-106">Type</span></span>|<span data-ttu-id="a05e5-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a05e5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a05e5-108">displayName</span><span class="sxs-lookup"><span data-stu-id="a05e5-108">displayName</span></span>|<span data-ttu-id="a05e5-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a05e5-109">String</span></span>|<span data-ttu-id="a05e5-110">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="a05e5-110">Display Name</span></span>|
|<span data-ttu-id="a05e5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a05e5-111">description</span></span>|<span data-ttu-id="a05e5-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a05e5-112">String</span></span>|<span data-ttu-id="a05e5-113">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="a05e5-113">Description.</span></span>|
|<span data-ttu-id="a05e5-114">omaUri</span><span class="sxs-lookup"><span data-stu-id="a05e5-114">omaUri</span></span>|<span data-ttu-id="a05e5-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a05e5-115">String</span></span>|<span data-ttu-id="a05e5-116">OMA.</span><span class="sxs-lookup"><span data-stu-id="a05e5-116">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a05e5-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a05e5-117">Relationships</span></span>
<span data-ttu-id="a05e5-118">Keine</span><span class="sxs-lookup"><span data-stu-id="a05e5-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a05e5-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a05e5-119">JSON Representation</span></span>
<span data-ttu-id="a05e5-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a05e5-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



