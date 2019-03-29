---
title: enrollmentTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f5e0941987ab2d41b53085471c3842e23c73c6e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984247"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="71f98-103">enrollmentTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="71f98-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="71f98-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71f98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71f98-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="71f98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71f98-106">Aktualisieren der Eigenschaften eines [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="71f98-106">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71f98-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71f98-107">Prerequisites</span></span>
<span data-ttu-id="71f98-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71f98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71f98-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71f98-110">Permission type</span></span>|<span data-ttu-id="71f98-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71f98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71f98-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71f98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71f98-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f98-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="71f98-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71f98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71f98-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71f98-115">Not supported.</span></span>|
|<span data-ttu-id="71f98-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71f98-116">Application</span></span>|<span data-ttu-id="71f98-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71f98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71f98-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71f98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="71f98-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71f98-119">Request headers</span></span>
|<span data-ttu-id="71f98-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71f98-120">Header</span></span>|<span data-ttu-id="71f98-121">Wert</span><span class="sxs-lookup"><span data-stu-id="71f98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71f98-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71f98-122">Authorization</span></span>|<span data-ttu-id="71f98-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71f98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71f98-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="71f98-124">Accept</span></span>|<span data-ttu-id="71f98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71f98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71f98-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71f98-126">Request body</span></span>
<span data-ttu-id="71f98-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="71f98-127">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="71f98-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="71f98-128">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="71f98-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71f98-129">Property</span></span>|<span data-ttu-id="71f98-130">Typ</span><span class="sxs-lookup"><span data-stu-id="71f98-130">Type</span></span>|<span data-ttu-id="71f98-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71f98-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71f98-132">id</span><span class="sxs-lookup"><span data-stu-id="71f98-132">id</span></span>|<span data-ttu-id="71f98-133">String</span><span class="sxs-lookup"><span data-stu-id="71f98-133">String</span></span>|<span data-ttu-id="71f98-134">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="71f98-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="71f98-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="71f98-135">eventDateTime</span></span>|<span data-ttu-id="71f98-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71f98-136">DateTimeOffset</span></span>|<span data-ttu-id="71f98-137">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="71f98-137">Time when the event occurred .</span></span> <span data-ttu-id="71f98-138">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="71f98-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="71f98-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="71f98-139">correlationId</span></span>|<span data-ttu-id="71f98-140">String</span><span class="sxs-lookup"><span data-stu-id="71f98-140">String</span></span>|<span data-ttu-id="71f98-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="71f98-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="71f98-142">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="71f98-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="71f98-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="71f98-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="71f98-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="71f98-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="71f98-145">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="71f98-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="71f98-146">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="71f98-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="71f98-147">eventName</span><span class="sxs-lookup"><span data-stu-id="71f98-147">eventName</span></span>|<span data-ttu-id="71f98-148">String</span><span class="sxs-lookup"><span data-stu-id="71f98-148">String</span></span>|<span data-ttu-id="71f98-149">Ereignis Name, der dem Problem Behandlungs Ereignis entspricht.</span><span class="sxs-lookup"><span data-stu-id="71f98-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="71f98-150">Es handelt sich um ein optionales Feld, geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="71f98-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="71f98-151">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="71f98-151">additionalInformation</span></span>|<span data-ttu-id="71f98-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="71f98-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="71f98-153">Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen über das von [DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) geerbte Problem Behandlungs Ereignis bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="71f98-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="71f98-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="71f98-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="71f98-155">String</span><span class="sxs-lookup"><span data-stu-id="71f98-155">String</span></span>|<span data-ttu-id="71f98-156">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="71f98-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="71f98-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="71f98-157">operatingSystem</span></span>|<span data-ttu-id="71f98-158">String</span><span class="sxs-lookup"><span data-stu-id="71f98-158">String</span></span>|<span data-ttu-id="71f98-159">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="71f98-159">Operating System.</span></span>|
|<span data-ttu-id="71f98-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="71f98-160">osVersion</span></span>|<span data-ttu-id="71f98-161">String</span><span class="sxs-lookup"><span data-stu-id="71f98-161">String</span></span>|<span data-ttu-id="71f98-162">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="71f98-162">OS Version.</span></span>|
|<span data-ttu-id="71f98-163">userId</span><span class="sxs-lookup"><span data-stu-id="71f98-163">userId</span></span>|<span data-ttu-id="71f98-164">String</span><span class="sxs-lookup"><span data-stu-id="71f98-164">String</span></span>|<span data-ttu-id="71f98-165">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="71f98-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="71f98-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="71f98-166">deviceId</span></span>|<span data-ttu-id="71f98-167">String</span><span class="sxs-lookup"><span data-stu-id="71f98-167">String</span></span>|<span data-ttu-id="71f98-168">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="71f98-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="71f98-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="71f98-169">enrollmentType</span></span>|[<span data-ttu-id="71f98-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="71f98-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="71f98-171">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="71f98-171">Type of the enrollment.</span></span> <span data-ttu-id="71f98-172">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="71f98-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="71f98-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="71f98-173">failureCategory</span></span>|[<span data-ttu-id="71f98-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="71f98-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="71f98-175">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="71f98-175">Highlevel failure category.</span></span> <span data-ttu-id="71f98-176">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="71f98-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="71f98-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="71f98-177">failureReason</span></span>|<span data-ttu-id="71f98-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="71f98-178">String</span></span>|<span data-ttu-id="71f98-179">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="71f98-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="71f98-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="71f98-180">Response</span></span>
<span data-ttu-id="71f98-181">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="71f98-181">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71f98-182">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71f98-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="71f98-183">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71f98-183">Request</span></span>
<span data-ttu-id="71f98-184">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71f98-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 1182

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
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
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```

### <a name="response"></a><span data-ttu-id="71f98-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="71f98-185">Response</span></span>
<span data-ttu-id="71f98-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71f98-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1231

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
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
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```




