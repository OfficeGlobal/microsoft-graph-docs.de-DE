---
title: deviceManagementTroubleshootingEvent erstellen
description: Erstellen eines neuen deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b838278d27dcf7349b570b51ba52c7211174b5fd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981027"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="a2ff6-103">deviceManagementTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="a2ff6-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="a2ff6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2ff6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2ff6-106">Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-106">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2ff6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a2ff6-107">Prerequisites</span></span>
<span data-ttu-id="a2ff6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2ff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2ff6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2ff6-110">Permission type</span></span>|<span data-ttu-id="a2ff6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2ff6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2ff6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2ff6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2ff6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ff6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a2ff6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2ff6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2ff6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2ff6-115">Not supported.</span></span>|
|<span data-ttu-id="a2ff6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2ff6-116">Application</span></span>|<span data-ttu-id="a2ff6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2ff6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2ff6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2ff6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="a2ff6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2ff6-119">Request headers</span></span>
|<span data-ttu-id="a2ff6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a2ff6-120">Header</span></span>|<span data-ttu-id="a2ff6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a2ff6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2ff6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2ff6-122">Authorization</span></span>|<span data-ttu-id="a2ff6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a2ff6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2ff6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a2ff6-124">Accept</span></span>|<span data-ttu-id="a2ff6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2ff6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2ff6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2ff6-126">Request body</span></span>
<span data-ttu-id="a2ff6-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-127">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="a2ff6-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-128">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="a2ff6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2ff6-129">Property</span></span>|<span data-ttu-id="a2ff6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a2ff6-130">Type</span></span>|<span data-ttu-id="a2ff6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2ff6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ff6-132">id</span><span class="sxs-lookup"><span data-stu-id="a2ff6-132">id</span></span>|<span data-ttu-id="a2ff6-133">String</span><span class="sxs-lookup"><span data-stu-id="a2ff6-133">String</span></span>|<span data-ttu-id="a2ff6-134">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="a2ff6-134">UUID for the object</span></span>|
|<span data-ttu-id="a2ff6-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ff6-135">eventDateTime</span></span>|<span data-ttu-id="a2ff6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ff6-136">DateTimeOffset</span></span>|<span data-ttu-id="a2ff6-137">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="a2ff6-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="a2ff6-138">correlationId</span></span>|<span data-ttu-id="a2ff6-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2ff6-139">String</span></span>|<span data-ttu-id="a2ff6-140">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-140">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="a2ff6-141">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a2ff6-141">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="a2ff6-142">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a2ff6-142">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="a2ff6-143">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-143">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="a2ff6-144">eventName</span><span class="sxs-lookup"><span data-stu-id="a2ff6-144">eventName</span></span>|<span data-ttu-id="a2ff6-145">String</span><span class="sxs-lookup"><span data-stu-id="a2ff6-145">String</span></span>|<span data-ttu-id="a2ff6-146">Ereignis Name, der dem Problem Behandlungs Ereignis entspricht.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-146">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="a2ff6-147">Es handelt sich um ein optionales Feld</span><span class="sxs-lookup"><span data-stu-id="a2ff6-147">It is an Optional field</span></span>|
|<span data-ttu-id="a2ff6-148">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="a2ff6-148">additionalInformation</span></span>|<span data-ttu-id="a2ff6-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a2ff6-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a2ff6-150">Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen zum Problem Behandlungs Ereignis enthalten.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-150">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="a2ff6-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2ff6-151">Response</span></span>
<span data-ttu-id="a2ff6-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-152">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2ff6-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2ff6-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2ff6-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2ff6-154">Request</span></span>
<span data-ttu-id="a2ff6-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="a2ff6-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2ff6-156">Response</span></span>
<span data-ttu-id="a2ff6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




