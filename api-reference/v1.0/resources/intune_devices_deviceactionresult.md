# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="10b0b-101">deviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="10b0b-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="10b0b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="10b0b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10b0b-103">Ergebnis von Gerätevorgang</span><span class="sxs-lookup"><span data-stu-id="10b0b-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="10b0b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="10b0b-104">Properties</span></span>
|<span data-ttu-id="10b0b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10b0b-105">Property</span></span>|<span data-ttu-id="10b0b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="10b0b-106">Type</span></span>|<span data-ttu-id="10b0b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10b0b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10b0b-108">actionName</span><span class="sxs-lookup"><span data-stu-id="10b0b-108">ActionName</span></span>|<span data-ttu-id="10b0b-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10b0b-109">String</span></span>|<span data-ttu-id="10b0b-110">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="10b0b-110">Action name</span></span>|
|<span data-ttu-id="10b0b-111">actionState</span><span class="sxs-lookup"><span data-stu-id="10b0b-111">actionState</span></span>|<span data-ttu-id="10b0b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10b0b-112">String</span></span>|<span data-ttu-id="10b0b-113">Status der Aktion; mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="10b0b-113">State of the action Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="10b0b-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="10b0b-114">startDateTime</span></span>|<span data-ttu-id="10b0b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10b0b-115">DateTimeOffset</span></span>|<span data-ttu-id="10b0b-116">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="10b0b-116">Time the action was initiated</span></span>|
|<span data-ttu-id="10b0b-117">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="10b0b-117">lastUpdatedDateTime</span></span>|<span data-ttu-id="10b0b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10b0b-118">DateTimeOffset</span></span>|<span data-ttu-id="10b0b-119">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="10b0b-119">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="10b0b-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="10b0b-120">Relationships</span></span>
<span data-ttu-id="10b0b-121">Keine</span><span class="sxs-lookup"><span data-stu-id="10b0b-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10b0b-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="10b0b-122">JSON Representation</span></span>
<span data-ttu-id="10b0b-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="10b0b-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



