# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="4ece5-101">importedWindowsAutopilotDeviceIdentityState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4ece5-101">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="4ece5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4ece5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ece5-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4ece5-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4ece5-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4ece5-104">Properties</span></span>
|<span data-ttu-id="4ece5-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4ece5-105">Property</span></span>|<span data-ttu-id="4ece5-106">Typ</span><span class="sxs-lookup"><span data-stu-id="4ece5-106">Type</span></span>|<span data-ttu-id="4ece5-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ece5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ece5-108">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="4ece5-108">deviceImportStatus</span></span>|[<span data-ttu-id="4ece5-109">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="4ece5-109">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="4ece5-110">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="4ece5-110">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="4ece5-111">Die möglichen Werte sind: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="4ece5-111">The possible values are `unknown`, `pending`, `partial`, `complete`, `error`, , , , , , , or .</span></span>|
|<span data-ttu-id="4ece5-112">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="4ece5-112">deviceRegistrationId</span></span>|<span data-ttu-id="4ece5-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ece5-113">String</span></span>|<span data-ttu-id="4ece5-114">Vom Geräteverzeichnisdienst (DDS) gemeldete Geräteregistrierungs-ID für erfolgreich hinzugefügtes Gerät</span><span class="sxs-lookup"><span data-stu-id="4ece5-114">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="4ece5-115">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="4ece5-115">deviceErrorCode</span></span>|<span data-ttu-id="4ece5-116">Int32</span><span class="sxs-lookup"><span data-stu-id="4ece5-116">Int32</span></span>|<span data-ttu-id="4ece5-117">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlercode</span><span class="sxs-lookup"><span data-stu-id="4ece5-117">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="4ece5-118">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="4ece5-118">deviceErrorName</span></span>|<span data-ttu-id="4ece5-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ece5-119">String</span></span>|<span data-ttu-id="4ece5-120">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlername</span><span class="sxs-lookup"><span data-stu-id="4ece5-120">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ece5-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4ece5-121">Relationships</span></span>
<span data-ttu-id="4ece5-122">Keine</span><span class="sxs-lookup"><span data-stu-id="4ece5-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4ece5-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4ece5-123">JSON Representation</span></span>
<span data-ttu-id="4ece5-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4ece5-124">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```



