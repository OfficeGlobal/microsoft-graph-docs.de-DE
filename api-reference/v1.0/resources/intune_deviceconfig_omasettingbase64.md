# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="0a97f-101">omaSettingBase64-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0a97f-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="0a97f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0a97f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a97f-103">Base64-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="0a97f-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="0a97f-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0a97f-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0a97f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a97f-105">Properties</span></span>
|<span data-ttu-id="0a97f-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a97f-106">Property</span></span>|<span data-ttu-id="0a97f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="0a97f-107">Type</span></span>|<span data-ttu-id="0a97f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a97f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a97f-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0a97f-109">displayName</span></span>|<span data-ttu-id="0a97f-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a97f-110">String</span></span>|<span data-ttu-id="0a97f-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="0a97f-111">Display Name.</span></span> <span data-ttu-id="0a97f-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0a97f-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0a97f-113">description</span><span class="sxs-lookup"><span data-stu-id="0a97f-113">description</span></span>|<span data-ttu-id="0a97f-114">String</span><span class="sxs-lookup"><span data-stu-id="0a97f-114">String</span></span>|<span data-ttu-id="0a97f-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="0a97f-115">Description.</span></span> <span data-ttu-id="0a97f-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0a97f-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0a97f-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="0a97f-117">omaUri</span></span>|<span data-ttu-id="0a97f-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a97f-118">String</span></span>|<span data-ttu-id="0a97f-119">OMA</span><span class="sxs-lookup"><span data-stu-id="0a97f-119">OMA.</span></span> <span data-ttu-id="0a97f-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0a97f-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0a97f-121">fileName</span><span class="sxs-lookup"><span data-stu-id="0a97f-121">fileName</span></span>|<span data-ttu-id="0a97f-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a97f-122">String</span></span>|<span data-ttu-id="0a97f-123">Die dem Dateinamen zugeordnete Werteigenschaft (\*.cer</span><span class="sxs-lookup"><span data-stu-id="0a97f-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="0a97f-124">\*.crt ).</span><span class="sxs-lookup"><span data-stu-id="0a97f-124">\*.crt ).</span></span>|
|<span data-ttu-id="0a97f-125">value</span><span class="sxs-lookup"><span data-stu-id="0a97f-125">value</span></span>|<span data-ttu-id="0a97f-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a97f-126">String</span></span>|<span data-ttu-id="0a97f-127">Wert</span><span class="sxs-lookup"><span data-stu-id="0a97f-127">Value.</span></span> <span data-ttu-id="0a97f-128">(Base64-codierte Zeichenfolge)</span><span class="sxs-lookup"><span data-stu-id="0a97f-128">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a97f-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0a97f-129">Relationships</span></span>
<span data-ttu-id="0a97f-130">Keine</span><span class="sxs-lookup"><span data-stu-id="0a97f-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a97f-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0a97f-131">JSON Representation</span></span>
<span data-ttu-id="0a97f-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0a97f-132">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}-->
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



