---
title: EnrollmentTroubleshootingEvent erstellen
description: Erstellen eines neuen enrollmentTroubleshootingEvent-Objekts.
ms.openlocfilehash: 1c9e36f1cabdbe059bca467f8e1099b2c01c487c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017372"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="d32b3-103">EnrollmentTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="d32b3-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="d32b3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d32b3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d32b3-105">Erstellen eines neuen [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d32b3-105">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d32b3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d32b3-106">Prerequisites</span></span>
<span data-ttu-id="d32b3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d32b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d32b3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d32b3-109">Permission type</span></span>|<span data-ttu-id="d32b3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d32b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d32b3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d32b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d32b3-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d32b3-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d32b3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d32b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d32b3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d32b3-114">Not supported.</span></span>|
|<span data-ttu-id="d32b3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d32b3-115">Application</span></span>|<span data-ttu-id="d32b3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d32b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d32b3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d32b3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="d32b3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d32b3-118">Request headers</span></span>
|<span data-ttu-id="d32b3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d32b3-119">Header</span></span>|<span data-ttu-id="d32b3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d32b3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d32b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d32b3-121">Authorization</span></span>|<span data-ttu-id="d32b3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d32b3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d32b3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d32b3-123">Accept</span></span>|<span data-ttu-id="d32b3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d32b3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d32b3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d32b3-125">Request body</span></span>
<span data-ttu-id="d32b3-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="d32b3-126">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="d32b3-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs enrollmentTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="d32b3-127">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="d32b3-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d32b3-128">Property</span></span>|<span data-ttu-id="d32b3-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d32b3-129">Type</span></span>|<span data-ttu-id="d32b3-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d32b3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d32b3-131">id</span><span class="sxs-lookup"><span data-stu-id="d32b3-131">id</span></span>|<span data-ttu-id="d32b3-132">String</span><span class="sxs-lookup"><span data-stu-id="d32b3-132">String</span></span>|<span data-ttu-id="d32b3-133">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d32b3-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d32b3-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="d32b3-134">eventDateTime</span></span>|<span data-ttu-id="d32b3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d32b3-135">DateTimeOffset</span></span>|<span data-ttu-id="d32b3-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="d32b3-136">Time when the event occurred .</span></span> <span data-ttu-id="d32b3-137">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d32b3-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d32b3-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="d32b3-138">correlationId</span></span>|<span data-ttu-id="d32b3-139">String</span><span class="sxs-lookup"><span data-stu-id="d32b3-139">String</span></span>|<span data-ttu-id="d32b3-140">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d32b3-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="d32b3-141">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d32b3-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d32b3-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d32b3-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="d32b3-143">String</span><span class="sxs-lookup"><span data-stu-id="d32b3-143">String</span></span>|<span data-ttu-id="d32b3-144">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="d32b3-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="d32b3-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d32b3-145">operatingSystem</span></span>|<span data-ttu-id="d32b3-146">String</span><span class="sxs-lookup"><span data-stu-id="d32b3-146">String</span></span>|<span data-ttu-id="d32b3-147">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="d32b3-147">Operating System.</span></span>|
|<span data-ttu-id="d32b3-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="d32b3-148">osVersion</span></span>|<span data-ttu-id="d32b3-149">String</span><span class="sxs-lookup"><span data-stu-id="d32b3-149">String</span></span>|<span data-ttu-id="d32b3-150">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="d32b3-150">OS Version.</span></span>|
|<span data-ttu-id="d32b3-151">userId</span><span class="sxs-lookup"><span data-stu-id="d32b3-151">userId</span></span>|<span data-ttu-id="d32b3-152">String</span><span class="sxs-lookup"><span data-stu-id="d32b3-152">String</span></span>|<span data-ttu-id="d32b3-153">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="d32b3-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="d32b3-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="d32b3-154">deviceId</span></span>|<span data-ttu-id="d32b3-155">String</span><span class="sxs-lookup"><span data-stu-id="d32b3-155">String</span></span>|<span data-ttu-id="d32b3-156">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="d32b3-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="d32b3-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="d32b3-157">enrollmentType</span></span>|[<span data-ttu-id="d32b3-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d32b3-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="d32b3-159">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="d32b3-159">Type of the enrollment.</span></span> <span data-ttu-id="d32b3-160">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="d32b3-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="d32b3-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="d32b3-161">failureCategory</span></span>|[<span data-ttu-id="d32b3-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="d32b3-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="d32b3-163">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="d32b3-163">Highlevel failure category.</span></span> <span data-ttu-id="d32b3-164">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="d32b3-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="d32b3-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="d32b3-165">failureReason</span></span>|<span data-ttu-id="d32b3-166">String</span><span class="sxs-lookup"><span data-stu-id="d32b3-166">String</span></span>|<span data-ttu-id="d32b3-167">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="d32b3-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="d32b3-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="d32b3-168">Response</span></span>
<span data-ttu-id="d32b3-169">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d32b3-169">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d32b3-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d32b3-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="d32b3-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d32b3-171">Request</span></span>
<span data-ttu-id="d32b3-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d32b3-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="d32b3-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="d32b3-173">Response</span></span>
<span data-ttu-id="d32b3-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d32b3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



