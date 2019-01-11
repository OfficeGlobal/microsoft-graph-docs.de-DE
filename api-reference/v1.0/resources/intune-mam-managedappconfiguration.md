---
title: managedAppConfiguration-Ressourcentyp
description: Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b3acf921f76e34e21427364ef84d1647cc7d0f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861320"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="b451f-103">managedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b451f-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="b451f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b451f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b451f-105">Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.</span><span class="sxs-lookup"><span data-stu-id="b451f-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="b451f-106">Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b451f-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b451f-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="b451f-107">Methods</span></span>
|<span data-ttu-id="b451f-108">Methode</span><span class="sxs-lookup"><span data-stu-id="b451f-108">Method</span></span>|<span data-ttu-id="b451f-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b451f-109">Return Type</span></span>|<span data-ttu-id="b451f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b451f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b451f-111">managedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="b451f-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="b451f-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b451f-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="b451f-113">Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="b451f-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b451f-114">managedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="b451f-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="b451f-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b451f-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="b451f-116">Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b451f-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b451f-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b451f-117">Properties</span></span>
|<span data-ttu-id="b451f-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b451f-118">Property</span></span>|<span data-ttu-id="b451f-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b451f-119">Type</span></span>|<span data-ttu-id="b451f-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b451f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b451f-121">displayName</span><span class="sxs-lookup"><span data-stu-id="b451f-121">displayName</span></span>|<span data-ttu-id="b451f-122">String</span><span class="sxs-lookup"><span data-stu-id="b451f-122">String</span></span>|<span data-ttu-id="b451f-123">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b451f-123">Policy display name.</span></span> <span data-ttu-id="b451f-124">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b451f-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b451f-125">description</span><span class="sxs-lookup"><span data-stu-id="b451f-125">description</span></span>|<span data-ttu-id="b451f-126">String</span><span class="sxs-lookup"><span data-stu-id="b451f-126">String</span></span>|<span data-ttu-id="b451f-127">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b451f-127">The policy's description.</span></span> <span data-ttu-id="b451f-128">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b451f-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b451f-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b451f-129">createdDateTime</span></span>|<span data-ttu-id="b451f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b451f-130">DateTimeOffset</span></span>|<span data-ttu-id="b451f-131">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b451f-131">The date and time the policy was created.</span></span> <span data-ttu-id="b451f-132">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b451f-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b451f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b451f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b451f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b451f-134">DateTimeOffset</span></span>|<span data-ttu-id="b451f-135">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b451f-135">Last time the policy was modified.</span></span> <span data-ttu-id="b451f-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b451f-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b451f-137">id</span><span class="sxs-lookup"><span data-stu-id="b451f-137">id</span></span>|<span data-ttu-id="b451f-138">String</span><span class="sxs-lookup"><span data-stu-id="b451f-138">String</span></span>|<span data-ttu-id="b451f-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b451f-139">Key of the entity.</span></span> <span data-ttu-id="b451f-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b451f-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b451f-141">Version</span><span class="sxs-lookup"><span data-stu-id="b451f-141">version</span></span>|<span data-ttu-id="b451f-142">String</span><span class="sxs-lookup"><span data-stu-id="b451f-142">String</span></span>|<span data-ttu-id="b451f-143">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="b451f-143">Version of the entity.</span></span> <span data-ttu-id="b451f-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b451f-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b451f-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="b451f-145">customSettings</span></span>|<span data-ttu-id="b451f-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b451f-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b451f-147">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.</span><span class="sxs-lookup"><span data-stu-id="b451f-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="b451f-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b451f-148">Relationships</span></span>
<span data-ttu-id="b451f-149">Keine</span><span class="sxs-lookup"><span data-stu-id="b451f-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b451f-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b451f-150">JSON Representation</span></span>
<span data-ttu-id="b451f-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b451f-151">Here is a JSON representation of the resource.</span></span>
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



