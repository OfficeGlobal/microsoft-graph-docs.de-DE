# <a name="devicemanagement-resource-type"></a><span data-ttu-id="204e4-101">deviceManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="204e4-101">deviceManagement resource type</span></span>

> <span data-ttu-id="204e4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="204e4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="204e4-103">Die deviceManagement-Ressource stellt die Geräteentitäten der Sammlung eines Mandanten dar, die vorab in Intune bereitgestellt wurden, und die Registrierungsprofile, die Geräteidentitäten zugewiesen werden können, die eine Konfiguration der Vorabregistrierung unterstützen.</span><span class="sxs-lookup"><span data-stu-id="204e4-103">The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="204e4-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="204e4-104">Methods</span></span>
|<span data-ttu-id="204e4-105">Methode</span><span class="sxs-lookup"><span data-stu-id="204e4-105">Method</span></span>|<span data-ttu-id="204e4-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="204e4-106">Return Type</span></span>|<span data-ttu-id="204e4-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="204e4-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="204e4-108">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="204e4-108">Get deviceManagement</span></span>](../api/intune_corpenrollment_devicemanagement_get.md)|[<span data-ttu-id="204e4-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="204e4-109">deviceManagement</span></span>](../resources/intune_corpenrollment_devicemanagement.md)|<span data-ttu-id="204e4-110">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_corpenrollment_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="204e4-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_corpenrollment_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="204e4-111">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="204e4-111">Update deviceManagement</span></span>](../api/intune_corpenrollment_devicemanagement_update.md)|[<span data-ttu-id="204e4-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="204e4-112">deviceManagement</span></span>](../resources/intune_corpenrollment_devicemanagement.md)|<span data-ttu-id="204e4-113">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_corpenrollment_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="204e4-113">Update the properties of a [calendar](../resources/intune_corpenrollment_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="204e4-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="204e4-114">Properties</span></span>
|<span data-ttu-id="204e4-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="204e4-115">Property</span></span>|<span data-ttu-id="204e4-116">Typ</span><span class="sxs-lookup"><span data-stu-id="204e4-116">Type</span></span>|<span data-ttu-id="204e4-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="204e4-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="204e4-118">id</span><span class="sxs-lookup"><span data-stu-id="204e4-118">id</span></span>|<span data-ttu-id="204e4-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="204e4-119">String</span></span>|<span data-ttu-id="204e4-120">GUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="204e4-120">The resource GUID for the security object is not valid.</span></span>|

## <a name="relationships"></a><span data-ttu-id="204e4-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="204e4-121">Relationships</span></span>
<span data-ttu-id="204e4-122">Keine</span><span class="sxs-lookup"><span data-stu-id="204e4-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="204e4-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="204e4-123">JSON Representation</span></span>
<span data-ttu-id="204e4-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="204e4-124">Here is a JSON representation of the resource.</span></span>
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



