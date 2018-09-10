# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="b4e26-101">omaSettingFloatingPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b4e26-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="b4e26-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4e26-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4e26-103">Gleitkommadefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="b4e26-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="b4e26-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="b4e26-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4e26-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4e26-105">Properties</span></span>
|<span data-ttu-id="b4e26-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4e26-106">Property</span></span>|<span data-ttu-id="b4e26-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b4e26-107">Type</span></span>|<span data-ttu-id="b4e26-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4e26-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4e26-109">displayName</span><span class="sxs-lookup"><span data-stu-id="b4e26-109">displayName</span></span>|<span data-ttu-id="b4e26-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e26-110">String</span></span>|<span data-ttu-id="b4e26-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="b4e26-111">Display Name.</span></span> <span data-ttu-id="b4e26-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b4e26-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b4e26-113">description</span><span class="sxs-lookup"><span data-stu-id="b4e26-113">description</span></span>|<span data-ttu-id="b4e26-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e26-114">String</span></span>|<span data-ttu-id="b4e26-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="b4e26-115">Description.</span></span> <span data-ttu-id="b4e26-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b4e26-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b4e26-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="b4e26-117">omaUri</span></span>|<span data-ttu-id="b4e26-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4e26-118">String</span></span>|<span data-ttu-id="b4e26-119">OMA</span><span class="sxs-lookup"><span data-stu-id="b4e26-119">OMA.</span></span> <span data-ttu-id="b4e26-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b4e26-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b4e26-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b4e26-121">value</span></span>|<span data-ttu-id="b4e26-122">Einzelner</span><span class="sxs-lookup"><span data-stu-id="b4e26-122">Single</span></span>|<span data-ttu-id="b4e26-123">Wert.</span><span class="sxs-lookup"><span data-stu-id="b4e26-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4e26-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b4e26-124">Relationships</span></span>
<span data-ttu-id="b4e26-125">Keine</span><span class="sxs-lookup"><span data-stu-id="b4e26-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b4e26-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4e26-126">JSON Representation</span></span>
<span data-ttu-id="b4e26-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4e26-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```








