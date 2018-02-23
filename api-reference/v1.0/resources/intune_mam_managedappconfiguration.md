# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="d59d1-101">managedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d59d1-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="d59d1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d59d1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d59d1-103">Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.</span><span class="sxs-lookup"><span data-stu-id="d59d1-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="d59d1-104">Erbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d59d1-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d59d1-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d59d1-105">Methods</span></span>
|<span data-ttu-id="d59d1-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d59d1-106">Method</span></span>|<span data-ttu-id="d59d1-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d59d1-107">Return Type</span></span>|<span data-ttu-id="d59d1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d59d1-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d59d1-109">managedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="d59d1-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="d59d1-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d59d1-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="d59d1-111">Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="d59d1-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d59d1-112">managedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="d59d1-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="d59d1-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d59d1-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="d59d1-114">Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d59d1-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d59d1-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d59d1-115">Properties</span></span>
|<span data-ttu-id="d59d1-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d59d1-116">Property</span></span>|<span data-ttu-id="d59d1-117">Typ</span><span class="sxs-lookup"><span data-stu-id="d59d1-117">Type</span></span>|<span data-ttu-id="d59d1-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d59d1-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d59d1-119">displayName</span><span class="sxs-lookup"><span data-stu-id="d59d1-119">displayName</span></span>|<span data-ttu-id="d59d1-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d59d1-120">String</span></span>|<span data-ttu-id="d59d1-121">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d59d1-121">Policy display name.</span></span> <span data-ttu-id="d59d1-122">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d59d1-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d59d1-123">description</span><span class="sxs-lookup"><span data-stu-id="d59d1-123">description</span></span>|<span data-ttu-id="d59d1-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d59d1-124">String</span></span>|<span data-ttu-id="d59d1-125">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d59d1-125">The policy's description.</span></span> <span data-ttu-id="d59d1-126">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d59d1-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d59d1-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d59d1-127">createdDateTime</span></span>|<span data-ttu-id="d59d1-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d59d1-128">DateTimeOffset</span></span>|<span data-ttu-id="d59d1-129">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d59d1-129">The date and time the group was created.</span></span> <span data-ttu-id="d59d1-130">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d59d1-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d59d1-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d59d1-131">lastModifiedDateTime</span></span>|<span data-ttu-id="d59d1-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d59d1-132">DateTimeOffset</span></span>|<span data-ttu-id="d59d1-133">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d59d1-133">Last time the policy was modified.</span></span> <span data-ttu-id="d59d1-134">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d59d1-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d59d1-135">id</span><span class="sxs-lookup"><span data-stu-id="d59d1-135">id</span></span>|<span data-ttu-id="d59d1-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d59d1-136">String</span></span>|<span data-ttu-id="d59d1-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d59d1-137">Key of the setting.</span></span> <span data-ttu-id="d59d1-138">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d59d1-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d59d1-139">Version</span><span class="sxs-lookup"><span data-stu-id="d59d1-139">version</span></span>|<span data-ttu-id="d59d1-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d59d1-140">String</span></span>|<span data-ttu-id="d59d1-141">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="d59d1-141">Version of the entity.</span></span> <span data-ttu-id="d59d1-142">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d59d1-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d59d1-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="d59d1-143">customSettings</span></span>|<span data-ttu-id="d59d1-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d59d1-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="d59d1-145">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.</span><span class="sxs-lookup"><span data-stu-id="d59d1-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="d59d1-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d59d1-146">Relationships</span></span>
<span data-ttu-id="d59d1-147">Keine</span><span class="sxs-lookup"><span data-stu-id="d59d1-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d59d1-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d59d1-148">JSON Representation</span></span>
<span data-ttu-id="d59d1-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d59d1-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



