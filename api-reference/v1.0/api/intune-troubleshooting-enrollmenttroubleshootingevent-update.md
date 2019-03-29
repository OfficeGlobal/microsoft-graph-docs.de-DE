---
title: enrollmentTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a16a24a27a56ab1a733b46fa9ad9b7469f0a8ee3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975770"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="f7218-103">enrollmentTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f7218-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="f7218-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f7218-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7218-105">Aktualisieren der Eigenschaften eines [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f7218-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7218-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f7218-106">Prerequisites</span></span>
<span data-ttu-id="f7218-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7218-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7218-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7218-109">Permission type</span></span>|<span data-ttu-id="f7218-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7218-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7218-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7218-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7218-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7218-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f7218-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7218-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7218-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7218-114">Not supported.</span></span>|
|<span data-ttu-id="f7218-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7218-115">Application</span></span>|<span data-ttu-id="f7218-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7218-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7218-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7218-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="f7218-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7218-118">Request headers</span></span>
|<span data-ttu-id="f7218-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f7218-119">Header</span></span>|<span data-ttu-id="f7218-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f7218-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7218-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7218-121">Authorization</span></span>|<span data-ttu-id="f7218-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f7218-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7218-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f7218-123">Accept</span></span>|<span data-ttu-id="f7218-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f7218-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7218-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7218-125">Request body</span></span>
<span data-ttu-id="f7218-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="f7218-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="f7218-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f7218-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="f7218-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7218-128">Property</span></span>|<span data-ttu-id="f7218-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f7218-129">Type</span></span>|<span data-ttu-id="f7218-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7218-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7218-131">id</span><span class="sxs-lookup"><span data-stu-id="f7218-131">id</span></span>|<span data-ttu-id="f7218-132">String</span><span class="sxs-lookup"><span data-stu-id="f7218-132">String</span></span>|<span data-ttu-id="f7218-133">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f7218-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f7218-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f7218-134">eventDateTime</span></span>|<span data-ttu-id="f7218-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7218-135">DateTimeOffset</span></span>|<span data-ttu-id="f7218-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="f7218-136">Time when the event occurred .</span></span> <span data-ttu-id="f7218-137">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f7218-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f7218-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="f7218-138">correlationId</span></span>|<span data-ttu-id="f7218-139">String</span><span class="sxs-lookup"><span data-stu-id="f7218-139">String</span></span>|<span data-ttu-id="f7218-140">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="f7218-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="f7218-141">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f7218-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f7218-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f7218-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="f7218-143">String</span><span class="sxs-lookup"><span data-stu-id="f7218-143">String</span></span>|<span data-ttu-id="f7218-144">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="f7218-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="f7218-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f7218-145">operatingSystem</span></span>|<span data-ttu-id="f7218-146">String</span><span class="sxs-lookup"><span data-stu-id="f7218-146">String</span></span>|<span data-ttu-id="f7218-147">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="f7218-147">Operating System.</span></span>|
|<span data-ttu-id="f7218-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="f7218-148">osVersion</span></span>|<span data-ttu-id="f7218-149">String</span><span class="sxs-lookup"><span data-stu-id="f7218-149">String</span></span>|<span data-ttu-id="f7218-150">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="f7218-150">OS Version.</span></span>|
|<span data-ttu-id="f7218-151">userId</span><span class="sxs-lookup"><span data-stu-id="f7218-151">userId</span></span>|<span data-ttu-id="f7218-152">String</span><span class="sxs-lookup"><span data-stu-id="f7218-152">String</span></span>|<span data-ttu-id="f7218-153">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="f7218-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="f7218-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="f7218-154">deviceId</span></span>|<span data-ttu-id="f7218-155">String</span><span class="sxs-lookup"><span data-stu-id="f7218-155">String</span></span>|<span data-ttu-id="f7218-156">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="f7218-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="f7218-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="f7218-157">enrollmentType</span></span>|[<span data-ttu-id="f7218-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f7218-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f7218-159">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="f7218-159">Type of the enrollment.</span></span> <span data-ttu-id="f7218-160">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="f7218-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="f7218-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="f7218-161">failureCategory</span></span>|[<span data-ttu-id="f7218-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="f7218-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="f7218-163">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="f7218-163">Highlevel failure category.</span></span> <span data-ttu-id="f7218-164">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="f7218-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="f7218-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="f7218-165">failureReason</span></span>|<span data-ttu-id="f7218-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7218-166">String</span></span>|<span data-ttu-id="f7218-167">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="f7218-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="f7218-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7218-168">Response</span></span>
<span data-ttu-id="f7218-169">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f7218-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7218-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7218-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7218-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7218-171">Request</span></span>
<span data-ttu-id="f7218-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f7218-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
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

### <a name="response"></a><span data-ttu-id="f7218-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7218-173">Response</span></span>
<span data-ttu-id="f7218-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7218-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
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



