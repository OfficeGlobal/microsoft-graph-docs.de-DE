# <a name="omasettingstring-resource-type"></a><span data-ttu-id="f7d35-101">omaSettingString-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f7d35-101">omaSettingString resource type</span></span>

> <span data-ttu-id="f7d35-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f7d35-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7d35-103">Zeichenfolgendefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="f7d35-103">OMA Settings String definition.</span></span>

<span data-ttu-id="f7d35-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="f7d35-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f7d35-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7d35-105">Properties</span></span>
|<span data-ttu-id="f7d35-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7d35-106">Property</span></span>|<span data-ttu-id="f7d35-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f7d35-107">Type</span></span>|<span data-ttu-id="f7d35-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7d35-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d35-109">displayName</span><span class="sxs-lookup"><span data-stu-id="f7d35-109">displayName</span></span>|<span data-ttu-id="f7d35-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7d35-110">String</span></span>|<span data-ttu-id="f7d35-111">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="f7d35-111">Display Name</span></span> <span data-ttu-id="f7d35-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="f7d35-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="f7d35-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7d35-113">description</span></span>|<span data-ttu-id="f7d35-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7d35-114">String</span></span>|<span data-ttu-id="f7d35-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="f7d35-115">Description.</span></span> <span data-ttu-id="f7d35-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="f7d35-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="f7d35-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="f7d35-117">omaUri</span></span>|<span data-ttu-id="f7d35-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7d35-118">String</span></span>|<span data-ttu-id="f7d35-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="f7d35-119">OMA.</span></span> <span data-ttu-id="f7d35-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="f7d35-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="f7d35-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f7d35-121">value</span></span>|<span data-ttu-id="f7d35-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7d35-122">String</span></span>|<span data-ttu-id="f7d35-123">Wert.</span><span class="sxs-lookup"><span data-stu-id="f7d35-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7d35-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f7d35-124">Relationships</span></span>
<span data-ttu-id="f7d35-125">Keine</span><span class="sxs-lookup"><span data-stu-id="f7d35-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f7d35-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7d35-126">JSON Representation</span></span>
<span data-ttu-id="f7d35-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7d35-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



