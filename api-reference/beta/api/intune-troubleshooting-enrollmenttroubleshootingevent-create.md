---
title: EnrollmentTroubleshootingEvent erstellen
description: Erstellen eines neuen enrollmentTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ae80e2084945b1dd5fb0259b16b178ab2d38ec5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924566"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="910cd-103">EnrollmentTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="910cd-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="910cd-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="910cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="910cd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="910cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="910cd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="910cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="910cd-107">Erstellen eines neuen [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="910cd-107">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="910cd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="910cd-108">Prerequisites</span></span>
<span data-ttu-id="910cd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="910cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="910cd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="910cd-111">Permission type</span></span>|<span data-ttu-id="910cd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="910cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="910cd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="910cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="910cd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="910cd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="910cd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="910cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="910cd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="910cd-116">Not supported.</span></span>|
|<span data-ttu-id="910cd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="910cd-117">Application</span></span>|<span data-ttu-id="910cd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="910cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="910cd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="910cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="910cd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="910cd-120">Request headers</span></span>
|<span data-ttu-id="910cd-121">Header</span><span class="sxs-lookup"><span data-stu-id="910cd-121">Header</span></span>|<span data-ttu-id="910cd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="910cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="910cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="910cd-123">Authorization</span></span>|<span data-ttu-id="910cd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="910cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="910cd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="910cd-125">Accept</span></span>|<span data-ttu-id="910cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="910cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="910cd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="910cd-127">Request body</span></span>
<span data-ttu-id="910cd-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="910cd-128">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="910cd-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs enrollmentTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="910cd-129">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="910cd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="910cd-130">Property</span></span>|<span data-ttu-id="910cd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="910cd-131">Type</span></span>|<span data-ttu-id="910cd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="910cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="910cd-133">id</span><span class="sxs-lookup"><span data-stu-id="910cd-133">id</span></span>|<span data-ttu-id="910cd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cd-134">String</span></span>|<span data-ttu-id="910cd-135">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="910cd-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="910cd-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="910cd-136">eventDateTime</span></span>|<span data-ttu-id="910cd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910cd-137">DateTimeOffset</span></span>|<span data-ttu-id="910cd-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="910cd-138">Time when the event occurred .</span></span> <span data-ttu-id="910cd-139">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="910cd-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="910cd-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="910cd-140">correlationId</span></span>|<span data-ttu-id="910cd-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cd-141">String</span></span>|<span data-ttu-id="910cd-142">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="910cd-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="910cd-143">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="910cd-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="910cd-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="910cd-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="910cd-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cd-145">String</span></span>|<span data-ttu-id="910cd-146">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="910cd-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="910cd-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="910cd-147">operatingSystem</span></span>|<span data-ttu-id="910cd-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cd-148">String</span></span>|<span data-ttu-id="910cd-149">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="910cd-149">Operating System.</span></span>|
|<span data-ttu-id="910cd-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="910cd-150">osVersion</span></span>|<span data-ttu-id="910cd-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cd-151">String</span></span>|<span data-ttu-id="910cd-152">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="910cd-152">OS Version.</span></span>|
|<span data-ttu-id="910cd-153">userId</span><span class="sxs-lookup"><span data-stu-id="910cd-153">userId</span></span>|<span data-ttu-id="910cd-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cd-154">String</span></span>|<span data-ttu-id="910cd-155">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="910cd-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="910cd-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="910cd-156">deviceId</span></span>|<span data-ttu-id="910cd-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cd-157">String</span></span>|<span data-ttu-id="910cd-158">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="910cd-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="910cd-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="910cd-159">enrollmentType</span></span>|[<span data-ttu-id="910cd-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="910cd-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="910cd-161">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="910cd-161">Type of the enrollment.</span></span> <span data-ttu-id="910cd-162">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="910cd-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="910cd-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="910cd-163">failureCategory</span></span>|[<span data-ttu-id="910cd-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="910cd-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="910cd-165">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="910cd-165">Highlevel failure category.</span></span> <span data-ttu-id="910cd-166">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="910cd-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="910cd-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="910cd-167">failureReason</span></span>|<span data-ttu-id="910cd-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cd-168">String</span></span>|<span data-ttu-id="910cd-169">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="910cd-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="910cd-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="910cd-170">Response</span></span>
<span data-ttu-id="910cd-171">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="910cd-171">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="910cd-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="910cd-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="910cd-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="910cd-173">Request</span></span>
<span data-ttu-id="910cd-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="910cd-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="910cd-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="910cd-175">Response</span></span>
<span data-ttu-id="910cd-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="910cd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





