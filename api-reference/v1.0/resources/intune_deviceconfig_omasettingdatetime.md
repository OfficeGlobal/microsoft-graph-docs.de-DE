# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="abad1-101">omaSettingDateTime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="abad1-101">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="abad1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="abad1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abad1-103">DateTime-Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="abad1-103">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="abad1-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="abad1-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="abad1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="abad1-105">Properties</span></span>
|<span data-ttu-id="abad1-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="abad1-106">Property</span></span>|<span data-ttu-id="abad1-107">Typ</span><span class="sxs-lookup"><span data-stu-id="abad1-107">Type</span></span>|<span data-ttu-id="abad1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abad1-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abad1-109">displayName</span><span class="sxs-lookup"><span data-stu-id="abad1-109">displayName</span></span>|<span data-ttu-id="abad1-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abad1-110">String</span></span>|<span data-ttu-id="abad1-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="abad1-111">Display Name.</span></span> <span data-ttu-id="abad1-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="abad1-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="abad1-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abad1-113">description</span></span>|<span data-ttu-id="abad1-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abad1-114">String</span></span>|<span data-ttu-id="abad1-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="abad1-115">Description.</span></span> <span data-ttu-id="abad1-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="abad1-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="abad1-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="abad1-117">omaUri</span></span>|<span data-ttu-id="abad1-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abad1-118">String</span></span>|<span data-ttu-id="abad1-119">OMA</span><span class="sxs-lookup"><span data-stu-id="abad1-119">OMA.</span></span> <span data-ttu-id="abad1-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="abad1-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="abad1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="abad1-121">value</span></span>|<span data-ttu-id="abad1-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abad1-122">DateTimeOffset</span></span>|<span data-ttu-id="abad1-123">Wert.</span><span class="sxs-lookup"><span data-stu-id="abad1-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abad1-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="abad1-124">Relationships</span></span>
<span data-ttu-id="abad1-125">Keine</span><span class="sxs-lookup"><span data-stu-id="abad1-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="abad1-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="abad1-126">JSON Representation</span></span>
<span data-ttu-id="abad1-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="abad1-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



