---
title: AppleVppTokenTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines appleVppTokenTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ce92f73e3aaa8b9f7a1442e3088c221266ff299
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986537"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="58fbe-103">AppleVppTokenTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="58fbe-103">Update appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="58fbe-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58fbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58fbe-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="58fbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58fbe-106">Aktualisieren der Eigenschaften eines [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="58fbe-106">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58fbe-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58fbe-107">Prerequisites</span></span>
<span data-ttu-id="58fbe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58fbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58fbe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58fbe-110">Permission type</span></span>|<span data-ttu-id="58fbe-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58fbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58fbe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58fbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58fbe-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58fbe-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58fbe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58fbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58fbe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58fbe-115">Not supported.</span></span>|
|<span data-ttu-id="58fbe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58fbe-116">Application</span></span>|<span data-ttu-id="58fbe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58fbe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58fbe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58fbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="58fbe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58fbe-119">Request headers</span></span>
|<span data-ttu-id="58fbe-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58fbe-120">Header</span></span>|<span data-ttu-id="58fbe-121">Wert</span><span class="sxs-lookup"><span data-stu-id="58fbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58fbe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58fbe-122">Authorization</span></span>|<span data-ttu-id="58fbe-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58fbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58fbe-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="58fbe-124">Accept</span></span>|<span data-ttu-id="58fbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58fbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58fbe-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58fbe-126">Request body</span></span>
<span data-ttu-id="58fbe-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="58fbe-127">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="58fbe-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="58fbe-128">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="58fbe-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58fbe-129">Property</span></span>|<span data-ttu-id="58fbe-130">Typ</span><span class="sxs-lookup"><span data-stu-id="58fbe-130">Type</span></span>|<span data-ttu-id="58fbe-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58fbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58fbe-132">id</span><span class="sxs-lookup"><span data-stu-id="58fbe-132">id</span></span>|<span data-ttu-id="58fbe-133">String</span><span class="sxs-lookup"><span data-stu-id="58fbe-133">String</span></span>|<span data-ttu-id="58fbe-134">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="58fbe-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58fbe-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="58fbe-135">eventDateTime</span></span>|<span data-ttu-id="58fbe-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58fbe-136">DateTimeOffset</span></span>|<span data-ttu-id="58fbe-137">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="58fbe-137">Time when the event occurred .</span></span> <span data-ttu-id="58fbe-138">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="58fbe-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58fbe-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="58fbe-139">correlationId</span></span>|<span data-ttu-id="58fbe-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58fbe-140">String</span></span>|<span data-ttu-id="58fbe-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="58fbe-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="58fbe-142">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="58fbe-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58fbe-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="58fbe-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="58fbe-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="58fbe-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="58fbe-145">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="58fbe-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="58fbe-146">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="58fbe-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58fbe-147">eventName</span><span class="sxs-lookup"><span data-stu-id="58fbe-147">eventName</span></span>|<span data-ttu-id="58fbe-148">String</span><span class="sxs-lookup"><span data-stu-id="58fbe-148">String</span></span>|<span data-ttu-id="58fbe-149">Ereignis Name, der dem Problem Behandlungs Ereignis entspricht.</span><span class="sxs-lookup"><span data-stu-id="58fbe-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="58fbe-150">Es handelt sich um ein optionales Feld, geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="58fbe-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58fbe-151">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="58fbe-151">additionalInformation</span></span>|<span data-ttu-id="58fbe-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="58fbe-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="58fbe-153">Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen über das von [DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) geerbte Problem Behandlungs Ereignis bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="58fbe-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58fbe-154">Token-Nr.</span><span class="sxs-lookup"><span data-stu-id="58fbe-154">tokenId</span></span>|<span data-ttu-id="58fbe-155">String</span><span class="sxs-lookup"><span data-stu-id="58fbe-155">String</span></span>|<span data-ttu-id="58fbe-156">Token-ID des Apple Volume Purchase programs.</span><span class="sxs-lookup"><span data-stu-id="58fbe-156">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="58fbe-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="58fbe-157">Response</span></span>
<span data-ttu-id="58fbe-158">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="58fbe-158">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58fbe-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58fbe-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="58fbe-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58fbe-160">Request</span></span>
<span data-ttu-id="58fbe-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58fbe-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58fbe-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="58fbe-162">Response</span></span>
<span data-ttu-id="58fbe-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58fbe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




