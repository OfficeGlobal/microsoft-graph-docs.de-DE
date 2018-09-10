# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="69599-101">omaSettingInteger-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="69599-101">omaSettingInteger resource type</span></span>

> <span data-ttu-id="69599-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69599-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69599-103">Ganzzahl-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="69599-103">OMA Settings Integer definition.</span></span>

<span data-ttu-id="69599-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="69599-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69599-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69599-105">Properties</span></span>
|<span data-ttu-id="69599-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69599-106">Property</span></span>|<span data-ttu-id="69599-107">Typ</span><span class="sxs-lookup"><span data-stu-id="69599-107">Type</span></span>|<span data-ttu-id="69599-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69599-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69599-109">displayName</span><span class="sxs-lookup"><span data-stu-id="69599-109">displayName</span></span>|<span data-ttu-id="69599-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69599-110">String</span></span>|<span data-ttu-id="69599-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="69599-111">Display Name.</span></span> <span data-ttu-id="69599-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="69599-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="69599-113">description</span><span class="sxs-lookup"><span data-stu-id="69599-113">description</span></span>|<span data-ttu-id="69599-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69599-114">String</span></span>|<span data-ttu-id="69599-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="69599-115">Description.</span></span> <span data-ttu-id="69599-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="69599-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="69599-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="69599-117">omaUri</span></span>|<span data-ttu-id="69599-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69599-118">String</span></span>|<span data-ttu-id="69599-119">OMA</span><span class="sxs-lookup"><span data-stu-id="69599-119">OMA.</span></span> <span data-ttu-id="69599-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="69599-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="69599-121">value</span><span class="sxs-lookup"><span data-stu-id="69599-121">value</span></span>|<span data-ttu-id="69599-122">Int32</span><span class="sxs-lookup"><span data-stu-id="69599-122">Int32</span></span>|<span data-ttu-id="69599-123">Wert</span><span class="sxs-lookup"><span data-stu-id="69599-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69599-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="69599-124">Relationships</span></span>
<span data-ttu-id="69599-125">Keine</span><span class="sxs-lookup"><span data-stu-id="69599-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="69599-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69599-126">JSON Representation</span></span>
<span data-ttu-id="69599-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="69599-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```








