# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="127af-101">omaSettingStringXml-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="127af-101">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="127af-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="127af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="127af-103">Zeichenfolgen-XML-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="127af-103">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="127af-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="127af-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="127af-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="127af-105">Properties</span></span>
|<span data-ttu-id="127af-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="127af-106">Property</span></span>|<span data-ttu-id="127af-107">Typ</span><span class="sxs-lookup"><span data-stu-id="127af-107">Type</span></span>|<span data-ttu-id="127af-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="127af-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="127af-109">displayName</span><span class="sxs-lookup"><span data-stu-id="127af-109">displayName</span></span>|<span data-ttu-id="127af-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="127af-110">String</span></span>|<span data-ttu-id="127af-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="127af-111">Display Name</span></span> <span data-ttu-id="127af-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="127af-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="127af-113">description</span><span class="sxs-lookup"><span data-stu-id="127af-113">description</span></span>|<span data-ttu-id="127af-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="127af-114">String</span></span>|<span data-ttu-id="127af-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="127af-115">Description.</span></span> <span data-ttu-id="127af-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="127af-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="127af-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="127af-117">omaUri</span></span>|<span data-ttu-id="127af-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="127af-118">String</span></span>|<span data-ttu-id="127af-119">OMA</span><span class="sxs-lookup"><span data-stu-id="127af-119">OMA.</span></span> <span data-ttu-id="127af-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="127af-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="127af-121">fileName</span><span class="sxs-lookup"><span data-stu-id="127af-121">fileName</span></span>|<span data-ttu-id="127af-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="127af-122">String</span></span>|<span data-ttu-id="127af-123">Die dem Dateinamen zugeordnete Werteigenschaft (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="127af-123">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="127af-124">value</span><span class="sxs-lookup"><span data-stu-id="127af-124">value</span></span>|<span data-ttu-id="127af-125">Binär</span><span class="sxs-lookup"><span data-stu-id="127af-125">Binary</span></span>|<span data-ttu-id="127af-126">Wert</span><span class="sxs-lookup"><span data-stu-id="127af-126">Value.</span></span> <span data-ttu-id="127af-127">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="127af-127">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="127af-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="127af-128">Relationships</span></span>
<span data-ttu-id="127af-129">Keine</span><span class="sxs-lookup"><span data-stu-id="127af-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="127af-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="127af-130">JSON Representation</span></span>
<span data-ttu-id="127af-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="127af-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```



