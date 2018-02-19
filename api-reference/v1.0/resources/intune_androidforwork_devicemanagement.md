# <a name="devicemanagement-resource-type"></a><span data-ttu-id="d0a47-101">deviceManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0a47-101">deviceManagement resource type</span></span>

> <span data-ttu-id="d0a47-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d0a47-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0a47-103">Singleton-Entität, die als Container für Android for Work-Einstellungsfunktionen unter der Geräteverwaltung dient.</span><span class="sxs-lookup"><span data-stu-id="d0a47-103">Singleton entity that acts as a container for Android for Work settings functionality under device management.</span></span>
## <a name="methods"></a><span data-ttu-id="d0a47-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="d0a47-104">Methods</span></span>
|<span data-ttu-id="d0a47-105">Methode</span><span class="sxs-lookup"><span data-stu-id="d0a47-105">Method</span></span>|<span data-ttu-id="d0a47-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d0a47-106">Return Type</span></span>|<span data-ttu-id="d0a47-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0a47-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0a47-108">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="d0a47-108">Get deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_get.md)|[<span data-ttu-id="d0a47-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d0a47-109">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="d0a47-110">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_androidforwork_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d0a47-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="d0a47-111">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d0a47-111">Update deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_update.md)|[<span data-ttu-id="d0a47-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d0a47-112">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="d0a47-113">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_androidforwork_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d0a47-113">Update the properties of a [calendar](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d0a47-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d0a47-114">Properties</span></span>
|<span data-ttu-id="d0a47-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0a47-115">Property</span></span>|<span data-ttu-id="d0a47-116">Typ</span><span class="sxs-lookup"><span data-stu-id="d0a47-116">Type</span></span>|<span data-ttu-id="d0a47-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0a47-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0a47-118">id</span><span class="sxs-lookup"><span data-stu-id="d0a47-118">id</span></span>|<span data-ttu-id="d0a47-119">String</span><span class="sxs-lookup"><span data-stu-id="d0a47-119">String</span></span>|<span data-ttu-id="d0a47-120">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d0a47-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0a47-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d0a47-121">Relationships</span></span>
|<span data-ttu-id="d0a47-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d0a47-122">Relationship</span></span>|<span data-ttu-id="d0a47-123">Typ</span><span class="sxs-lookup"><span data-stu-id="d0a47-123">Type</span></span>|<span data-ttu-id="d0a47-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0a47-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0a47-125">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="d0a47-125">androidForWorkSettings</span></span>|[<span data-ttu-id="d0a47-126">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="d0a47-126">androidForWorkSettings</span></span>](../resources/intune_androidforwork_androidforworksettings.md)|<span data-ttu-id="d0a47-127">Die Singleton-Entität mit Android for Work-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="d0a47-127">The singleton Android for Work settings entity.</span></span>|
|<span data-ttu-id="d0a47-128">androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="d0a47-128">androidForWorkAppConfigurationSchemas</span></span>|<span data-ttu-id="d0a47-129">[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d0a47-129">[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) collection</span></span>|<span data-ttu-id="d0a47-130">Android for Work-App – Konfigurationsschemaentitäten</span><span class="sxs-lookup"><span data-stu-id="d0a47-130">Android for Work app configuration schema entities.</span></span>|
|<span data-ttu-id="d0a47-131">androidForWorkEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="d0a47-131">androidForWorkEnrollmentProfiles</span></span>|<span data-ttu-id="d0a47-132">[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d0a47-132">[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) collection</span></span>|<span data-ttu-id="d0a47-133">Android for Work-Registrierungsprofilentitäten.</span><span class="sxs-lookup"><span data-stu-id="d0a47-133">Android for Work enrollment profile entities.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0a47-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d0a47-134">JSON Representation</span></span>
<span data-ttu-id="d0a47-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d0a47-135">Here is a JSON representation of the resource.</span></span>
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



