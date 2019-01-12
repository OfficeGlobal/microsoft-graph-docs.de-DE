---
title: enrollmentTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 002f1e29c993326ab85d17d5092935525249a9db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939771"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="3fb6b-103">enrollmentTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3fb6b-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="3fb6b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fb6b-105">Aktualisieren der Eigenschaften eines [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fb6b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3fb6b-106">Prerequisites</span></span>
<span data-ttu-id="3fb6b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fb6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fb6b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3fb6b-109">Permission type</span></span>|<span data-ttu-id="3fb6b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3fb6b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fb6b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3fb6b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3fb6b-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fb6b-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3fb6b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3fb6b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fb6b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fb6b-114">Not supported.</span></span>|
|<span data-ttu-id="3fb6b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3fb6b-115">Application</span></span>|<span data-ttu-id="3fb6b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fb6b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fb6b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fb6b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="3fb6b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3fb6b-118">Request headers</span></span>
|<span data-ttu-id="3fb6b-119">Header</span><span class="sxs-lookup"><span data-stu-id="3fb6b-119">Header</span></span>|<span data-ttu-id="3fb6b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3fb6b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fb6b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fb6b-121">Authorization</span></span>|<span data-ttu-id="3fb6b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3fb6b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fb6b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3fb6b-123">Accept</span></span>|<span data-ttu-id="3fb6b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3fb6b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fb6b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3fb6b-125">Request body</span></span>
<span data-ttu-id="3fb6b-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="3fb6b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="3fb6b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3fb6b-128">Property</span></span>|<span data-ttu-id="3fb6b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3fb6b-129">Type</span></span>|<span data-ttu-id="3fb6b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3fb6b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fb6b-131">id</span><span class="sxs-lookup"><span data-stu-id="3fb6b-131">id</span></span>|<span data-ttu-id="3fb6b-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3fb6b-132">String</span></span>|<span data-ttu-id="3fb6b-133">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3fb6b-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3fb6b-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="3fb6b-134">eventDateTime</span></span>|<span data-ttu-id="3fb6b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fb6b-135">DateTimeOffset</span></span>|<span data-ttu-id="3fb6b-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-136">Time when the event occurred .</span></span> <span data-ttu-id="3fb6b-137">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3fb6b-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3fb6b-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="3fb6b-138">correlationId</span></span>|<span data-ttu-id="3fb6b-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3fb6b-139">String</span></span>|<span data-ttu-id="3fb6b-140">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="3fb6b-141">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3fb6b-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3fb6b-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3fb6b-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="3fb6b-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3fb6b-143">String</span></span>|<span data-ttu-id="3fb6b-144">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="3fb6b-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="3fb6b-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3fb6b-145">operatingSystem</span></span>|<span data-ttu-id="3fb6b-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3fb6b-146">String</span></span>|<span data-ttu-id="3fb6b-147">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="3fb6b-147">Operating System.</span></span>|
|<span data-ttu-id="3fb6b-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="3fb6b-148">osVersion</span></span>|<span data-ttu-id="3fb6b-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3fb6b-149">String</span></span>|<span data-ttu-id="3fb6b-150">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="3fb6b-150">OS Version.</span></span>|
|<span data-ttu-id="3fb6b-151">userId</span><span class="sxs-lookup"><span data-stu-id="3fb6b-151">userId</span></span>|<span data-ttu-id="3fb6b-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3fb6b-152">String</span></span>|<span data-ttu-id="3fb6b-153">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="3fb6b-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="3fb6b-154">deviceId</span></span>|<span data-ttu-id="3fb6b-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3fb6b-155">String</span></span>|<span data-ttu-id="3fb6b-156">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="3fb6b-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="3fb6b-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="3fb6b-157">enrollmentType</span></span>|[<span data-ttu-id="3fb6b-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3fb6b-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="3fb6b-159">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-159">Type of the enrollment.</span></span> <span data-ttu-id="3fb6b-160">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="3fb6b-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="3fb6b-161">failureCategory</span></span>|[<span data-ttu-id="3fb6b-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="3fb6b-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="3fb6b-163">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-163">Highlevel failure category.</span></span> <span data-ttu-id="3fb6b-164">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="3fb6b-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="3fb6b-165">failureReason</span></span>|<span data-ttu-id="3fb6b-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3fb6b-166">String</span></span>|<span data-ttu-id="3fb6b-167">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="3fb6b-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="3fb6b-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fb6b-168">Response</span></span>
<span data-ttu-id="3fb6b-169">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fb6b-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3fb6b-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fb6b-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fb6b-171">Request</span></span>
<span data-ttu-id="3fb6b-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 440

{
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

### <a name="response"></a><span data-ttu-id="3fb6b-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fb6b-173">Response</span></span>
<span data-ttu-id="3fb6b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3fb6b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



