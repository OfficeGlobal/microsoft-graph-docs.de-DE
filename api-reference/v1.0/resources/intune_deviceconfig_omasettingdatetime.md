# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="94b84-101">omaSettingDateTime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="94b84-101">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="94b84-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="94b84-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94b84-103">DateTime-Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="94b84-103">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="94b84-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="94b84-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="94b84-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94b84-105">Properties</span></span>
|<span data-ttu-id="94b84-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94b84-106">Property</span></span>|<span data-ttu-id="94b84-107">Typ</span><span class="sxs-lookup"><span data-stu-id="94b84-107">Type</span></span>|<span data-ttu-id="94b84-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94b84-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94b84-109">displayName</span><span class="sxs-lookup"><span data-stu-id="94b84-109">displayName</span></span>|<span data-ttu-id="94b84-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="94b84-110">String</span></span>|<span data-ttu-id="94b84-111">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="94b84-111">Display Name</span></span> <span data-ttu-id="94b84-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="94b84-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="94b84-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94b84-113">description</span></span>|<span data-ttu-id="94b84-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="94b84-114">String</span></span>|<span data-ttu-id="94b84-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="94b84-115">Description.</span></span> <span data-ttu-id="94b84-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="94b84-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="94b84-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="94b84-117">omaUri</span></span>|<span data-ttu-id="94b84-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="94b84-118">String</span></span>|<span data-ttu-id="94b84-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="94b84-119">OMA.</span></span> <span data-ttu-id="94b84-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="94b84-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="94b84-121">Wert</span><span class="sxs-lookup"><span data-stu-id="94b84-121">value</span></span>|<span data-ttu-id="94b84-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94b84-122">DateTimeOffset</span></span>|<span data-ttu-id="94b84-123">Wert.</span><span class="sxs-lookup"><span data-stu-id="94b84-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94b84-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="94b84-124">Relationships</span></span>
<span data-ttu-id="94b84-125">Keine</span><span class="sxs-lookup"><span data-stu-id="94b84-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94b84-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="94b84-126">JSON Representation</span></span>
<span data-ttu-id="94b84-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="94b84-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



