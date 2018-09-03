# <a name="reportroot-resource-type"></a><span data-ttu-id="52afe-101">reportRoot-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="52afe-101">reportRoot resource type</span></span>

> <span data-ttu-id="52afe-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="52afe-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52afe-103">Die Ressource, die eine Instanz der Verlaufsberichte darstellt.</span><span class="sxs-lookup"><span data-stu-id="52afe-103">The resource that represents an instance of History Reports.</span></span>
## <a name="methods"></a><span data-ttu-id="52afe-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="52afe-104">Methods</span></span>
|<span data-ttu-id="52afe-105">Methode</span><span class="sxs-lookup"><span data-stu-id="52afe-105">Method</span></span>|<span data-ttu-id="52afe-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="52afe-106">Return Type</span></span>|<span data-ttu-id="52afe-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52afe-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="52afe-108">reportRoot abrufen</span><span class="sxs-lookup"><span data-stu-id="52afe-108">Get reportRoot</span></span>](../api/intune_deviceconfig_reportroot_get.md)|[<span data-ttu-id="52afe-109">reportRoot</span><span class="sxs-lookup"><span data-stu-id="52afe-109">reportRoot</span></span>](../resources/intune_deviceconfig_reportroot.md)|<span data-ttu-id="52afe-110">Lesen von Eigenschaften und Beziehungen des [reportRoot](../resources/intune_deviceconfig_reportroot.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="52afe-110">Read properties and relationships of the [reportRoot](../resources/intune_deviceconfig_reportroot.md) object.</span></span>|
|[<span data-ttu-id="52afe-111">reportRoot aktualisieren</span><span class="sxs-lookup"><span data-stu-id="52afe-111">Update reportRoot</span></span>](../api/intune_deviceconfig_reportroot_update.md)|[<span data-ttu-id="52afe-112">reportRoot</span><span class="sxs-lookup"><span data-stu-id="52afe-112">reportRoot</span></span>](../resources/intune_deviceconfig_reportroot.md)|<span data-ttu-id="52afe-113">Aktualisieren der Eigenschaften eines [reportRoot](../resources/intune_deviceconfig_reportroot.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="52afe-113">Update the properties of a [reportRoot](../resources/intune_deviceconfig_reportroot.md) object.</span></span>|
|[<span data-ttu-id="52afe-114">deviceConfigurationUserActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="52afe-114">deviceConfigurationUserActivity function</span></span>](../api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md)|[<span data-ttu-id="52afe-115">Bericht</span><span class="sxs-lookup"><span data-stu-id="52afe-115">report</span></span>](../resources/intune_deviceconfig_report.md)|<span data-ttu-id="52afe-116">Metadaten für den Gerätekonfigurations-Benutzeraktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="52afe-116">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="52afe-117">deviceConfigurationDeviceActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="52afe-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="52afe-118">Bericht</span><span class="sxs-lookup"><span data-stu-id="52afe-118">report</span></span>](../resources/intune_deviceconfig_report.md)|<span data-ttu-id="52afe-119">Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="52afe-119">Metadata for the device configuration device activity report</span></span>|

## <a name="relationships"></a><span data-ttu-id="52afe-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="52afe-120">Relationships</span></span>
<span data-ttu-id="52afe-121">Keine</span><span class="sxs-lookup"><span data-stu-id="52afe-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52afe-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="52afe-122">JSON Representation</span></span>
<span data-ttu-id="52afe-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="52afe-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
}
```

## <a name="example"></a><span data-ttu-id="52afe-124">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52afe-124">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
