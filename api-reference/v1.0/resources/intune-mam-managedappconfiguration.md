---
title: managedAppConfiguration-Ressourcentyp
description: Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86c6ecdcad64ae38887370101f96106a9b3aa816
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250768"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="1b618-103">managedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1b618-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="1b618-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1b618-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b618-105">Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.</span><span class="sxs-lookup"><span data-stu-id="1b618-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="1b618-106">Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b618-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1b618-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="1b618-107">Methods</span></span>
|<span data-ttu-id="1b618-108">Methode</span><span class="sxs-lookup"><span data-stu-id="1b618-108">Method</span></span>|<span data-ttu-id="1b618-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1b618-109">Return Type</span></span>|<span data-ttu-id="1b618-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b618-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b618-111">managedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="1b618-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="1b618-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1b618-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="1b618-113">Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="1b618-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1b618-114">managedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="1b618-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="1b618-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b618-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="1b618-116">Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b618-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b618-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1b618-117">Properties</span></span>
|<span data-ttu-id="1b618-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b618-118">Property</span></span>|<span data-ttu-id="1b618-119">Typ</span><span class="sxs-lookup"><span data-stu-id="1b618-119">Type</span></span>|<span data-ttu-id="1b618-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b618-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b618-121">displayName</span><span class="sxs-lookup"><span data-stu-id="1b618-121">displayName</span></span>|<span data-ttu-id="1b618-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b618-122">String</span></span>|<span data-ttu-id="1b618-123">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="1b618-123">Policy display name.</span></span> <span data-ttu-id="1b618-124">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b618-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b618-125">description</span><span class="sxs-lookup"><span data-stu-id="1b618-125">description</span></span>|<span data-ttu-id="1b618-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b618-126">String</span></span>|<span data-ttu-id="1b618-127">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="1b618-127">The policy's description.</span></span> <span data-ttu-id="1b618-128">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b618-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b618-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b618-129">createdDateTime</span></span>|<span data-ttu-id="1b618-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b618-130">DateTimeOffset</span></span>|<span data-ttu-id="1b618-131">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="1b618-131">The date and time the policy was created.</span></span> <span data-ttu-id="1b618-132">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b618-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b618-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b618-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1b618-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b618-134">DateTimeOffset</span></span>|<span data-ttu-id="1b618-135">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="1b618-135">Last time the policy was modified.</span></span> <span data-ttu-id="1b618-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b618-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b618-137">id</span><span class="sxs-lookup"><span data-stu-id="1b618-137">id</span></span>|<span data-ttu-id="1b618-138">string</span><span class="sxs-lookup"><span data-stu-id="1b618-138">String</span></span>|<span data-ttu-id="1b618-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1b618-139">Key of the entity.</span></span> <span data-ttu-id="1b618-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b618-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b618-141">Version</span><span class="sxs-lookup"><span data-stu-id="1b618-141">version</span></span>|<span data-ttu-id="1b618-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b618-142">String</span></span>|<span data-ttu-id="1b618-143">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="1b618-143">Version of the entity.</span></span> <span data-ttu-id="1b618-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b618-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b618-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="1b618-145">customSettings</span></span>|<span data-ttu-id="1b618-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1b618-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="1b618-147">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.</span><span class="sxs-lookup"><span data-stu-id="1b618-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b618-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1b618-148">Relationships</span></span>
<span data-ttu-id="1b618-149">Keine</span><span class="sxs-lookup"><span data-stu-id="1b618-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b618-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1b618-150">JSON Representation</span></span>
<span data-ttu-id="1b618-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1b618-151">Here is a JSON representation of the resource.</span></span>
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



