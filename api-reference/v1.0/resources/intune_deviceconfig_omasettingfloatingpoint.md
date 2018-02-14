# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="112d4-101">omaSettingFloatingPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="112d4-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="112d4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="112d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="112d4-103">Gleitkommadefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="112d4-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="112d4-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="112d4-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="112d4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="112d4-105">Properties</span></span>
|<span data-ttu-id="112d4-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="112d4-106">Property</span></span>|<span data-ttu-id="112d4-107">Typ</span><span class="sxs-lookup"><span data-stu-id="112d4-107">Type</span></span>|<span data-ttu-id="112d4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="112d4-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="112d4-109">displayName</span><span class="sxs-lookup"><span data-stu-id="112d4-109">displayName</span></span>|<span data-ttu-id="112d4-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="112d4-110">String</span></span>|<span data-ttu-id="112d4-111">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="112d4-111">Display Name</span></span> <span data-ttu-id="112d4-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="112d4-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="112d4-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="112d4-113">description</span></span>|<span data-ttu-id="112d4-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="112d4-114">String</span></span>|<span data-ttu-id="112d4-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="112d4-115">Description.</span></span> <span data-ttu-id="112d4-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="112d4-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="112d4-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="112d4-117">omaUri</span></span>|<span data-ttu-id="112d4-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="112d4-118">String</span></span>|<span data-ttu-id="112d4-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="112d4-119">OMA.</span></span> <span data-ttu-id="112d4-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="112d4-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="112d4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="112d4-121">value</span></span>|<span data-ttu-id="112d4-122">Einzelner</span><span class="sxs-lookup"><span data-stu-id="112d4-122">Single</span></span>|<span data-ttu-id="112d4-123">Wert.</span><span class="sxs-lookup"><span data-stu-id="112d4-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="112d4-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="112d4-124">Relationships</span></span>
<span data-ttu-id="112d4-125">Keine</span><span class="sxs-lookup"><span data-stu-id="112d4-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="112d4-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="112d4-126">JSON Representation</span></span>
<span data-ttu-id="112d4-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="112d4-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



