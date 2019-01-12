---
title: managedAppConfiguration-Ressourcentyp
description: Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2bf4e8ce0d32bea7714ae489167dbb582043fa5a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936634"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="7bd43-103">managedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7bd43-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="7bd43-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7bd43-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bd43-105">Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.</span><span class="sxs-lookup"><span data-stu-id="7bd43-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="7bd43-106">Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bd43-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7bd43-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="7bd43-107">Methods</span></span>
|<span data-ttu-id="7bd43-108">Methode</span><span class="sxs-lookup"><span data-stu-id="7bd43-108">Method</span></span>|<span data-ttu-id="7bd43-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7bd43-109">Return Type</span></span>|<span data-ttu-id="7bd43-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bd43-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7bd43-111">managedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="7bd43-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="7bd43-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7bd43-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="7bd43-113">Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="7bd43-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7bd43-114">managedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="7bd43-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="7bd43-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7bd43-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="7bd43-116">Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7bd43-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7bd43-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7bd43-117">Properties</span></span>
|<span data-ttu-id="7bd43-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7bd43-118">Property</span></span>|<span data-ttu-id="7bd43-119">Typ</span><span class="sxs-lookup"><span data-stu-id="7bd43-119">Type</span></span>|<span data-ttu-id="7bd43-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bd43-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bd43-121">displayName</span><span class="sxs-lookup"><span data-stu-id="7bd43-121">displayName</span></span>|<span data-ttu-id="7bd43-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7bd43-122">String</span></span>|<span data-ttu-id="7bd43-123">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="7bd43-123">Policy display name.</span></span> <span data-ttu-id="7bd43-124">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bd43-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7bd43-125">description</span><span class="sxs-lookup"><span data-stu-id="7bd43-125">description</span></span>|<span data-ttu-id="7bd43-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7bd43-126">String</span></span>|<span data-ttu-id="7bd43-127">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="7bd43-127">The policy's description.</span></span> <span data-ttu-id="7bd43-128">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bd43-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7bd43-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7bd43-129">createdDateTime</span></span>|<span data-ttu-id="7bd43-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bd43-130">DateTimeOffset</span></span>|<span data-ttu-id="7bd43-131">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="7bd43-131">The date and time the policy was created.</span></span> <span data-ttu-id="7bd43-132">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bd43-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7bd43-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bd43-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7bd43-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bd43-134">DateTimeOffset</span></span>|<span data-ttu-id="7bd43-135">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="7bd43-135">Last time the policy was modified.</span></span> <span data-ttu-id="7bd43-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bd43-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7bd43-137">id</span><span class="sxs-lookup"><span data-stu-id="7bd43-137">id</span></span>|<span data-ttu-id="7bd43-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7bd43-138">String</span></span>|<span data-ttu-id="7bd43-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7bd43-139">Key of the entity.</span></span> <span data-ttu-id="7bd43-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bd43-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7bd43-141">Version</span><span class="sxs-lookup"><span data-stu-id="7bd43-141">version</span></span>|<span data-ttu-id="7bd43-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7bd43-142">String</span></span>|<span data-ttu-id="7bd43-143">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="7bd43-143">Version of the entity.</span></span> <span data-ttu-id="7bd43-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bd43-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7bd43-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="7bd43-145">customSettings</span></span>|<span data-ttu-id="7bd43-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7bd43-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7bd43-147">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.</span><span class="sxs-lookup"><span data-stu-id="7bd43-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bd43-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7bd43-148">Relationships</span></span>
<span data-ttu-id="7bd43-149">Keine</span><span class="sxs-lookup"><span data-stu-id="7bd43-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7bd43-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7bd43-150">JSON Representation</span></span>
<span data-ttu-id="7bd43-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7bd43-151">Here is a JSON representation of the resource.</span></span>
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



