---
title: AppleVppTokenTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines appleVppTokenTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4885817ebef2149ee296a323f550e7793f210d44
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157876"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="26c42-103">AppleVppTokenTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="26c42-103">Update appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="26c42-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26c42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26c42-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="26c42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26c42-106">Aktualisieren der Eigenschaften eines [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="26c42-106">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26c42-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="26c42-107">Prerequisites</span></span>
<span data-ttu-id="26c42-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="26c42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="26c42-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26c42-110">Permission type</span></span>|<span data-ttu-id="26c42-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26c42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26c42-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26c42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26c42-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26c42-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="26c42-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26c42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26c42-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26c42-115">Not supported.</span></span>|
|<span data-ttu-id="26c42-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26c42-116">Application</span></span>|<span data-ttu-id="26c42-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26c42-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26c42-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26c42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="26c42-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26c42-119">Request headers</span></span>
|<span data-ttu-id="26c42-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="26c42-120">Header</span></span>|<span data-ttu-id="26c42-121">Wert</span><span class="sxs-lookup"><span data-stu-id="26c42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26c42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26c42-122">Authorization</span></span>|<span data-ttu-id="26c42-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="26c42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26c42-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="26c42-124">Accept</span></span>|<span data-ttu-id="26c42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26c42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26c42-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26c42-126">Request body</span></span>
<span data-ttu-id="26c42-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="26c42-127">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="26c42-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="26c42-128">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="26c42-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26c42-129">Property</span></span>|<span data-ttu-id="26c42-130">Typ</span><span class="sxs-lookup"><span data-stu-id="26c42-130">Type</span></span>|<span data-ttu-id="26c42-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26c42-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26c42-132">id</span><span class="sxs-lookup"><span data-stu-id="26c42-132">id</span></span>|<span data-ttu-id="26c42-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26c42-133">String</span></span>|<span data-ttu-id="26c42-134">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="26c42-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="26c42-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="26c42-135">eventDateTime</span></span>|<span data-ttu-id="26c42-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26c42-136">DateTimeOffset</span></span>|<span data-ttu-id="26c42-137">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="26c42-137">Time when the event occurred .</span></span> <span data-ttu-id="26c42-138">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="26c42-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="26c42-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="26c42-139">correlationId</span></span>|<span data-ttu-id="26c42-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26c42-140">String</span></span>|<span data-ttu-id="26c42-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="26c42-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="26c42-142">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="26c42-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="26c42-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="26c42-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="26c42-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="26c42-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="26c42-145">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="26c42-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="26c42-146">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="26c42-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="26c42-147">eventName</span><span class="sxs-lookup"><span data-stu-id="26c42-147">eventName</span></span>|<span data-ttu-id="26c42-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26c42-148">String</span></span>|<span data-ttu-id="26c42-149">Ereignis Name, der dem Problem Behandlungs Ereignis entspricht.</span><span class="sxs-lookup"><span data-stu-id="26c42-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="26c42-150">Es handelt sich um ein optionales Feld, geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="26c42-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="26c42-151">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="26c42-151">additionalInformation</span></span>|<span data-ttu-id="26c42-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="26c42-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="26c42-153">Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen über das von [DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) geerbte Problem Behandlungs Ereignis bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="26c42-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="26c42-154">Token-Nr.</span><span class="sxs-lookup"><span data-stu-id="26c42-154">tokenId</span></span>|<span data-ttu-id="26c42-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26c42-155">String</span></span>|<span data-ttu-id="26c42-156">Token-ID des Apple Volume Purchase programs.</span><span class="sxs-lookup"><span data-stu-id="26c42-156">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="26c42-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="26c42-157">Response</span></span>
<span data-ttu-id="26c42-158">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="26c42-158">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26c42-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26c42-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="26c42-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26c42-160">Request</span></span>
<span data-ttu-id="26c42-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26c42-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 881

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
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
  ],
  "tokenId": "Token Id value"
}
```

### <a name="response"></a><span data-ttu-id="26c42-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="26c42-162">Response</span></span>
<span data-ttu-id="26c42-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26c42-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 930

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
  "id": "09295f26-5f26-0929-265f-2909265f2909",
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
  ],
  "tokenId": "Token Id value"
}
```




