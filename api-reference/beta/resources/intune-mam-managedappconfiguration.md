---
title: managedAppConfiguration-Ressourcentyp
description: Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3c8db1f356890dc478833e7b77267a218f08bbc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148083"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="732d7-103">managedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="732d7-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="732d7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="732d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="732d7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="732d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="732d7-106">Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.</span><span class="sxs-lookup"><span data-stu-id="732d7-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="732d7-107">Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="732d7-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="732d7-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="732d7-108">Methods</span></span>
|<span data-ttu-id="732d7-109">Methode</span><span class="sxs-lookup"><span data-stu-id="732d7-109">Method</span></span>|<span data-ttu-id="732d7-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="732d7-110">Return Type</span></span>|<span data-ttu-id="732d7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="732d7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="732d7-112">managedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="732d7-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="732d7-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="732d7-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="732d7-114">Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="732d7-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="732d7-115">managedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="732d7-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="732d7-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="732d7-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="732d7-117">Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="732d7-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="732d7-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="732d7-118">Properties</span></span>
|<span data-ttu-id="732d7-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="732d7-119">Property</span></span>|<span data-ttu-id="732d7-120">Typ</span><span class="sxs-lookup"><span data-stu-id="732d7-120">Type</span></span>|<span data-ttu-id="732d7-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="732d7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="732d7-122">displayName</span><span class="sxs-lookup"><span data-stu-id="732d7-122">displayName</span></span>|<span data-ttu-id="732d7-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="732d7-123">String</span></span>|<span data-ttu-id="732d7-124">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="732d7-124">Policy display name.</span></span> <span data-ttu-id="732d7-125">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="732d7-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="732d7-126">description</span><span class="sxs-lookup"><span data-stu-id="732d7-126">description</span></span>|<span data-ttu-id="732d7-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="732d7-127">String</span></span>|<span data-ttu-id="732d7-128">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="732d7-128">The policy's description.</span></span> <span data-ttu-id="732d7-129">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="732d7-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="732d7-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="732d7-130">createdDateTime</span></span>|<span data-ttu-id="732d7-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732d7-131">DateTimeOffset</span></span>|<span data-ttu-id="732d7-132">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="732d7-132">The date and time the policy was created.</span></span> <span data-ttu-id="732d7-133">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="732d7-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="732d7-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="732d7-134">lastModifiedDateTime</span></span>|<span data-ttu-id="732d7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732d7-135">DateTimeOffset</span></span>|<span data-ttu-id="732d7-136">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="732d7-136">Last time the policy was modified.</span></span> <span data-ttu-id="732d7-137">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="732d7-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="732d7-138">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="732d7-138">roleScopeTagIds</span></span>|<span data-ttu-id="732d7-139">String collection</span><span class="sxs-lookup"><span data-stu-id="732d7-139">String collection</span></span>|<span data-ttu-id="732d7-140">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="732d7-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="732d7-141">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="732d7-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="732d7-142">id</span><span class="sxs-lookup"><span data-stu-id="732d7-142">id</span></span>|<span data-ttu-id="732d7-143">string</span><span class="sxs-lookup"><span data-stu-id="732d7-143">String</span></span>|<span data-ttu-id="732d7-144">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="732d7-144">Key of the entity.</span></span> <span data-ttu-id="732d7-145">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="732d7-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="732d7-146">Version</span><span class="sxs-lookup"><span data-stu-id="732d7-146">version</span></span>|<span data-ttu-id="732d7-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="732d7-147">String</span></span>|<span data-ttu-id="732d7-148">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="732d7-148">Version of the entity.</span></span> <span data-ttu-id="732d7-149">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="732d7-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="732d7-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="732d7-150">customSettings</span></span>|<span data-ttu-id="732d7-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="732d7-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="732d7-152">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.</span><span class="sxs-lookup"><span data-stu-id="732d7-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="732d7-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="732d7-153">Relationships</span></span>
<span data-ttu-id="732d7-154">Keine</span><span class="sxs-lookup"><span data-stu-id="732d7-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="732d7-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="732d7-155">JSON Representation</span></span>
<span data-ttu-id="732d7-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="732d7-156">Here is a JSON representation of the resource.</span></span>
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




