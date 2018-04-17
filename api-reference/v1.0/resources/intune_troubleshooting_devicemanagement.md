# <a name="devicemanagement-resource-type"></a><span data-ttu-id="daa49-101">deviceManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="daa49-101">deviceManagement resource type</span></span>

> <span data-ttu-id="daa49-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="daa49-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="daa49-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="daa49-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="daa49-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="daa49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="daa49-105">Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="daa49-105">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="daa49-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="daa49-106">Methods</span></span>
|<span data-ttu-id="daa49-107">Methode</span><span class="sxs-lookup"><span data-stu-id="daa49-107">Method</span></span>|<span data-ttu-id="daa49-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="daa49-108">Return Type</span></span>|<span data-ttu-id="daa49-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="daa49-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="daa49-110">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="daa49-110">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="daa49-111">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="daa49-111">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="daa49-112">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="daa49-112">Read properties and relationships of the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="daa49-113">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="daa49-113">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="daa49-114">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="daa49-114">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="daa49-115">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="daa49-115">Update the properties of a [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="daa49-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="daa49-116">Properties</span></span>
|<span data-ttu-id="daa49-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="daa49-117">Property</span></span>|<span data-ttu-id="daa49-118">Typ</span><span class="sxs-lookup"><span data-stu-id="daa49-118">Type</span></span>|<span data-ttu-id="daa49-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="daa49-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daa49-120">id</span><span class="sxs-lookup"><span data-stu-id="daa49-120">id</span></span>|<span data-ttu-id="daa49-121">String</span><span class="sxs-lookup"><span data-stu-id="daa49-121">String</span></span>|<span data-ttu-id="daa49-122">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="daa49-122">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="daa49-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="daa49-123">Relationships</span></span>
|<span data-ttu-id="daa49-124">Beziehung</span><span class="sxs-lookup"><span data-stu-id="daa49-124">Relationship</span></span>|<span data-ttu-id="daa49-125">Typ</span><span class="sxs-lookup"><span data-stu-id="daa49-125">Type</span></span>|<span data-ttu-id="daa49-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="daa49-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daa49-127">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="daa49-127">troubleshootingEvents</span></span>|<span data-ttu-id="daa49-128">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="daa49-128">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="daa49-129">Die Liste der Problembehandlungsereignisse für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="daa49-129">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="daa49-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="daa49-130">JSON Representation</span></span>
<span data-ttu-id="daa49-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="daa49-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



