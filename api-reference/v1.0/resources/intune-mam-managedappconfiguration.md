---
title: managedAppConfiguration-Ressourcentyp
description: Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.
ms.openlocfilehash: 42544aeacda4494a7757a15bef75a493d96fe0cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019906"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="9e2e6-103">managedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e2e6-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="9e2e6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9e2e6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e2e6-105">Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.</span><span class="sxs-lookup"><span data-stu-id="9e2e6-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="9e2e6-106">Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e2e6-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9e2e6-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="9e2e6-107">Methods</span></span>
|<span data-ttu-id="9e2e6-108">Methode</span><span class="sxs-lookup"><span data-stu-id="9e2e6-108">Method</span></span>|<span data-ttu-id="9e2e6-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9e2e6-109">Return Type</span></span>|<span data-ttu-id="9e2e6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e2e6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e2e6-111">managedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="9e2e6-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="9e2e6-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9e2e6-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="9e2e6-113">Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="9e2e6-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="9e2e6-114">managedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="9e2e6-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="9e2e6-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e2e6-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="9e2e6-116">Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9e2e6-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e2e6-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e2e6-117">Properties</span></span>
|<span data-ttu-id="9e2e6-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e2e6-118">Property</span></span>|<span data-ttu-id="9e2e6-119">Typ</span><span class="sxs-lookup"><span data-stu-id="9e2e6-119">Type</span></span>|<span data-ttu-id="9e2e6-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e2e6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e2e6-121">displayName</span><span class="sxs-lookup"><span data-stu-id="9e2e6-121">displayName</span></span>|<span data-ttu-id="9e2e6-122">String</span><span class="sxs-lookup"><span data-stu-id="9e2e6-122">String</span></span>|<span data-ttu-id="9e2e6-123">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="9e2e6-123">Policy display name.</span></span> <span data-ttu-id="9e2e6-124">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e2e6-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2e6-125">description</span><span class="sxs-lookup"><span data-stu-id="9e2e6-125">description</span></span>|<span data-ttu-id="9e2e6-126">String</span><span class="sxs-lookup"><span data-stu-id="9e2e6-126">String</span></span>|<span data-ttu-id="9e2e6-127">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="9e2e6-127">The policy's description.</span></span> <span data-ttu-id="9e2e6-128">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e2e6-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2e6-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e2e6-129">createdDateTime</span></span>|<span data-ttu-id="9e2e6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e2e6-130">DateTimeOffset</span></span>|<span data-ttu-id="9e2e6-131">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="9e2e6-131">The date and time the policy was created.</span></span> <span data-ttu-id="9e2e6-132">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e2e6-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2e6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e2e6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="9e2e6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e2e6-134">DateTimeOffset</span></span>|<span data-ttu-id="9e2e6-135">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="9e2e6-135">Last time the policy was modified.</span></span> <span data-ttu-id="9e2e6-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e2e6-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2e6-137">id</span><span class="sxs-lookup"><span data-stu-id="9e2e6-137">id</span></span>|<span data-ttu-id="9e2e6-138">String</span><span class="sxs-lookup"><span data-stu-id="9e2e6-138">String</span></span>|<span data-ttu-id="9e2e6-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9e2e6-139">Key of the entity.</span></span> <span data-ttu-id="9e2e6-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e2e6-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2e6-141">Version</span><span class="sxs-lookup"><span data-stu-id="9e2e6-141">version</span></span>|<span data-ttu-id="9e2e6-142">String</span><span class="sxs-lookup"><span data-stu-id="9e2e6-142">String</span></span>|<span data-ttu-id="9e2e6-143">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="9e2e6-143">Version of the entity.</span></span> <span data-ttu-id="9e2e6-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e2e6-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e2e6-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="9e2e6-145">customSettings</span></span>|<span data-ttu-id="9e2e6-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9e2e6-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9e2e6-147">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.</span><span class="sxs-lookup"><span data-stu-id="9e2e6-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e2e6-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e2e6-148">Relationships</span></span>
<span data-ttu-id="9e2e6-149">Keine</span><span class="sxs-lookup"><span data-stu-id="9e2e6-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e2e6-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e2e6-150">JSON Representation</span></span>
<span data-ttu-id="9e2e6-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e2e6-151">Here is a JSON representation of the resource.</span></span>
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



