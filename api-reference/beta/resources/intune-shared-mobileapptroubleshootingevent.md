---
title: mobileAppTroubleshootingEvent-Ressourcentyp
description: Beschreibt die mobileAppTroubleshootingEvent-Ressource der Microsoft Graph-API für InTune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfa126fea86c7edb302953efc3b88376f2d68a09
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162944"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="27231-103">mobileAppTroubleshootingEvent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="27231-103">mobileAppTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="27231-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="27231-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27231-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="27231-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27231-106">Ereignis, das den Installationsstatus einer Benutzer-Geräteanwendung für die Geräteverwaltung und die Problembehandlung von Ereignis Workflows darstellt.</span><span class="sxs-lookup"><span data-stu-id="27231-106">Event representing a users device application install status for device management and troubleshooting event workflows.</span></span>

## <a name="methods"></a><span data-ttu-id="27231-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="27231-107">Methods</span></span>
|<span data-ttu-id="27231-108">Methode</span><span class="sxs-lookup"><span data-stu-id="27231-108">Method</span></span>|<span data-ttu-id="27231-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="27231-109">Return Type</span></span>|<span data-ttu-id="27231-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27231-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27231-111">MobileAppTroubleshootingEvents aufListen</span><span class="sxs-lookup"><span data-stu-id="27231-111">List mobileAppTroubleshootingEvents</span></span>](../api/intune-shared-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="27231-112">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="27231-112">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="27231-113">AufListen von Eigenschaften und Beziehungen der [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="27231-113">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="27231-114">MobileAppTroubleshootingEvent abrufen</span><span class="sxs-lookup"><span data-stu-id="27231-114">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[<span data-ttu-id="27231-115">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="27231-115">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="27231-116">Lesen von Eigenschaften und Beziehungen des [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="27231-116">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="27231-117">MobileAppTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="27231-117">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[<span data-ttu-id="27231-118">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="27231-118">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="27231-119">Erstellen eines neuen [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="27231-119">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="27231-120">MobileAppTroubleshootingEvent löschen</span><span class="sxs-lookup"><span data-stu-id="27231-120">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="27231-121">Keine</span><span class="sxs-lookup"><span data-stu-id="27231-121">None</span></span>|<span data-ttu-id="27231-122">Löscht eine [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="27231-122">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="27231-123">MobileAppTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="27231-123">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[<span data-ttu-id="27231-124">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="27231-124">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="27231-125">Aktualisieren der Eigenschaften eines [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="27231-125">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27231-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27231-126">Properties</span></span>
|<span data-ttu-id="27231-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27231-127">Property</span></span>|<span data-ttu-id="27231-128">Typ</span><span class="sxs-lookup"><span data-stu-id="27231-128">Type</span></span>|<span data-ttu-id="27231-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27231-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27231-130">id</span><span class="sxs-lookup"><span data-stu-id="27231-130">id</span></span>|<span data-ttu-id="27231-131">string</span><span class="sxs-lookup"><span data-stu-id="27231-131">String</span></span>|<span data-ttu-id="27231-132">UUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="27231-132">UUID for the object.</span></span>|
|<span data-ttu-id="27231-133">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="27231-133">**Troubleshooting**</span></span>|
|<span data-ttu-id="27231-134">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="27231-134">additionalInformation</span></span>|<span data-ttu-id="27231-135">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="27231-135">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="27231-136">Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen über das von [DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) geerbte Problem Behandlungs Ereignis bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="27231-136">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="27231-137">applicationId</span><span class="sxs-lookup"><span data-stu-id="27231-137">applicationId</span></span>|<span data-ttu-id="27231-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27231-138">String</span></span>|<span data-ttu-id="27231-139">InTune-Anwendungsbezeichner.</span><span class="sxs-lookup"><span data-stu-id="27231-139">Intune application identifier.</span></span>|
|<span data-ttu-id="27231-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="27231-140">correlationId</span></span>|<span data-ttu-id="27231-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27231-141">String</span></span>|<span data-ttu-id="27231-142">ID, die zum Nachverfolgen des Fehlers im Dienst verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="27231-142">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="27231-143">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="27231-143">eventDateTime</span></span>|<span data-ttu-id="27231-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27231-144">DateTimeOffset</span></span>|<span data-ttu-id="27231-145">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="27231-145">Time when the event occurred .</span></span> |
|<span data-ttu-id="27231-146">eventName</span><span class="sxs-lookup"><span data-stu-id="27231-146">eventName</span></span>|<span data-ttu-id="27231-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27231-147">String</span></span>|<span data-ttu-id="27231-148">Ereignis Name, der dem Problem Behandlungs Ereignis entspricht.</span><span class="sxs-lookup"><span data-stu-id="27231-148">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="27231-149">Optional</span><span class="sxs-lookup"><span data-stu-id="27231-149">Optional</span></span>|
|<span data-ttu-id="27231-150">Geschichte</span><span class="sxs-lookup"><span data-stu-id="27231-150">history</span></span>|<span data-ttu-id="27231-151">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="27231-151">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="27231-152">InTune-Problem Behandlungs Historie für mobile Anwendungen</span><span class="sxs-lookup"><span data-stu-id="27231-152">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="27231-153">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="27231-153">managedDeviceIdentifier</span></span>|<span data-ttu-id="27231-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27231-154">String</span></span>|<span data-ttu-id="27231-155">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="27231-155">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="27231-156">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="27231-156">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="27231-157">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="27231-157">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="27231-158">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="27231-158">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="27231-159">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="27231-159">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="27231-160">userId</span><span class="sxs-lookup"><span data-stu-id="27231-160">userId</span></span>|<span data-ttu-id="27231-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27231-161">String</span></span>|<span data-ttu-id="27231-162">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="27231-162">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27231-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="27231-163">Relationships</span></span>
|<span data-ttu-id="27231-164">Beziehung</span><span class="sxs-lookup"><span data-stu-id="27231-164">Relationship</span></span>|<span data-ttu-id="27231-165">Typ</span><span class="sxs-lookup"><span data-stu-id="27231-165">Type</span></span>|<span data-ttu-id="27231-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27231-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27231-167">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="27231-167">**Device management**</span></span>|
|<span data-ttu-id="27231-168">appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="27231-168">appLogCollectionRequests</span></span>|<span data-ttu-id="27231-169">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="27231-169">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection</span></span>|<span data-ttu-id="27231-170">Die Collection-Eigenschaft von AppLogUploadRequest.</span><span class="sxs-lookup"><span data-stu-id="27231-170">The collection property of AppLogUploadRequest.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="27231-171">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27231-171">JSON Representation</span></span>
<span data-ttu-id="27231-172">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27231-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```




