# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="fe919-101">omaSettingInteger-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fe919-101">omaSettingInteger resource type</span></span>

> <span data-ttu-id="fe919-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fe919-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe919-103">Ganzzahl-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="fe919-103">OMA Settings Integer definition.</span></span>

<span data-ttu-id="fe919-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fe919-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fe919-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fe919-105">Properties</span></span>
|<span data-ttu-id="fe919-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fe919-106">Property</span></span>|<span data-ttu-id="fe919-107">Typ</span><span class="sxs-lookup"><span data-stu-id="fe919-107">Type</span></span>|<span data-ttu-id="fe919-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe919-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe919-109">displayName</span><span class="sxs-lookup"><span data-stu-id="fe919-109">displayName</span></span>|<span data-ttu-id="fe919-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe919-110">String</span></span>|<span data-ttu-id="fe919-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="fe919-111">Display Name</span></span> <span data-ttu-id="fe919-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fe919-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fe919-113">description</span><span class="sxs-lookup"><span data-stu-id="fe919-113">description</span></span>|<span data-ttu-id="fe919-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe919-114">String</span></span>|<span data-ttu-id="fe919-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe919-115">Description.</span></span> <span data-ttu-id="fe919-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fe919-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fe919-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="fe919-117">omaUri</span></span>|<span data-ttu-id="fe919-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe919-118">String</span></span>|<span data-ttu-id="fe919-119">OMA</span><span class="sxs-lookup"><span data-stu-id="fe919-119">OMA.</span></span> <span data-ttu-id="fe919-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fe919-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fe919-121">value</span><span class="sxs-lookup"><span data-stu-id="fe919-121">value</span></span>|<span data-ttu-id="fe919-122">Int32</span><span class="sxs-lookup"><span data-stu-id="fe919-122">Int32</span></span>|<span data-ttu-id="fe919-123">Wert</span><span class="sxs-lookup"><span data-stu-id="fe919-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe919-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fe919-124">Relationships</span></span>
<span data-ttu-id="fe919-125">Keine</span><span class="sxs-lookup"><span data-stu-id="fe919-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fe919-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fe919-126">JSON Representation</span></span>
<span data-ttu-id="fe919-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fe919-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



