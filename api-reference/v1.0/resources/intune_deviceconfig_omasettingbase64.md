# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="658bd-101">omaSettingBase64-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="658bd-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="658bd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="658bd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="658bd-103">Base64-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="658bd-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="658bd-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="658bd-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="658bd-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="658bd-105">Properties</span></span>
|<span data-ttu-id="658bd-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="658bd-106">Property</span></span>|<span data-ttu-id="658bd-107">Typ</span><span class="sxs-lookup"><span data-stu-id="658bd-107">Type</span></span>|<span data-ttu-id="658bd-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="658bd-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="658bd-109">displayName</span><span class="sxs-lookup"><span data-stu-id="658bd-109">displayName</span></span>|<span data-ttu-id="658bd-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="658bd-110">String</span></span>|<span data-ttu-id="658bd-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="658bd-111">Display Name.</span></span> <span data-ttu-id="658bd-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="658bd-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="658bd-113">description</span><span class="sxs-lookup"><span data-stu-id="658bd-113">description</span></span>|<span data-ttu-id="658bd-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="658bd-114">String</span></span>|<span data-ttu-id="658bd-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="658bd-115">Description.</span></span> <span data-ttu-id="658bd-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="658bd-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="658bd-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="658bd-117">omaUri</span></span>|<span data-ttu-id="658bd-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="658bd-118">String</span></span>|<span data-ttu-id="658bd-119">OMA</span><span class="sxs-lookup"><span data-stu-id="658bd-119">OMA.</span></span> <span data-ttu-id="658bd-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="658bd-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="658bd-121">fileName</span><span class="sxs-lookup"><span data-stu-id="658bd-121">fileName</span></span>|<span data-ttu-id="658bd-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="658bd-122">String</span></span>|<span data-ttu-id="658bd-123">Die dem Dateinamen zugeordnete Werteigenschaft (\*.cer</span><span class="sxs-lookup"><span data-stu-id="658bd-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="658bd-124">.CRT</span><span class="sxs-lookup"><span data-stu-id="658bd-124">\*.crt</span></span> | <span data-ttu-id="658bd-125">p7b</span><span class="sxs-lookup"><span data-stu-id="658bd-125">\*.p7b</span></span> | <span data-ttu-id="658bd-126">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="658bd-126">\*.bin).</span></span>|
|<span data-ttu-id="658bd-127">Wert</span><span class="sxs-lookup"><span data-stu-id="658bd-127">value</span></span>|<span data-ttu-id="658bd-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="658bd-128">String</span></span>|<span data-ttu-id="658bd-129">Wert</span><span class="sxs-lookup"><span data-stu-id="658bd-129">Value.</span></span> <span data-ttu-id="658bd-130">(Base64-codierte Zeichenfolge)</span><span class="sxs-lookup"><span data-stu-id="658bd-130">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="658bd-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="658bd-131">Relationships</span></span>
<span data-ttu-id="658bd-132">Keine</span><span class="sxs-lookup"><span data-stu-id="658bd-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="658bd-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="658bd-133">JSON Representation</span></span>
<span data-ttu-id="658bd-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="658bd-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



