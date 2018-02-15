# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="8d46e-101">omaSettingBase64-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8d46e-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="8d46e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d46e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d46e-103">Base64-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="8d46e-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="8d46e-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8d46e-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d46e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8d46e-105">Properties</span></span>
|<span data-ttu-id="8d46e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d46e-106">Property</span></span>|<span data-ttu-id="8d46e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="8d46e-107">Type</span></span>|<span data-ttu-id="8d46e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d46e-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d46e-109">displayName</span><span class="sxs-lookup"><span data-stu-id="8d46e-109">displayName</span></span>|<span data-ttu-id="8d46e-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d46e-110">String</span></span>|<span data-ttu-id="8d46e-111">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="8d46e-111">Display Name</span></span> <span data-ttu-id="8d46e-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8d46e-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="8d46e-113">description</span><span class="sxs-lookup"><span data-stu-id="8d46e-113">description</span></span>|<span data-ttu-id="8d46e-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d46e-114">String</span></span>|<span data-ttu-id="8d46e-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d46e-115">Description.</span></span> <span data-ttu-id="8d46e-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8d46e-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="8d46e-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="8d46e-117">omaUri</span></span>|<span data-ttu-id="8d46e-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d46e-118">String</span></span>|<span data-ttu-id="8d46e-119">OMA</span><span class="sxs-lookup"><span data-stu-id="8d46e-119">OMA.</span></span> <span data-ttu-id="8d46e-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8d46e-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="8d46e-121">fileName</span><span class="sxs-lookup"><span data-stu-id="8d46e-121">fileName</span></span>|<span data-ttu-id="8d46e-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d46e-122">String</span></span>|<span data-ttu-id="8d46e-123">Die dem Dateinamen zugeordnete Werteigenschaft (\*.cer</span><span class="sxs-lookup"><span data-stu-id="8d46e-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="8d46e-124">\*.crt ).</span><span class="sxs-lookup"><span data-stu-id="8d46e-124">\*.crt ).</span></span>|
|<span data-ttu-id="8d46e-125">value</span><span class="sxs-lookup"><span data-stu-id="8d46e-125">value</span></span>|<span data-ttu-id="8d46e-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d46e-126">String</span></span>|<span data-ttu-id="8d46e-127">Wert</span><span class="sxs-lookup"><span data-stu-id="8d46e-127">Value.</span></span> <span data-ttu-id="8d46e-128">(Base64-codierte Zeichenfolge)</span><span class="sxs-lookup"><span data-stu-id="8d46e-128">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d46e-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8d46e-129">Relationships</span></span>
<span data-ttu-id="8d46e-130">Keine</span><span class="sxs-lookup"><span data-stu-id="8d46e-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8d46e-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8d46e-131">JSON Representation</span></span>
<span data-ttu-id="8d46e-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8d46e-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



