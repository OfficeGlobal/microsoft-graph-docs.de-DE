---
title: Ressourcentyp androidManagedStoreAppConfigurationSchemaItem
description: Konfiguration mit einem Element in einer Android Anwendung benutzerdefinierte Konfigurationsschema.
localization_priority: Normal
ms.openlocfilehash: 05bf7e945ef645368c4b421b2180e4f4c342ec69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886646"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="1d37f-103">Ressourcentyp androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="1d37f-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="1d37f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d37f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d37f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d37f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d37f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1d37f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d37f-107">Konfiguration mit einem Element in einer Android Anwendung benutzerdefinierte Konfigurationsschema.</span><span class="sxs-lookup"><span data-stu-id="1d37f-107">Single configuration item inside an Android application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="1d37f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1d37f-108">Properties</span></span>
|<span data-ttu-id="1d37f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d37f-109">Property</span></span>|<span data-ttu-id="1d37f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1d37f-110">Type</span></span>|<span data-ttu-id="1d37f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d37f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d37f-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="1d37f-112">schemaItemKey</span></span>|<span data-ttu-id="1d37f-113">String</span><span class="sxs-lookup"><span data-stu-id="1d37f-113">String</span></span>|<span data-ttu-id="1d37f-114">Eindeutiger Schlüssel, mit dem die Anwendung das Element identifiziert.</span><span class="sxs-lookup"><span data-stu-id="1d37f-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="1d37f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="1d37f-115">displayName</span></span>|<span data-ttu-id="1d37f-116">String</span><span class="sxs-lookup"><span data-stu-id="1d37f-116">String</span></span>|<span data-ttu-id="1d37f-117">Lesbarer Name</span><span class="sxs-lookup"><span data-stu-id="1d37f-117">Human readable name</span></span>|
|<span data-ttu-id="1d37f-118">description</span><span class="sxs-lookup"><span data-stu-id="1d37f-118">description</span></span>|<span data-ttu-id="1d37f-119">String</span><span class="sxs-lookup"><span data-stu-id="1d37f-119">String</span></span>|<span data-ttu-id="1d37f-120">Beschreibung dessen, was das Element innerhalb der Anwendung steuert.</span><span class="sxs-lookup"><span data-stu-id="1d37f-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="1d37f-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="1d37f-121">defaultBoolValue</span></span>|<span data-ttu-id="1d37f-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d37f-122">Boolean</span></span>|<span data-ttu-id="1d37f-123">Standardwert für boolesche Elemente, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="1d37f-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="1d37f-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="1d37f-124">defaultIntValue</span></span>|<span data-ttu-id="1d37f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1d37f-125">Int32</span></span>|<span data-ttu-id="1d37f-126">Standardwert für Elemente vom Typ Integer, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="1d37f-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="1d37f-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="1d37f-127">defaultStringValue</span></span>|<span data-ttu-id="1d37f-128">String</span><span class="sxs-lookup"><span data-stu-id="1d37f-128">String</span></span>|<span data-ttu-id="1d37f-129">Standardwert für Elemente vom Typ String, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="1d37f-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="1d37f-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="1d37f-130">defaultStringArrayValue</span></span>|<span data-ttu-id="1d37f-131">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1d37f-131">String collection</span></span>|<span data-ttu-id="1d37f-132">Standardwert für Elemente vom Typ String-Array, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="1d37f-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="1d37f-133">dataType</span><span class="sxs-lookup"><span data-stu-id="1d37f-133">dataType</span></span>|[<span data-ttu-id="1d37f-134">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="1d37f-134">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="1d37f-135">Der Typ der Wert, den dieses Element beschreibt.</span><span class="sxs-lookup"><span data-stu-id="1d37f-135">The type of value this item describes.</span></span> <span data-ttu-id="1d37f-136">Mögliche Werte sind: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray` und `hidden`.</span><span class="sxs-lookup"><span data-stu-id="1d37f-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="1d37f-137">selections</span><span class="sxs-lookup"><span data-stu-id="1d37f-137">selections</span></span>|<span data-ttu-id="1d37f-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1d37f-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="1d37f-139">Liste lesbarer Name-Wert-Paare für die gültigen Werte, die für dieses Element festgelegt werden können (nur Choice- und Multiselect-Elemente)</span><span class="sxs-lookup"><span data-stu-id="1d37f-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d37f-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1d37f-140">Relationships</span></span>
<span data-ttu-id="1d37f-141">Keine</span><span class="sxs-lookup"><span data-stu-id="1d37f-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d37f-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1d37f-142">JSON Representation</span></span>
<span data-ttu-id="1d37f-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1d37f-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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





