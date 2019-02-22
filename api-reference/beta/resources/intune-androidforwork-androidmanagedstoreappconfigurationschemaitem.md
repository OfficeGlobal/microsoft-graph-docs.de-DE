---
title: androidManagedStoreAppConfigurationSchemaItem-Ressourcentyp
description: Einzelnes Konfigurationselement innerhalb des benutzerdefinierten Konfigurationsschemas einer Android-Anwendung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8acd3dc2eddbab3433c30289a8273fd8ca397848
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169202"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="f42a8-103">androidManagedStoreAppConfigurationSchemaItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f42a8-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="f42a8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f42a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f42a8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f42a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f42a8-106">Einzelnes Konfigurationselement innerhalb des benutzerdefinierten Konfigurationsschemas einer Android-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="f42a8-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="f42a8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f42a8-107">Properties</span></span>
|<span data-ttu-id="f42a8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f42a8-108">Property</span></span>|<span data-ttu-id="f42a8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f42a8-109">Type</span></span>|<span data-ttu-id="f42a8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f42a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f42a8-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="f42a8-111">schemaItemKey</span></span>|<span data-ttu-id="f42a8-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f42a8-112">String</span></span>|<span data-ttu-id="f42a8-113">Eindeutiger Schlüssel, mit dem die Anwendung das Element identifiziert.</span><span class="sxs-lookup"><span data-stu-id="f42a8-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="f42a8-114">displayName</span><span class="sxs-lookup"><span data-stu-id="f42a8-114">displayName</span></span>|<span data-ttu-id="f42a8-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f42a8-115">String</span></span>|<span data-ttu-id="f42a8-116">Lesbarer Name</span><span class="sxs-lookup"><span data-stu-id="f42a8-116">Human readable name</span></span>|
|<span data-ttu-id="f42a8-117">description</span><span class="sxs-lookup"><span data-stu-id="f42a8-117">description</span></span>|<span data-ttu-id="f42a8-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f42a8-118">String</span></span>|<span data-ttu-id="f42a8-119">Beschreibung dessen, was das Element innerhalb der Anwendung steuert.</span><span class="sxs-lookup"><span data-stu-id="f42a8-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="f42a8-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="f42a8-120">defaultBoolValue</span></span>|<span data-ttu-id="f42a8-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f42a8-121">Boolean</span></span>|<span data-ttu-id="f42a8-122">Standardwert für boolesche Elemente, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="f42a8-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f42a8-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="f42a8-123">defaultIntValue</span></span>|<span data-ttu-id="f42a8-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f42a8-124">Int32</span></span>|<span data-ttu-id="f42a8-125">Standardwert für Elemente vom Typ Integer, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="f42a8-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f42a8-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="f42a8-126">defaultStringValue</span></span>|<span data-ttu-id="f42a8-127">String</span><span class="sxs-lookup"><span data-stu-id="f42a8-127">String</span></span>|<span data-ttu-id="f42a8-128">Standardwert für Elemente vom Typ String, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="f42a8-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f42a8-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="f42a8-129">defaultStringArrayValue</span></span>|<span data-ttu-id="f42a8-130">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f42a8-130">String collection</span></span>|<span data-ttu-id="f42a8-131">Standardwert für Elemente vom Typ String-Array, wenn vom App-Entwickler angegeben.</span><span class="sxs-lookup"><span data-stu-id="f42a8-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="f42a8-132">dataType</span><span class="sxs-lookup"><span data-stu-id="f42a8-132">dataType</span></span>|[<span data-ttu-id="f42a8-133">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="f42a8-133">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="f42a8-134">Der Typ des Werts, der in diesem Element beschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="f42a8-134">The type of value this item describes.</span></span> <span data-ttu-id="f42a8-135">Mögliche Werte sind: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray` und `hidden`.</span><span class="sxs-lookup"><span data-stu-id="f42a8-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="f42a8-136">selections</span><span class="sxs-lookup"><span data-stu-id="f42a8-136">selections</span></span>|<span data-ttu-id="f42a8-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f42a8-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f42a8-138">Liste lesbarer Name-Wert-Paare für die gültigen Werte, die für dieses Element festgelegt werden können (nur Choice- und Multiselect-Elemente)</span><span class="sxs-lookup"><span data-stu-id="f42a8-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f42a8-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f42a8-139">Relationships</span></span>
<span data-ttu-id="f42a8-140">Keine</span><span class="sxs-lookup"><span data-stu-id="f42a8-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f42a8-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f42a8-141">JSON Representation</span></span>
<span data-ttu-id="f42a8-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f42a8-142">Here is a JSON representation of the resource.</span></span>
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




