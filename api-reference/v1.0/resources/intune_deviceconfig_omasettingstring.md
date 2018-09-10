# <a name="omasettingstring-resource-type"></a><span data-ttu-id="b75fa-101">omaSettingString-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b75fa-101">omaSettingString resource type</span></span>

> <span data-ttu-id="b75fa-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b75fa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b75fa-103">Zeichenfolgendefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="b75fa-103">OMA Settings String definition.</span></span>

<span data-ttu-id="b75fa-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="b75fa-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b75fa-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b75fa-105">Properties</span></span>
|<span data-ttu-id="b75fa-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b75fa-106">Property</span></span>|<span data-ttu-id="b75fa-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b75fa-107">Type</span></span>|<span data-ttu-id="b75fa-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b75fa-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b75fa-109">displayName</span><span class="sxs-lookup"><span data-stu-id="b75fa-109">displayName</span></span>|<span data-ttu-id="b75fa-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b75fa-110">String</span></span>|<span data-ttu-id="b75fa-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="b75fa-111">Display Name.</span></span> <span data-ttu-id="b75fa-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b75fa-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b75fa-113">description</span><span class="sxs-lookup"><span data-stu-id="b75fa-113">description</span></span>|<span data-ttu-id="b75fa-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b75fa-114">String</span></span>|<span data-ttu-id="b75fa-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="b75fa-115">Description.</span></span> <span data-ttu-id="b75fa-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b75fa-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b75fa-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="b75fa-117">omaUri</span></span>|<span data-ttu-id="b75fa-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b75fa-118">String</span></span>|<span data-ttu-id="b75fa-119">OMA</span><span class="sxs-lookup"><span data-stu-id="b75fa-119">OMA.</span></span> <span data-ttu-id="b75fa-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b75fa-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b75fa-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b75fa-121">value</span></span>|<span data-ttu-id="b75fa-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b75fa-122">String</span></span>|<span data-ttu-id="b75fa-123">Wert.</span><span class="sxs-lookup"><span data-stu-id="b75fa-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b75fa-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b75fa-124">Relationships</span></span>
<span data-ttu-id="b75fa-125">Keine</span><span class="sxs-lookup"><span data-stu-id="b75fa-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b75fa-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b75fa-126">JSON Representation</span></span>
<span data-ttu-id="b75fa-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b75fa-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```








