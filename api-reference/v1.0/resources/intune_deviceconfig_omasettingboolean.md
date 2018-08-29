# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="ae50d-101">omaSettingBoolean-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ae50d-101">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="ae50d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ae50d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae50d-103">Boolesche Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="ae50d-103">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="ae50d-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="ae50d-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ae50d-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae50d-105">Properties</span></span>
|<span data-ttu-id="ae50d-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae50d-106">Property</span></span>|<span data-ttu-id="ae50d-107">Typ</span><span class="sxs-lookup"><span data-stu-id="ae50d-107">Type</span></span>|<span data-ttu-id="ae50d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae50d-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae50d-109">displayName</span><span class="sxs-lookup"><span data-stu-id="ae50d-109">displayName</span></span>|<span data-ttu-id="ae50d-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae50d-110">String</span></span>|<span data-ttu-id="ae50d-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="ae50d-111">Display Name.</span></span> <span data-ttu-id="ae50d-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ae50d-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="ae50d-113">description</span><span class="sxs-lookup"><span data-stu-id="ae50d-113">description</span></span>|<span data-ttu-id="ae50d-114">String</span><span class="sxs-lookup"><span data-stu-id="ae50d-114">String</span></span>|<span data-ttu-id="ae50d-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="ae50d-115">Description.</span></span> <span data-ttu-id="ae50d-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ae50d-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="ae50d-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="ae50d-117">omaUri</span></span>|<span data-ttu-id="ae50d-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae50d-118">String</span></span>|<span data-ttu-id="ae50d-119">OMA</span><span class="sxs-lookup"><span data-stu-id="ae50d-119">OMA.</span></span> <span data-ttu-id="ae50d-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ae50d-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="ae50d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ae50d-121">value</span></span>|<span data-ttu-id="ae50d-122">Boolescher</span><span class="sxs-lookup"><span data-stu-id="ae50d-122">Boolean</span></span>|<span data-ttu-id="ae50d-123">Wert.</span><span class="sxs-lookup"><span data-stu-id="ae50d-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae50d-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ae50d-124">Relationships</span></span>
<span data-ttu-id="ae50d-125">Keine</span><span class="sxs-lookup"><span data-stu-id="ae50d-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ae50d-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae50d-126">JSON Representation</span></span>
<span data-ttu-id="ae50d-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ae50d-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



