# <a name="devicemanagement-resource-type"></a><span data-ttu-id="c0303-101">deviceManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c0303-101">deviceManagement resource type</span></span>

> <span data-ttu-id="c0303-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0303-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0303-103">Singleton-Entität, die als Container für alle Geräte-App-Verwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="c0303-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="c0303-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="c0303-104">Methods</span></span>
|<span data-ttu-id="c0303-105">Methode</span><span class="sxs-lookup"><span data-stu-id="c0303-105">Method</span></span>|<span data-ttu-id="c0303-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c0303-106">Return Type</span></span>|<span data-ttu-id="c0303-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0303-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0303-108">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="c0303-108">Get deviceManagement</span></span>](../api/intune_auditing_devicemanagement_get.md)|[<span data-ttu-id="c0303-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c0303-109">deviceManagement</span></span>](../resources/intune_auditing_devicemanagement.md)|<span data-ttu-id="c0303-110">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_auditing_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c0303-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_auditing_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="c0303-111">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c0303-111">Update deviceManagement</span></span>](../api/intune_auditing_devicemanagement_update.md)|[<span data-ttu-id="c0303-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c0303-112">deviceManagement</span></span>](../resources/intune_auditing_devicemanagement.md)|<span data-ttu-id="c0303-113">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_auditing_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c0303-113">Update the properties of a [calendar](../resources/intune_auditing_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0303-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c0303-114">Properties</span></span>
|<span data-ttu-id="c0303-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0303-115">Property</span></span>|<span data-ttu-id="c0303-116">Typ</span><span class="sxs-lookup"><span data-stu-id="c0303-116">Type</span></span>|<span data-ttu-id="c0303-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0303-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0303-118">id</span><span class="sxs-lookup"><span data-stu-id="c0303-118">id</span></span>|<span data-ttu-id="c0303-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0303-119">String</span></span>|<span data-ttu-id="c0303-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c0303-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0303-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c0303-121">Relationships</span></span>
|<span data-ttu-id="c0303-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="c0303-122">Relationship</span></span>|<span data-ttu-id="c0303-123">Typ</span><span class="sxs-lookup"><span data-stu-id="c0303-123">Type</span></span>|<span data-ttu-id="c0303-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0303-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0303-125">auditEvents</span><span class="sxs-lookup"><span data-stu-id="c0303-125">auditEvents</span></span>|<span data-ttu-id="c0303-126">[auditEvent](../resources/intune_auditing_auditevent.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c0303-126">[auditEvent](../resources/intune_auditing_auditevent.md) collection</span></span>|<span data-ttu-id="c0303-127">Audit-Ereignisse</span><span class="sxs-lookup"><span data-stu-id="c0303-127">The Audit Events</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0303-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c0303-128">JSON Representation</span></span>
<span data-ttu-id="c0303-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c0303-129">Here is a JSON representation of the resource.</span></span>
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



