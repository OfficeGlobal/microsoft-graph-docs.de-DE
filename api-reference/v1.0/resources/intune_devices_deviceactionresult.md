# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="322c9-101">deviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="322c9-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="322c9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="322c9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="322c9-103">Ergebnis von Gerätevorgang</span><span class="sxs-lookup"><span data-stu-id="322c9-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="322c9-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="322c9-104">Properties</span></span>
|<span data-ttu-id="322c9-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="322c9-105">Property</span></span>|<span data-ttu-id="322c9-106">Typ</span><span class="sxs-lookup"><span data-stu-id="322c9-106">Type</span></span>|<span data-ttu-id="322c9-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="322c9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="322c9-108">actionName</span><span class="sxs-lookup"><span data-stu-id="322c9-108">actionName</span></span>|<span data-ttu-id="322c9-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="322c9-109">String</span></span>|<span data-ttu-id="322c9-110">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="322c9-110">Action name</span></span>|
|<span data-ttu-id="322c9-111">actionState</span><span class="sxs-lookup"><span data-stu-id="322c9-111">actionState</span></span>|[<span data-ttu-id="322c9-112">actionState</span><span class="sxs-lookup"><span data-stu-id="322c9-112">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="322c9-p101">Status der Aktion; mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="322c9-p101">State of the action Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="322c9-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="322c9-115">startDateTime</span></span>|<span data-ttu-id="322c9-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="322c9-116">DateTimeOffset</span></span>|<span data-ttu-id="322c9-117">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="322c9-117">Time the action was initiated</span></span>|
|<span data-ttu-id="322c9-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="322c9-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="322c9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="322c9-119">DateTimeOffset</span></span>|<span data-ttu-id="322c9-120">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="322c9-120">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="322c9-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="322c9-121">Relationships</span></span>
<span data-ttu-id="322c9-122">Keine</span><span class="sxs-lookup"><span data-stu-id="322c9-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="322c9-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="322c9-123">JSON Representation</span></span>
<span data-ttu-id="322c9-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="322c9-124">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```








