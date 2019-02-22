---
title: EnrollmentTroubleshootingEvent erstellen
description: Erstellen eines neuen enrollmentTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 230bf0dd823c734620a296009939d82a2100914d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147516"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="b8202-103">EnrollmentTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="b8202-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="b8202-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8202-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8202-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8202-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8202-106">Erstellen eines neuen [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8202-106">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8202-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8202-107">Prerequisites</span></span>
<span data-ttu-id="b8202-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8202-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b8202-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8202-110">Permission type</span></span>|<span data-ttu-id="b8202-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8202-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8202-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8202-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8202-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8202-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b8202-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8202-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8202-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8202-115">Not supported.</span></span>|
|<span data-ttu-id="b8202-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8202-116">Application</span></span>|<span data-ttu-id="b8202-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8202-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8202-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8202-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="b8202-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8202-119">Request headers</span></span>
|<span data-ttu-id="b8202-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8202-120">Header</span></span>|<span data-ttu-id="b8202-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b8202-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8202-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8202-122">Authorization</span></span>|<span data-ttu-id="b8202-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8202-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8202-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b8202-124">Accept</span></span>|<span data-ttu-id="b8202-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8202-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8202-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8202-126">Request body</span></span>
<span data-ttu-id="b8202-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="b8202-127">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="b8202-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs enrollmentTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="b8202-128">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="b8202-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8202-129">Property</span></span>|<span data-ttu-id="b8202-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b8202-130">Type</span></span>|<span data-ttu-id="b8202-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8202-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8202-132">id</span><span class="sxs-lookup"><span data-stu-id="b8202-132">id</span></span>|<span data-ttu-id="b8202-133">string</span><span class="sxs-lookup"><span data-stu-id="b8202-133">String</span></span>|<span data-ttu-id="b8202-134">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b8202-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b8202-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b8202-135">eventDateTime</span></span>|<span data-ttu-id="b8202-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8202-136">DateTimeOffset</span></span>|<span data-ttu-id="b8202-137">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="b8202-137">Time when the event occurred .</span></span> <span data-ttu-id="b8202-138">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b8202-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b8202-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="b8202-139">correlationId</span></span>|<span data-ttu-id="b8202-140">String</span><span class="sxs-lookup"><span data-stu-id="b8202-140">String</span></span>|<span data-ttu-id="b8202-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="b8202-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="b8202-142">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b8202-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b8202-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b8202-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="b8202-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b8202-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="b8202-145">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="b8202-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="b8202-146">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b8202-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b8202-147">eventName</span><span class="sxs-lookup"><span data-stu-id="b8202-147">eventName</span></span>|<span data-ttu-id="b8202-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8202-148">String</span></span>|<span data-ttu-id="b8202-149">Ereignis Name, der dem Problem Behandlungs Ereignis entspricht.</span><span class="sxs-lookup"><span data-stu-id="b8202-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="b8202-150">Es handelt sich um ein optionales Feld, geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b8202-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b8202-151">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="b8202-151">additionalInformation</span></span>|<span data-ttu-id="b8202-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b8202-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b8202-153">Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen über das von [DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) geerbte Problem Behandlungs Ereignis bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="b8202-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b8202-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b8202-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="b8202-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8202-155">String</span></span>|<span data-ttu-id="b8202-156">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="b8202-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="b8202-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8202-157">operatingSystem</span></span>|<span data-ttu-id="b8202-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8202-158">String</span></span>|<span data-ttu-id="b8202-159">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="b8202-159">Operating System.</span></span>|
|<span data-ttu-id="b8202-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="b8202-160">osVersion</span></span>|<span data-ttu-id="b8202-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8202-161">String</span></span>|<span data-ttu-id="b8202-162">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="b8202-162">OS Version.</span></span>|
|<span data-ttu-id="b8202-163">userId</span><span class="sxs-lookup"><span data-stu-id="b8202-163">userId</span></span>|<span data-ttu-id="b8202-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8202-164">String</span></span>|<span data-ttu-id="b8202-165">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="b8202-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="b8202-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="b8202-166">deviceId</span></span>|<span data-ttu-id="b8202-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8202-167">String</span></span>|<span data-ttu-id="b8202-168">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="b8202-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="b8202-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="b8202-169">enrollmentType</span></span>|[<span data-ttu-id="b8202-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b8202-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="b8202-171">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="b8202-171">Type of the enrollment.</span></span> <span data-ttu-id="b8202-172">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="b8202-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="b8202-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="b8202-173">failureCategory</span></span>|[<span data-ttu-id="b8202-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="b8202-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="b8202-175">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="b8202-175">Highlevel failure category.</span></span> <span data-ttu-id="b8202-176">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="b8202-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="b8202-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="b8202-177">failureReason</span></span>|<span data-ttu-id="b8202-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8202-178">String</span></span>|<span data-ttu-id="b8202-179">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="b8202-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="b8202-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8202-180">Response</span></span>
<span data-ttu-id="b8202-181">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b8202-181">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8202-182">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8202-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8202-183">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8202-183">Request</span></span>
<span data-ttu-id="b8202-184">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8202-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="b8202-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8202-185">Response</span></span>
<span data-ttu-id="b8202-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8202-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




