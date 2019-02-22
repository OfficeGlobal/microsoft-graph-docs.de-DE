---
title: deviceManagementTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ad17f38f4f9f078c956045f9f29950105f3461f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174748"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="26309-103">deviceManagementTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="26309-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="26309-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26309-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26309-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="26309-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26309-106">Aktualisieren der Eigenschaften eines [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="26309-106">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26309-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="26309-107">Prerequisites</span></span>
<span data-ttu-id="26309-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="26309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="26309-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26309-110">Permission type</span></span>|<span data-ttu-id="26309-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26309-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26309-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26309-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26309-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26309-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="26309-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26309-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26309-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26309-115">Not supported.</span></span>|
|<span data-ttu-id="26309-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26309-116">Application</span></span>|<span data-ttu-id="26309-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26309-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26309-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26309-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="26309-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26309-119">Request headers</span></span>
|<span data-ttu-id="26309-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="26309-120">Header</span></span>|<span data-ttu-id="26309-121">Wert</span><span class="sxs-lookup"><span data-stu-id="26309-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26309-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26309-122">Authorization</span></span>|<span data-ttu-id="26309-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="26309-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26309-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="26309-124">Accept</span></span>|<span data-ttu-id="26309-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26309-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26309-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26309-126">Request body</span></span>
<span data-ttu-id="26309-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="26309-127">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="26309-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="26309-128">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="26309-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26309-129">Property</span></span>|<span data-ttu-id="26309-130">Typ</span><span class="sxs-lookup"><span data-stu-id="26309-130">Type</span></span>|<span data-ttu-id="26309-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26309-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26309-132">id</span><span class="sxs-lookup"><span data-stu-id="26309-132">id</span></span>|<span data-ttu-id="26309-133">String</span><span class="sxs-lookup"><span data-stu-id="26309-133">String</span></span>|<span data-ttu-id="26309-134">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="26309-134">UUID for the object</span></span>|
|<span data-ttu-id="26309-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="26309-135">eventDateTime</span></span>|<span data-ttu-id="26309-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26309-136">DateTimeOffset</span></span>|<span data-ttu-id="26309-137">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="26309-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="26309-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="26309-138">correlationId</span></span>|<span data-ttu-id="26309-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26309-139">String</span></span>|<span data-ttu-id="26309-140">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="26309-140">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="26309-141">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="26309-141">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="26309-142">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="26309-142">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="26309-143">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="26309-143">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="26309-144">eventName</span><span class="sxs-lookup"><span data-stu-id="26309-144">eventName</span></span>|<span data-ttu-id="26309-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26309-145">String</span></span>|<span data-ttu-id="26309-146">Ereignis Name, der dem Problem Behandlungs Ereignis entspricht.</span><span class="sxs-lookup"><span data-stu-id="26309-146">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="26309-147">Es handelt sich um ein optionales Feld</span><span class="sxs-lookup"><span data-stu-id="26309-147">It is an Optional field</span></span>|
|<span data-ttu-id="26309-148">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="26309-148">additionalInformation</span></span>|<span data-ttu-id="26309-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="26309-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="26309-150">Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen zum Problem Behandlungs Ereignis enthalten.</span><span class="sxs-lookup"><span data-stu-id="26309-150">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="26309-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="26309-151">Response</span></span>
<span data-ttu-id="26309-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26309-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26309-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26309-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="26309-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26309-154">Request</span></span>
<span data-ttu-id="26309-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26309-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26309-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="26309-156">Response</span></span>
<span data-ttu-id="26309-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26309-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




