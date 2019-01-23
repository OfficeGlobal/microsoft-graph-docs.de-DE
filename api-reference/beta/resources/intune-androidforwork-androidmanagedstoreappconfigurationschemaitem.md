---
title: Ressourcentyp androidManagedStoreAppConfigurationSchemaItem
description: Konfiguration mit einem Element in einer Android Anwendung benutzerdefinierte Konfigurationsschema.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a12c8f4dc0a07dbf74c92193ac73fdcfe9bfd883
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398919"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="ff15a-103">Ressourcentyp androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="ff15a-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="ff15a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ff15a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff15a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff15a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff15a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ff15a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff15a-107">Konfiguration mit einem Element in einer Android Anwendung benutzerdefinierte Konfigurationsschema.</span><span class="sxs-lookup"><span data-stu-id="ff15a-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="ff15a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ff15a-108">Properties</span></span>
|<span data-ttu-id="ff15a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff15a-109">Property</span></span>|<span data-ttu-id="ff15a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ff15a-110">Type</span></span>|<span data-ttu-id="ff15a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff15a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff15a-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="ff15a-112">schemaItemKey</span></span>|<span data-ttu-id="ff15a-113">String</span><span class="sxs-lookup"><span data-stu-id="ff15a-113">String</span></span>|<span data-ttu-id="ff15a-114">Eindeutiger Schlüssel, mit dem die Anwendung das Element identifiziert.</span><span class="sxs-lookup"><span data-stu-id="ff15a-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="ff15a-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ff15a-115">displayName</span></span>|<span data-ttu-id="ff15a-116">String</span><span class="sxs-lookup"><span data-stu-id="ff15a-116">String</span></span>|<span data-ttu-id="ff15a-117">Lesbarer Name</span><span class="sxs-lookup"><span data-stu-id="ff15a-117">Human readable name</span></span>|
|<span data-ttu-id="ff15a-118">description</span><span class="sxs-lookup"><span data-stu-id="ff15a-118">description</span></span>|<span data-ttu-id="ff15a-119">String</span><span class="sxs-lookup"><span data-stu-id="ff15a-119">String</span></span>|<span data-ttu-id="ff15a-120">Beschreibung dessen, was das Element innerhalb der Anwendung steuert.</span><span class="sxs-lookup"><span data-stu-id="ff15a-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="ff15a-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="ff15a-121">defaultBoolValue</span></span>|<span data-ttu-id="ff15a-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff15a-122">Boolean</span></span>|<span data-ttu-id="ff15a-123">Standardwert für boolesche Elemente, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="ff15a-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="ff15a-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="ff15a-124">defaultIntValue</span></span>|<span data-ttu-id="ff15a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ff15a-125">Int32</span></span>|<span data-ttu-id="ff15a-126">Standardwert für Elemente vom Typ Integer, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="ff15a-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="ff15a-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="ff15a-127">defaultStringValue</span></span>|<span data-ttu-id="ff15a-128">String</span><span class="sxs-lookup"><span data-stu-id="ff15a-128">String</span></span>|<span data-ttu-id="ff15a-129">Standardwert für Elemente vom Typ String, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="ff15a-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="ff15a-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="ff15a-130">defaultStringArrayValue</span></span>|<span data-ttu-id="ff15a-131">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ff15a-131">String collection</span></span>|<span data-ttu-id="ff15a-132">Standardwert für Elemente vom Typ String-Array, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="ff15a-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="ff15a-133">dataType</span><span class="sxs-lookup"><span data-stu-id="ff15a-133">dataType</span></span>|[<span data-ttu-id="ff15a-134">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="ff15a-134">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="ff15a-135">Der Typ der Wert, den dieses Element beschreibt.</span><span class="sxs-lookup"><span data-stu-id="ff15a-135">The type of value this item describes.</span></span> <span data-ttu-id="ff15a-136">Mögliche Werte sind: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray` und `hidden`.</span><span class="sxs-lookup"><span data-stu-id="ff15a-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="ff15a-137">selections</span><span class="sxs-lookup"><span data-stu-id="ff15a-137">selections</span></span>|<span data-ttu-id="ff15a-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ff15a-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ff15a-139">Liste lesbarer Name-Wert-Paare für die gültigen Werte, die für dieses Element festgelegt werden können (nur Choice- und Multiselect-Elemente)</span><span class="sxs-lookup"><span data-stu-id="ff15a-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff15a-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ff15a-140">Relationships</span></span>
<span data-ttu-id="ff15a-141">Keine</span><span class="sxs-lookup"><span data-stu-id="ff15a-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff15a-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ff15a-142">JSON Representation</span></span>
<span data-ttu-id="ff15a-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ff15a-143">Here is a JSON representation of the resource.</span></span>
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




