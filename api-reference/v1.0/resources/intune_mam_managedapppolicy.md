# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="2efcd-101">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2efcd-101">managedAppPolicy resource type</span></span>

> <span data-ttu-id="2efcd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2efcd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2efcd-103">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="2efcd-103">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="2efcd-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="2efcd-104">Methods</span></span>
|<span data-ttu-id="2efcd-105">Methode</span><span class="sxs-lookup"><span data-stu-id="2efcd-105">Method</span></span>|<span data-ttu-id="2efcd-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2efcd-106">Return Type</span></span>|<span data-ttu-id="2efcd-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2efcd-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2efcd-108">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="2efcd-108">List managedAppPolicies</span></span>](../api/intune_mam_managedapppolicy_list.md)|<span data-ttu-id="2efcd-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2efcd-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="2efcd-110">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="2efcd-110">List properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="2efcd-111">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="2efcd-111">Get managedAppPolicy</span></span>](../api/intune_mam_managedapppolicy_get.md)|[<span data-ttu-id="2efcd-112">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2efcd-112">managedAppPolicy</span></span>](../resources/intune_mam_managedapppolicy.md)|<span data-ttu-id="2efcd-113">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2efcd-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="2efcd-114">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="2efcd-114">targetApps action</span></span>](../api/intune_mam_managedapppolicy_targetapps.md)|<span data-ttu-id="2efcd-115">Keine</span><span class="sxs-lookup"><span data-stu-id="2efcd-115">None</span></span>|<span data-ttu-id="2efcd-116">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="2efcd-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2efcd-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2efcd-117">Properties</span></span>
|<span data-ttu-id="2efcd-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2efcd-118">Property</span></span>|<span data-ttu-id="2efcd-119">Typ</span><span class="sxs-lookup"><span data-stu-id="2efcd-119">Type</span></span>|<span data-ttu-id="2efcd-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2efcd-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2efcd-121">displayName</span><span class="sxs-lookup"><span data-stu-id="2efcd-121">displayName</span></span>|<span data-ttu-id="2efcd-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2efcd-122">String</span></span>|<span data-ttu-id="2efcd-123">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2efcd-123">Policy display name.</span></span>|
|<span data-ttu-id="2efcd-124">description</span><span class="sxs-lookup"><span data-stu-id="2efcd-124">description</span></span>|<span data-ttu-id="2efcd-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2efcd-125">String</span></span>|<span data-ttu-id="2efcd-126">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2efcd-126">The policy's description.</span></span>|
|<span data-ttu-id="2efcd-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2efcd-127">createdDateTime</span></span>|<span data-ttu-id="2efcd-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2efcd-128">DateTimeOffset</span></span>|<span data-ttu-id="2efcd-129">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="2efcd-129">The date and time the group was created.</span></span>|
|<span data-ttu-id="2efcd-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2efcd-130">lastModifiedDateTime</span></span>|<span data-ttu-id="2efcd-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2efcd-131">DateTimeOffset</span></span>|<span data-ttu-id="2efcd-132">Das Datum und die Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="2efcd-132">Last time the policy was modified.</span></span>|
|<span data-ttu-id="2efcd-133">id</span><span class="sxs-lookup"><span data-stu-id="2efcd-133">id</span></span>|<span data-ttu-id="2efcd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2efcd-134">String</span></span>|<span data-ttu-id="2efcd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2efcd-135">Key of the setting.</span></span>|
|<span data-ttu-id="2efcd-136">version</span><span class="sxs-lookup"><span data-stu-id="2efcd-136">version</span></span>|<span data-ttu-id="2efcd-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2efcd-137">String</span></span>|<span data-ttu-id="2efcd-138">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="2efcd-138">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2efcd-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2efcd-139">Relationships</span></span>
<span data-ttu-id="2efcd-140">Keine</span><span class="sxs-lookup"><span data-stu-id="2efcd-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2efcd-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2efcd-141">JSON Representation</span></span>
<span data-ttu-id="2efcd-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2efcd-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



