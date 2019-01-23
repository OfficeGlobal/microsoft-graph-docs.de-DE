---
title: enrollmentTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentTroubleshootingEvent-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: efbc823b4ba7a5e28a0a2e7d82b7708102002a71
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399787"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="29613-103">enrollmentTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="29613-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="29613-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="29613-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29613-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="29613-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29613-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29613-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29613-107">Aktualisieren der Eigenschaften eines [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="29613-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29613-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="29613-108">Prerequisites</span></span>
<span data-ttu-id="29613-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="29613-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="29613-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29613-111">Permission type</span></span>|<span data-ttu-id="29613-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29613-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29613-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29613-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29613-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29613-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="29613-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29613-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29613-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29613-116">Not supported.</span></span>|
|<span data-ttu-id="29613-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29613-117">Application</span></span>|<span data-ttu-id="29613-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29613-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29613-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29613-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="29613-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29613-120">Request headers</span></span>
|<span data-ttu-id="29613-121">Header</span><span class="sxs-lookup"><span data-stu-id="29613-121">Header</span></span>|<span data-ttu-id="29613-122">Wert</span><span class="sxs-lookup"><span data-stu-id="29613-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29613-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="29613-123">Authorization</span></span>|<span data-ttu-id="29613-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="29613-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29613-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="29613-125">Accept</span></span>|<span data-ttu-id="29613-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29613-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29613-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29613-127">Request body</span></span>
<span data-ttu-id="29613-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="29613-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="29613-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="29613-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="29613-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="29613-130">Property</span></span>|<span data-ttu-id="29613-131">Typ</span><span class="sxs-lookup"><span data-stu-id="29613-131">Type</span></span>|<span data-ttu-id="29613-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29613-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29613-133">id</span><span class="sxs-lookup"><span data-stu-id="29613-133">id</span></span>|<span data-ttu-id="29613-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29613-134">String</span></span>|<span data-ttu-id="29613-135">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29613-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29613-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="29613-136">eventDateTime</span></span>|<span data-ttu-id="29613-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29613-137">DateTimeOffset</span></span>|<span data-ttu-id="29613-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="29613-138">Time when the event occurred .</span></span> <span data-ttu-id="29613-139">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29613-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29613-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="29613-140">correlationId</span></span>|<span data-ttu-id="29613-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29613-141">String</span></span>|<span data-ttu-id="29613-142">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="29613-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="29613-143">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29613-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29613-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="29613-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="29613-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="29613-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="29613-146">Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.</span><span class="sxs-lookup"><span data-stu-id="29613-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="29613-147">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29613-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29613-148">Ereignisname</span><span class="sxs-lookup"><span data-stu-id="29613-148">eventName</span></span>|<span data-ttu-id="29613-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29613-149">String</span></span>|<span data-ttu-id="29613-150">Name des Ereignisses, das Ereignis Problembehandlung entspricht.</span><span class="sxs-lookup"><span data-stu-id="29613-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="29613-151">Es ist ein optionales Feld Inherited aus [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29613-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29613-152">zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="29613-152">additionalInformation</span></span>|<span data-ttu-id="29613-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="29613-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="29613-154">Eine Reihe von Schlüssel und String-Wert-Paare bietet zusätzliche Informationen für die Problembehandlung bei Ereignis Inherited aus [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29613-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29613-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="29613-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="29613-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29613-156">String</span></span>|<span data-ttu-id="29613-157">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="29613-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="29613-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="29613-158">operatingSystem</span></span>|<span data-ttu-id="29613-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29613-159">String</span></span>|<span data-ttu-id="29613-160">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="29613-160">Operating System.</span></span>|
|<span data-ttu-id="29613-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="29613-161">osVersion</span></span>|<span data-ttu-id="29613-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29613-162">String</span></span>|<span data-ttu-id="29613-163">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="29613-163">OS Version.</span></span>|
|<span data-ttu-id="29613-164">userId</span><span class="sxs-lookup"><span data-stu-id="29613-164">userId</span></span>|<span data-ttu-id="29613-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29613-165">String</span></span>|<span data-ttu-id="29613-166">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="29613-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="29613-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="29613-167">deviceId</span></span>|<span data-ttu-id="29613-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29613-168">String</span></span>|<span data-ttu-id="29613-169">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="29613-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="29613-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="29613-170">enrollmentType</span></span>|[<span data-ttu-id="29613-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="29613-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="29613-172">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="29613-172">Type of the enrollment.</span></span> <span data-ttu-id="29613-173">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="29613-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="29613-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="29613-174">failureCategory</span></span>|[<span data-ttu-id="29613-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="29613-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="29613-176">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="29613-176">Highlevel failure category.</span></span> <span data-ttu-id="29613-177">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="29613-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="29613-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="29613-178">failureReason</span></span>|<span data-ttu-id="29613-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29613-179">String</span></span>|<span data-ttu-id="29613-180">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="29613-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="29613-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="29613-181">Response</span></span>
<span data-ttu-id="29613-182">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="29613-182">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29613-183">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29613-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="29613-184">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29613-184">Request</span></span>
<span data-ttu-id="29613-185">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29613-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29613-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="29613-186">Response</span></span>
<span data-ttu-id="29613-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29613-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




