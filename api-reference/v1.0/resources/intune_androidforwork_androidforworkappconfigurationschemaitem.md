# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="36b7d-101">androidForWorkAppConfigurationSchemaItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="36b7d-101">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="36b7d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="36b7d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36b7d-103">Einzelnes Konfigurationselement in einem benutzerdefinierten Konfigurationsschema einer Android for Work-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="36b7d-103">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="36b7d-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="36b7d-104">Properties</span></span>
|<span data-ttu-id="36b7d-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36b7d-105">Property</span></span>|<span data-ttu-id="36b7d-106">Typ</span><span class="sxs-lookup"><span data-stu-id="36b7d-106">Type</span></span>|<span data-ttu-id="36b7d-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36b7d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36b7d-108">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="36b7d-108">schemaItemKey</span></span>|<span data-ttu-id="36b7d-109">String</span><span class="sxs-lookup"><span data-stu-id="36b7d-109">String</span></span>|<span data-ttu-id="36b7d-110">Eindeutiger Schlüssel, mit dem die Anwendung das Element identifiziert.</span><span class="sxs-lookup"><span data-stu-id="36b7d-110">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="36b7d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="36b7d-111">displayName</span></span>|<span data-ttu-id="36b7d-112">String</span><span class="sxs-lookup"><span data-stu-id="36b7d-112">String</span></span>|<span data-ttu-id="36b7d-113">Lesbarer Name</span><span class="sxs-lookup"><span data-stu-id="36b7d-113">Human readable name</span></span>|
|<span data-ttu-id="36b7d-114">description</span><span class="sxs-lookup"><span data-stu-id="36b7d-114">description</span></span>|<span data-ttu-id="36b7d-115">String</span><span class="sxs-lookup"><span data-stu-id="36b7d-115">String</span></span>|<span data-ttu-id="36b7d-116">Beschreibung dessen, was das Element innerhalb der Anwendung steuert.</span><span class="sxs-lookup"><span data-stu-id="36b7d-116">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="36b7d-117">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="36b7d-117">defaultBoolValue</span></span>|<span data-ttu-id="36b7d-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="36b7d-118">Boolean</span></span>|<span data-ttu-id="36b7d-119">Standardwert für boolesche Elemente, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="36b7d-119">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="36b7d-120">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="36b7d-120">defaultIntValue</span></span>|<span data-ttu-id="36b7d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="36b7d-121">Int32</span></span>|<span data-ttu-id="36b7d-122">Standardwert für Elemente vom Typ Integer, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="36b7d-122">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="36b7d-123">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="36b7d-123">defaultStringValue</span></span>|<span data-ttu-id="36b7d-124">String</span><span class="sxs-lookup"><span data-stu-id="36b7d-124">String</span></span>|<span data-ttu-id="36b7d-125">Standardwert für Elemente vom Typ String, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="36b7d-125">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="36b7d-126">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="36b7d-126">defaultStringArrayValue</span></span>|<span data-ttu-id="36b7d-127">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="36b7d-127">String collection</span></span>|<span data-ttu-id="36b7d-128">Standardwert für Elemente vom Typ String-Array, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="36b7d-128">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="36b7d-129">dataType</span><span class="sxs-lookup"><span data-stu-id="36b7d-129">DataType</span></span>|<span data-ttu-id="36b7d-130">String</span><span class="sxs-lookup"><span data-stu-id="36b7d-130">String</span></span>|<span data-ttu-id="36b7d-131">Der Typ des Werts, den dieses Element beschreibt. Mögliche Werte: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="36b7d-131">The type of value this item describes Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="36b7d-132">selections</span><span class="sxs-lookup"><span data-stu-id="36b7d-132">selections</span></span>|<span data-ttu-id="36b7d-133">[keyValuePair](../resources/intune_androidforwork_keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="36b7d-133">[keyValuePair](../resources/intune_androidforwork_keyvaluepair.md) collection</span></span>|<span data-ttu-id="36b7d-134">Liste lesbarer Name-Wert-Paare für die gültigen Werte, die für dieses Element festgelegt werden können (nur Choice- und Multiselect-Elemente)</span><span class="sxs-lookup"><span data-stu-id="36b7d-134">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="36b7d-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="36b7d-135">Relationships</span></span>
<span data-ttu-id="36b7d-136">Keine</span><span class="sxs-lookup"><span data-stu-id="36b7d-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="36b7d-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="36b7d-137">JSON Representation</span></span>
<span data-ttu-id="36b7d-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="36b7d-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



