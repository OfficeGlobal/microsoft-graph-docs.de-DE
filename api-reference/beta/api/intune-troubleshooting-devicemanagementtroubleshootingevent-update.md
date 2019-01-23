---
title: deviceManagementTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementTroubleshootingEvent-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 935a5b835669a2d87fd761d8c62ccba537022f91
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415397"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="371b7-103">deviceManagementTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="371b7-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="371b7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="371b7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="371b7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="371b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="371b7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="371b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="371b7-107">Aktualisieren der Eigenschaften eines [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="371b7-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="371b7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="371b7-108">Prerequisites</span></span>
<span data-ttu-id="371b7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="371b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="371b7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="371b7-111">Permission type</span></span>|<span data-ttu-id="371b7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="371b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="371b7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="371b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="371b7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="371b7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="371b7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="371b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="371b7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="371b7-116">Not supported.</span></span>|
|<span data-ttu-id="371b7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="371b7-117">Application</span></span>|<span data-ttu-id="371b7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="371b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="371b7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="371b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="371b7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="371b7-120">Request headers</span></span>
|<span data-ttu-id="371b7-121">Header</span><span class="sxs-lookup"><span data-stu-id="371b7-121">Header</span></span>|<span data-ttu-id="371b7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="371b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="371b7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="371b7-123">Authorization</span></span>|<span data-ttu-id="371b7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="371b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="371b7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="371b7-125">Accept</span></span>|<span data-ttu-id="371b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="371b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="371b7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="371b7-127">Request body</span></span>
<span data-ttu-id="371b7-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="371b7-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="371b7-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="371b7-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="371b7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="371b7-130">Property</span></span>|<span data-ttu-id="371b7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="371b7-131">Type</span></span>|<span data-ttu-id="371b7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="371b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="371b7-133">id</span><span class="sxs-lookup"><span data-stu-id="371b7-133">id</span></span>|<span data-ttu-id="371b7-134">String</span><span class="sxs-lookup"><span data-stu-id="371b7-134">String</span></span>|<span data-ttu-id="371b7-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="371b7-135">UUID for the object</span></span>|
|<span data-ttu-id="371b7-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="371b7-136">eventDateTime</span></span>|<span data-ttu-id="371b7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="371b7-137">DateTimeOffset</span></span>|<span data-ttu-id="371b7-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="371b7-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="371b7-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="371b7-139">correlationId</span></span>|<span data-ttu-id="371b7-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="371b7-140">String</span></span>|<span data-ttu-id="371b7-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="371b7-141">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="371b7-142">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="371b7-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="371b7-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="371b7-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="371b7-144">Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.</span><span class="sxs-lookup"><span data-stu-id="371b7-144">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="371b7-145">Ereignisname</span><span class="sxs-lookup"><span data-stu-id="371b7-145">eventName</span></span>|<span data-ttu-id="371b7-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="371b7-146">String</span></span>|<span data-ttu-id="371b7-147">Name des Ereignisses, das Ereignis Problembehandlung entspricht.</span><span class="sxs-lookup"><span data-stu-id="371b7-147">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="371b7-148">Es ist ein optionales Feld</span><span class="sxs-lookup"><span data-stu-id="371b7-148">It is an Optional field</span></span>|
|<span data-ttu-id="371b7-149">zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="371b7-149">additionalInformation</span></span>|<span data-ttu-id="371b7-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="371b7-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="371b7-151">Eine Reihe von Schlüssel und String-Wert-Paare bietet zusätzliche Informationen für die Problembehandlung bei-Ereignis</span><span class="sxs-lookup"><span data-stu-id="371b7-151">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="371b7-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="371b7-152">Response</span></span>
<span data-ttu-id="371b7-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="371b7-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="371b7-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="371b7-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="371b7-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="371b7-155">Request</span></span>
<span data-ttu-id="371b7-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="371b7-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 852

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="371b7-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="371b7-157">Response</span></span>
<span data-ttu-id="371b7-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="371b7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 901

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```




