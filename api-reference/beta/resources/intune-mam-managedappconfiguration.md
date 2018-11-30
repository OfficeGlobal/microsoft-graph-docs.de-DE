---
title: managedAppConfiguration-Ressourcentyp
description: Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.
ms.openlocfilehash: 0f7007b0a94f8ca72d2357ca915550151cb0097b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065618"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="6ef23-103">managedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6ef23-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="6ef23-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ef23-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ef23-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ef23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ef23-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6ef23-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ef23-107">Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.</span><span class="sxs-lookup"><span data-stu-id="6ef23-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="6ef23-108">Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6ef23-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6ef23-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="6ef23-109">Methods</span></span>
|<span data-ttu-id="6ef23-110">Methode</span><span class="sxs-lookup"><span data-stu-id="6ef23-110">Method</span></span>|<span data-ttu-id="6ef23-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6ef23-111">Return Type</span></span>|<span data-ttu-id="6ef23-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ef23-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ef23-113">managedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="6ef23-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="6ef23-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ef23-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="6ef23-115">Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="6ef23-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6ef23-116">managedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="6ef23-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="6ef23-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ef23-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="6ef23-118">Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ef23-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ef23-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ef23-119">Properties</span></span>
|<span data-ttu-id="6ef23-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ef23-120">Property</span></span>|<span data-ttu-id="6ef23-121">Typ</span><span class="sxs-lookup"><span data-stu-id="6ef23-121">Type</span></span>|<span data-ttu-id="6ef23-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ef23-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ef23-123">displayName</span><span class="sxs-lookup"><span data-stu-id="6ef23-123">displayName</span></span>|<span data-ttu-id="6ef23-124">String</span><span class="sxs-lookup"><span data-stu-id="6ef23-124">String</span></span>|<span data-ttu-id="6ef23-125">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="6ef23-125">Policy display name.</span></span> <span data-ttu-id="6ef23-126">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6ef23-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6ef23-127">description</span><span class="sxs-lookup"><span data-stu-id="6ef23-127">description</span></span>|<span data-ttu-id="6ef23-128">String</span><span class="sxs-lookup"><span data-stu-id="6ef23-128">String</span></span>|<span data-ttu-id="6ef23-129">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="6ef23-129">The policy's description.</span></span> <span data-ttu-id="6ef23-130">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6ef23-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6ef23-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ef23-131">createdDateTime</span></span>|<span data-ttu-id="6ef23-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ef23-132">DateTimeOffset</span></span>|<span data-ttu-id="6ef23-133">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="6ef23-133">The date and time the policy was created.</span></span> <span data-ttu-id="6ef23-134">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6ef23-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6ef23-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ef23-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6ef23-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ef23-136">DateTimeOffset</span></span>|<span data-ttu-id="6ef23-137">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="6ef23-137">Last time the policy was modified.</span></span> <span data-ttu-id="6ef23-138">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6ef23-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6ef23-139">id</span><span class="sxs-lookup"><span data-stu-id="6ef23-139">id</span></span>|<span data-ttu-id="6ef23-140">String</span><span class="sxs-lookup"><span data-stu-id="6ef23-140">String</span></span>|<span data-ttu-id="6ef23-141">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6ef23-141">Key of the entity.</span></span> <span data-ttu-id="6ef23-142">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6ef23-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6ef23-143">Version</span><span class="sxs-lookup"><span data-stu-id="6ef23-143">version</span></span>|<span data-ttu-id="6ef23-144">String</span><span class="sxs-lookup"><span data-stu-id="6ef23-144">String</span></span>|<span data-ttu-id="6ef23-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="6ef23-145">Version of the entity.</span></span> <span data-ttu-id="6ef23-146">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6ef23-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6ef23-147">customSettings</span><span class="sxs-lookup"><span data-stu-id="6ef23-147">customSettings</span></span>|<span data-ttu-id="6ef23-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ef23-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6ef23-149">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.</span><span class="sxs-lookup"><span data-stu-id="6ef23-149">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ef23-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ef23-150">Relationships</span></span>
<span data-ttu-id="6ef23-151">Keine</span><span class="sxs-lookup"><span data-stu-id="6ef23-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ef23-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ef23-152">JSON Representation</span></span>
<span data-ttu-id="6ef23-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ef23-153">Here is a JSON representation of the resource.</span></span>
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





