---
title: enrollmentTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentTroubleshootingEvent-Objekts.
author: tfitzmac
ms.openlocfilehash: 38fb219c653e59504e5402c5313c1c871ee732d6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325368"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="7d68c-103">enrollmentTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7d68c-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="7d68c-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7d68c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d68c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7d68c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d68c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7d68c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d68c-107">Aktualisieren der Eigenschaften eines [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7d68c-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d68c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7d68c-108">Prerequisites</span></span>
<span data-ttu-id="7d68c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d68c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d68c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7d68c-111">Permission type</span></span>|<span data-ttu-id="7d68c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7d68c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d68c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7d68c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d68c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d68c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7d68c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7d68c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d68c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d68c-116">Not supported.</span></span>|
|<span data-ttu-id="7d68c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7d68c-117">Application</span></span>|<span data-ttu-id="7d68c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d68c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d68c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d68c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="7d68c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7d68c-120">Request headers</span></span>
|<span data-ttu-id="7d68c-121">Header</span><span class="sxs-lookup"><span data-stu-id="7d68c-121">Header</span></span>|<span data-ttu-id="7d68c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7d68c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d68c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7d68c-123">Authorization</span></span>|<span data-ttu-id="7d68c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7d68c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d68c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d68c-125">Accept</span></span>|<span data-ttu-id="7d68c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d68c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d68c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7d68c-127">Request body</span></span>
<span data-ttu-id="7d68c-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="7d68c-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="7d68c-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7d68c-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="7d68c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7d68c-130">Property</span></span>|<span data-ttu-id="7d68c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7d68c-131">Type</span></span>|<span data-ttu-id="7d68c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d68c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d68c-133">id</span><span class="sxs-lookup"><span data-stu-id="7d68c-133">id</span></span>|<span data-ttu-id="7d68c-134">String</span><span class="sxs-lookup"><span data-stu-id="7d68c-134">String</span></span>|<span data-ttu-id="7d68c-135">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7d68c-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7d68c-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="7d68c-136">eventDateTime</span></span>|<span data-ttu-id="7d68c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d68c-137">DateTimeOffset</span></span>|<span data-ttu-id="7d68c-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="7d68c-138">Time when the event occurred .</span></span> <span data-ttu-id="7d68c-139">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7d68c-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7d68c-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="7d68c-140">correlationId</span></span>|<span data-ttu-id="7d68c-141">String</span><span class="sxs-lookup"><span data-stu-id="7d68c-141">String</span></span>|<span data-ttu-id="7d68c-142">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="7d68c-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="7d68c-143">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7d68c-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7d68c-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7d68c-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="7d68c-145">String</span><span class="sxs-lookup"><span data-stu-id="7d68c-145">String</span></span>|<span data-ttu-id="7d68c-146">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="7d68c-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="7d68c-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7d68c-147">operatingSystem</span></span>|<span data-ttu-id="7d68c-148">String</span><span class="sxs-lookup"><span data-stu-id="7d68c-148">String</span></span>|<span data-ttu-id="7d68c-149">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="7d68c-149">Operating System.</span></span>|
|<span data-ttu-id="7d68c-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="7d68c-150">osVersion</span></span>|<span data-ttu-id="7d68c-151">String</span><span class="sxs-lookup"><span data-stu-id="7d68c-151">String</span></span>|<span data-ttu-id="7d68c-152">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="7d68c-152">OS Version.</span></span>|
|<span data-ttu-id="7d68c-153">userId</span><span class="sxs-lookup"><span data-stu-id="7d68c-153">userId</span></span>|<span data-ttu-id="7d68c-154">String</span><span class="sxs-lookup"><span data-stu-id="7d68c-154">String</span></span>|<span data-ttu-id="7d68c-155">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="7d68c-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="7d68c-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="7d68c-156">deviceId</span></span>|<span data-ttu-id="7d68c-157">String</span><span class="sxs-lookup"><span data-stu-id="7d68c-157">String</span></span>|<span data-ttu-id="7d68c-158">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="7d68c-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="7d68c-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="7d68c-159">enrollmentType</span></span>|[<span data-ttu-id="7d68c-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="7d68c-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="7d68c-161">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="7d68c-161">Type of the enrollment.</span></span> <span data-ttu-id="7d68c-162">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="7d68c-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="7d68c-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="7d68c-163">failureCategory</span></span>|[<span data-ttu-id="7d68c-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="7d68c-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="7d68c-165">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="7d68c-165">Highlevel failure category.</span></span> <span data-ttu-id="7d68c-166">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="7d68c-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="7d68c-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="7d68c-167">failureReason</span></span>|<span data-ttu-id="7d68c-168">String</span><span class="sxs-lookup"><span data-stu-id="7d68c-168">String</span></span>|<span data-ttu-id="7d68c-169">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="7d68c-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="7d68c-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d68c-170">Response</span></span>
<span data-ttu-id="7d68c-171">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7d68c-171">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d68c-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7d68c-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d68c-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d68c-173">Request</span></span>
<span data-ttu-id="7d68c-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7d68c-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="7d68c-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d68c-175">Response</span></span>
<span data-ttu-id="7d68c-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7d68c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





