# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="b6715-101">managedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b6715-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="b6715-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b6715-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6715-103">Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.</span><span class="sxs-lookup"><span data-stu-id="b6715-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="b6715-104">Erbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6715-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b6715-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="b6715-105">Methods</span></span>
|<span data-ttu-id="b6715-106">Methode</span><span class="sxs-lookup"><span data-stu-id="b6715-106">Method</span></span>|<span data-ttu-id="b6715-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b6715-107">Return Type</span></span>|<span data-ttu-id="b6715-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6715-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b6715-109">managedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="b6715-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="b6715-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b6715-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="b6715-111">Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="b6715-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b6715-112">managedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="b6715-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="b6715-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6715-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="b6715-114">Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b6715-114">Read properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6715-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b6715-115">Properties</span></span>
|<span data-ttu-id="b6715-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b6715-116">Property</span></span>|<span data-ttu-id="b6715-117">Typ</span><span class="sxs-lookup"><span data-stu-id="b6715-117">Type</span></span>|<span data-ttu-id="b6715-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6715-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6715-119">displayName</span><span class="sxs-lookup"><span data-stu-id="b6715-119">displayName</span></span>|<span data-ttu-id="b6715-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6715-120">String</span></span>|<span data-ttu-id="b6715-121">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b6715-121">Policy display name.</span></span> <span data-ttu-id="b6715-122">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6715-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="b6715-123">description</span><span class="sxs-lookup"><span data-stu-id="b6715-123">description</span></span>|<span data-ttu-id="b6715-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6715-124">String</span></span>|<span data-ttu-id="b6715-125">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b6715-125">The policy's description.</span></span> <span data-ttu-id="b6715-126">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6715-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="b6715-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6715-127">createdDateTime</span></span>|<span data-ttu-id="b6715-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6715-128">DateTimeOffset</span></span>|<span data-ttu-id="b6715-129">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b6715-129">The date and time the policy was created.</span></span> <span data-ttu-id="b6715-130">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6715-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="b6715-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6715-131">lastModifiedDateTime</span></span>|<span data-ttu-id="b6715-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6715-132">DateTimeOffset</span></span>|<span data-ttu-id="b6715-133">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b6715-133">Last time the policy was modified.</span></span> <span data-ttu-id="b6715-134">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6715-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="b6715-135">id</span><span class="sxs-lookup"><span data-stu-id="b6715-135">id</span></span>|<span data-ttu-id="b6715-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6715-136">String</span></span>|<span data-ttu-id="b6715-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b6715-137">Key of the entity.</span></span> <span data-ttu-id="b6715-138">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6715-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="b6715-139">Version</span><span class="sxs-lookup"><span data-stu-id="b6715-139">version</span></span>|<span data-ttu-id="b6715-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6715-140">String</span></span>|<span data-ttu-id="b6715-141">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="b6715-141">Version of the entity.</span></span> <span data-ttu-id="b6715-142">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6715-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="b6715-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="b6715-143">customSettings</span></span>|<span data-ttu-id="b6715-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b6715-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="b6715-145">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.</span><span class="sxs-lookup"><span data-stu-id="b6715-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6715-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b6715-146">Relationships</span></span>
<span data-ttu-id="b6715-147">Keine</span><span class="sxs-lookup"><span data-stu-id="b6715-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b6715-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b6715-148">JSON Representation</span></span>
<span data-ttu-id="b6715-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b6715-149">Here is a JSON representation of the resource.</span></span>
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



