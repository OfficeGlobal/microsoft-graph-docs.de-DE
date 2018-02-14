# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="00272-101">omaSettingBoolean-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="00272-101">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="00272-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="00272-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00272-103">Boolesche Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="00272-103">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="00272-104">Erbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="00272-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="00272-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00272-105">Properties</span></span>
|<span data-ttu-id="00272-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00272-106">Property</span></span>|<span data-ttu-id="00272-107">Typ</span><span class="sxs-lookup"><span data-stu-id="00272-107">Type</span></span>|<span data-ttu-id="00272-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00272-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00272-109">displayName</span><span class="sxs-lookup"><span data-stu-id="00272-109">displayName</span></span>|<span data-ttu-id="00272-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00272-110">String</span></span>|<span data-ttu-id="00272-111">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="00272-111">Display Name</span></span> <span data-ttu-id="00272-112">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="00272-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="00272-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00272-113">description</span></span>|<span data-ttu-id="00272-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00272-114">String</span></span>|<span data-ttu-id="00272-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="00272-115">Description.</span></span> <span data-ttu-id="00272-116">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="00272-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="00272-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="00272-117">omaUri</span></span>|<span data-ttu-id="00272-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00272-118">String</span></span>|<span data-ttu-id="00272-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="00272-119">OMA.</span></span> <span data-ttu-id="00272-120">Vererbt von [omaSetting](../resources/intune_deviceconfig_omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="00272-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="00272-121">Wert</span><span class="sxs-lookup"><span data-stu-id="00272-121">value</span></span>|<span data-ttu-id="00272-122">Boolescher</span><span class="sxs-lookup"><span data-stu-id="00272-122">Boolean</span></span>|<span data-ttu-id="00272-123">Wert.</span><span class="sxs-lookup"><span data-stu-id="00272-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00272-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="00272-124">Relationships</span></span>
<span data-ttu-id="00272-125">Keine</span><span class="sxs-lookup"><span data-stu-id="00272-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00272-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00272-126">JSON Representation</span></span>
<span data-ttu-id="00272-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00272-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



