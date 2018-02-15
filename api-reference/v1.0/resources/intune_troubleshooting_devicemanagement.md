# <a name="devicemanagement-resource-type"></a><span data-ttu-id="3a2db-101">deviceManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3a2db-101">deviceManagement resource type</span></span>

> <span data-ttu-id="3a2db-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3a2db-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a2db-103">Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="3a2db-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="3a2db-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="3a2db-104">Methods</span></span>
|<span data-ttu-id="3a2db-105">Methode</span><span class="sxs-lookup"><span data-stu-id="3a2db-105">Method</span></span>|<span data-ttu-id="3a2db-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3a2db-106">Return Type</span></span>|<span data-ttu-id="3a2db-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a2db-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3a2db-108">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="3a2db-108">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="3a2db-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3a2db-109">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="3a2db-110">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3a2db-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="3a2db-111">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3a2db-111">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="3a2db-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3a2db-112">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="3a2db-113">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3a2db-113">Update the properties of a [calendar](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3a2db-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3a2db-114">Properties</span></span>
|<span data-ttu-id="3a2db-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3a2db-115">Property</span></span>|<span data-ttu-id="3a2db-116">Typ</span><span class="sxs-lookup"><span data-stu-id="3a2db-116">Type</span></span>|<span data-ttu-id="3a2db-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a2db-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a2db-118">id</span><span class="sxs-lookup"><span data-stu-id="3a2db-118">id</span></span>|<span data-ttu-id="3a2db-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a2db-119">String</span></span>|<span data-ttu-id="3a2db-120">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3a2db-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a2db-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3a2db-121">Relationships</span></span>
|<span data-ttu-id="3a2db-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3a2db-122">Relationship</span></span>|<span data-ttu-id="3a2db-123">Typ</span><span class="sxs-lookup"><span data-stu-id="3a2db-123">Type</span></span>|<span data-ttu-id="3a2db-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a2db-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a2db-125">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="3a2db-125">troubleshootingEvents</span></span>|<span data-ttu-id="3a2db-126">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3a2db-126">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="3a2db-127">Die Liste der Problembehandlungsereignisse für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3a2db-127">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a2db-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3a2db-128">JSON Representation</span></span>
<span data-ttu-id="3a2db-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3a2db-129">Here is a JSON representation of the resource.</span></span>
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



