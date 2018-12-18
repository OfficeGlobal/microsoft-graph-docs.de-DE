---
title: EnrollmentTroubleshootingEvent erstellen
description: Erstellen eines neuen enrollmentTroubleshootingEvent-Objekts.
author: tfitzmac
ms.openlocfilehash: 213c81a66cca2696083f54a5e0fc4cad28cce9f1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309912"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="757e2-103">EnrollmentTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="757e2-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="757e2-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="757e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="757e2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="757e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="757e2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="757e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="757e2-107">Erstellen eines neuen [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="757e2-107">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="757e2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="757e2-108">Prerequisites</span></span>
<span data-ttu-id="757e2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="757e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="757e2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="757e2-111">Permission type</span></span>|<span data-ttu-id="757e2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="757e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="757e2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="757e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="757e2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="757e2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="757e2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="757e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="757e2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="757e2-116">Not supported.</span></span>|
|<span data-ttu-id="757e2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="757e2-117">Application</span></span>|<span data-ttu-id="757e2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="757e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="757e2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="757e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="757e2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="757e2-120">Request headers</span></span>
|<span data-ttu-id="757e2-121">Header</span><span class="sxs-lookup"><span data-stu-id="757e2-121">Header</span></span>|<span data-ttu-id="757e2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="757e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="757e2-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="757e2-123">Authorization</span></span>|<span data-ttu-id="757e2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="757e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="757e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="757e2-125">Accept</span></span>|<span data-ttu-id="757e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="757e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="757e2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="757e2-127">Request body</span></span>
<span data-ttu-id="757e2-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="757e2-128">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="757e2-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs enrollmentTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="757e2-129">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="757e2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="757e2-130">Property</span></span>|<span data-ttu-id="757e2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="757e2-131">Type</span></span>|<span data-ttu-id="757e2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="757e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="757e2-133">id</span><span class="sxs-lookup"><span data-stu-id="757e2-133">id</span></span>|<span data-ttu-id="757e2-134">String</span><span class="sxs-lookup"><span data-stu-id="757e2-134">String</span></span>|<span data-ttu-id="757e2-135">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="757e2-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="757e2-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="757e2-136">eventDateTime</span></span>|<span data-ttu-id="757e2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="757e2-137">DateTimeOffset</span></span>|<span data-ttu-id="757e2-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="757e2-138">Time when the event occurred .</span></span> <span data-ttu-id="757e2-139">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="757e2-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="757e2-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="757e2-140">correlationId</span></span>|<span data-ttu-id="757e2-141">String</span><span class="sxs-lookup"><span data-stu-id="757e2-141">String</span></span>|<span data-ttu-id="757e2-142">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="757e2-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="757e2-143">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="757e2-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="757e2-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="757e2-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="757e2-145">String</span><span class="sxs-lookup"><span data-stu-id="757e2-145">String</span></span>|<span data-ttu-id="757e2-146">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="757e2-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="757e2-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="757e2-147">operatingSystem</span></span>|<span data-ttu-id="757e2-148">String</span><span class="sxs-lookup"><span data-stu-id="757e2-148">String</span></span>|<span data-ttu-id="757e2-149">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="757e2-149">Operating System.</span></span>|
|<span data-ttu-id="757e2-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="757e2-150">osVersion</span></span>|<span data-ttu-id="757e2-151">String</span><span class="sxs-lookup"><span data-stu-id="757e2-151">String</span></span>|<span data-ttu-id="757e2-152">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="757e2-152">OS Version.</span></span>|
|<span data-ttu-id="757e2-153">userId</span><span class="sxs-lookup"><span data-stu-id="757e2-153">userId</span></span>|<span data-ttu-id="757e2-154">String</span><span class="sxs-lookup"><span data-stu-id="757e2-154">String</span></span>|<span data-ttu-id="757e2-155">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="757e2-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="757e2-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="757e2-156">deviceId</span></span>|<span data-ttu-id="757e2-157">String</span><span class="sxs-lookup"><span data-stu-id="757e2-157">String</span></span>|<span data-ttu-id="757e2-158">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="757e2-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="757e2-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="757e2-159">enrollmentType</span></span>|[<span data-ttu-id="757e2-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="757e2-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="757e2-161">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="757e2-161">Type of the enrollment.</span></span> <span data-ttu-id="757e2-162">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="757e2-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="757e2-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="757e2-163">failureCategory</span></span>|[<span data-ttu-id="757e2-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="757e2-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="757e2-165">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="757e2-165">Highlevel failure category.</span></span> <span data-ttu-id="757e2-166">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="757e2-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="757e2-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="757e2-167">failureReason</span></span>|<span data-ttu-id="757e2-168">String</span><span class="sxs-lookup"><span data-stu-id="757e2-168">String</span></span>|<span data-ttu-id="757e2-169">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="757e2-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="757e2-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="757e2-170">Response</span></span>
<span data-ttu-id="757e2-171">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="757e2-171">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="757e2-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="757e2-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="757e2-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="757e2-173">Request</span></span>
<span data-ttu-id="757e2-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="757e2-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="757e2-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="757e2-175">Response</span></span>
<span data-ttu-id="757e2-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="757e2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





