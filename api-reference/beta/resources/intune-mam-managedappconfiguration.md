---
title: managedAppConfiguration-Ressourcentyp
description: Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67b445c5f7882bb4befc3e2c5cc46e26c5cf50fc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405674"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="ae922-103">managedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ae922-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="ae922-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ae922-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae922-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae922-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae922-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae922-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae922-107">Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.</span><span class="sxs-lookup"><span data-stu-id="ae922-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="ae922-108">Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ae922-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ae922-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="ae922-109">Methods</span></span>
|<span data-ttu-id="ae922-110">Methode</span><span class="sxs-lookup"><span data-stu-id="ae922-110">Method</span></span>|<span data-ttu-id="ae922-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ae922-111">Return Type</span></span>|<span data-ttu-id="ae922-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae922-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae922-113">managedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="ae922-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="ae922-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ae922-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="ae922-115">Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="ae922-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ae922-116">managedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="ae922-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="ae922-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae922-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="ae922-118">Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae922-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae922-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae922-119">Properties</span></span>
|<span data-ttu-id="ae922-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae922-120">Property</span></span>|<span data-ttu-id="ae922-121">Typ</span><span class="sxs-lookup"><span data-stu-id="ae922-121">Type</span></span>|<span data-ttu-id="ae922-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae922-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae922-123">displayName</span><span class="sxs-lookup"><span data-stu-id="ae922-123">displayName</span></span>|<span data-ttu-id="ae922-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae922-124">String</span></span>|<span data-ttu-id="ae922-125">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="ae922-125">Policy display name.</span></span> <span data-ttu-id="ae922-126">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ae922-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae922-127">description</span><span class="sxs-lookup"><span data-stu-id="ae922-127">description</span></span>|<span data-ttu-id="ae922-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae922-128">String</span></span>|<span data-ttu-id="ae922-129">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="ae922-129">The policy's description.</span></span> <span data-ttu-id="ae922-130">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ae922-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae922-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae922-131">createdDateTime</span></span>|<span data-ttu-id="ae922-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae922-132">DateTimeOffset</span></span>|<span data-ttu-id="ae922-133">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="ae922-133">The date and time the policy was created.</span></span> <span data-ttu-id="ae922-134">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ae922-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae922-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae922-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ae922-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae922-136">DateTimeOffset</span></span>|<span data-ttu-id="ae922-137">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="ae922-137">Last time the policy was modified.</span></span> <span data-ttu-id="ae922-138">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ae922-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae922-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae922-139">roleScopeTagIds</span></span>|<span data-ttu-id="ae922-140">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ae922-140">String collection</span></span>|<span data-ttu-id="ae922-141">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="ae922-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ae922-142">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ae922-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae922-143">id</span><span class="sxs-lookup"><span data-stu-id="ae922-143">id</span></span>|<span data-ttu-id="ae922-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae922-144">String</span></span>|<span data-ttu-id="ae922-145">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ae922-145">Key of the entity.</span></span> <span data-ttu-id="ae922-146">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ae922-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae922-147">Version</span><span class="sxs-lookup"><span data-stu-id="ae922-147">version</span></span>|<span data-ttu-id="ae922-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae922-148">String</span></span>|<span data-ttu-id="ae922-149">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="ae922-149">Version of the entity.</span></span> <span data-ttu-id="ae922-150">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ae922-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae922-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="ae922-151">customSettings</span></span>|<span data-ttu-id="ae922-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ae922-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ae922-153">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.</span><span class="sxs-lookup"><span data-stu-id="ae922-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae922-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ae922-154">Relationships</span></span>
<span data-ttu-id="ae922-155">Keine</span><span class="sxs-lookup"><span data-stu-id="ae922-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae922-156">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae922-156">JSON Representation</span></span>
<span data-ttu-id="ae922-157">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ae922-157">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
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




