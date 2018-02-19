# <a name="devicemanagement-resource-type"></a><span data-ttu-id="c6db7-101">deviceManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c6db7-101">deviceManagement resource type</span></span>

> <span data-ttu-id="c6db7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c6db7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6db7-103">Die deviceManagement-Ressource stellt die Geräteentitäten der Sammlung eines Mandanten dar, die vorab in Intune bereitgestellt wurden, und die Registrierungsprofile, die Geräteidentitäten zugewiesen werden können, die eine Konfiguration der Vorabregistrierung unterstützen.</span><span class="sxs-lookup"><span data-stu-id="c6db7-103">The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="c6db7-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="c6db7-104">Methods</span></span>
|<span data-ttu-id="c6db7-105">Methode</span><span class="sxs-lookup"><span data-stu-id="c6db7-105">Method</span></span>|<span data-ttu-id="c6db7-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c6db7-106">Return Type</span></span>|<span data-ttu-id="c6db7-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6db7-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6db7-108">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="c6db7-108">Get deviceManagement</span></span>](../api/intune_enrollment_devicemanagement_get.md)|[<span data-ttu-id="c6db7-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c6db7-109">deviceManagement</span></span>](../resources/intune_enrollment_devicemanagement.md)|<span data-ttu-id="c6db7-110">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_enrollment_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c6db7-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_enrollment_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="c6db7-111">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c6db7-111">Update deviceManagement</span></span>](../api/intune_enrollment_devicemanagement_update.md)|[<span data-ttu-id="c6db7-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c6db7-112">deviceManagement</span></span>](../resources/intune_enrollment_devicemanagement.md)|<span data-ttu-id="c6db7-113">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_enrollment_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c6db7-113">Update the properties of a [calendar](../resources/intune_enrollment_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6db7-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c6db7-114">Properties</span></span>
|<span data-ttu-id="c6db7-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6db7-115">Property</span></span>|<span data-ttu-id="c6db7-116">Typ</span><span class="sxs-lookup"><span data-stu-id="c6db7-116">Type</span></span>|<span data-ttu-id="c6db7-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6db7-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6db7-118">id</span><span class="sxs-lookup"><span data-stu-id="c6db7-118">id</span></span>|<span data-ttu-id="c6db7-119">String</span><span class="sxs-lookup"><span data-stu-id="c6db7-119">String</span></span>|<span data-ttu-id="c6db7-120">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="c6db7-120">The resource GUID for the security object is not valid.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6db7-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c6db7-121">Relationships</span></span>
<span data-ttu-id="c6db7-122">Keine</span><span class="sxs-lookup"><span data-stu-id="c6db7-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6db7-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c6db7-123">JSON Representation</span></span>
<span data-ttu-id="c6db7-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c6db7-124">Here is a JSON representation of the resource.</span></span>
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



