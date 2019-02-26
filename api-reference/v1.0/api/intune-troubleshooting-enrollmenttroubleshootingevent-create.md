---
title: EnrollmentTroubleshootingEvent erstellen
description: Erstellen eines neuen enrollmentTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d501a97d7281aad7fe79039d0fb893777c84c446
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252868"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="0455c-103">EnrollmentTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="0455c-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="0455c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0455c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0455c-105">Erstellen eines neuen [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0455c-105">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0455c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0455c-106">Prerequisites</span></span>
<span data-ttu-id="0455c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0455c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0455c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0455c-109">Permission type</span></span>|<span data-ttu-id="0455c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0455c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0455c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0455c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0455c-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0455c-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0455c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0455c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0455c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0455c-114">Not supported.</span></span>|
|<span data-ttu-id="0455c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0455c-115">Application</span></span>|<span data-ttu-id="0455c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0455c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0455c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0455c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="0455c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0455c-118">Request headers</span></span>
|<span data-ttu-id="0455c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0455c-119">Header</span></span>|<span data-ttu-id="0455c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0455c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0455c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0455c-121">Authorization</span></span>|<span data-ttu-id="0455c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0455c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0455c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0455c-123">Accept</span></span>|<span data-ttu-id="0455c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0455c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0455c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0455c-125">Request body</span></span>
<span data-ttu-id="0455c-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="0455c-126">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="0455c-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs enrollmentTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="0455c-127">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="0455c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0455c-128">Property</span></span>|<span data-ttu-id="0455c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0455c-129">Type</span></span>|<span data-ttu-id="0455c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0455c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0455c-131">id</span><span class="sxs-lookup"><span data-stu-id="0455c-131">id</span></span>|<span data-ttu-id="0455c-132">string</span><span class="sxs-lookup"><span data-stu-id="0455c-132">String</span></span>|<span data-ttu-id="0455c-133">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0455c-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0455c-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="0455c-134">eventDateTime</span></span>|<span data-ttu-id="0455c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0455c-135">DateTimeOffset</span></span>|<span data-ttu-id="0455c-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="0455c-136">Time when the event occurred .</span></span> <span data-ttu-id="0455c-137">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0455c-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0455c-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="0455c-138">correlationId</span></span>|<span data-ttu-id="0455c-139">String</span><span class="sxs-lookup"><span data-stu-id="0455c-139">String</span></span>|<span data-ttu-id="0455c-140">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="0455c-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="0455c-141">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0455c-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0455c-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0455c-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="0455c-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0455c-143">String</span></span>|<span data-ttu-id="0455c-144">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="0455c-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="0455c-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0455c-145">operatingSystem</span></span>|<span data-ttu-id="0455c-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0455c-146">String</span></span>|<span data-ttu-id="0455c-147">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="0455c-147">Operating System.</span></span>|
|<span data-ttu-id="0455c-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="0455c-148">osVersion</span></span>|<span data-ttu-id="0455c-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0455c-149">String</span></span>|<span data-ttu-id="0455c-150">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="0455c-150">OS Version.</span></span>|
|<span data-ttu-id="0455c-151">userId</span><span class="sxs-lookup"><span data-stu-id="0455c-151">userId</span></span>|<span data-ttu-id="0455c-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0455c-152">String</span></span>|<span data-ttu-id="0455c-153">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="0455c-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="0455c-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="0455c-154">deviceId</span></span>|<span data-ttu-id="0455c-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0455c-155">String</span></span>|<span data-ttu-id="0455c-156">Azure AD-Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="0455c-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="0455c-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="0455c-157">enrollmentType</span></span>|[<span data-ttu-id="0455c-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0455c-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="0455c-159">Typ der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="0455c-159">Type of the enrollment.</span></span> <span data-ttu-id="0455c-160">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="0455c-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="0455c-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="0455c-161">failureCategory</span></span>|[<span data-ttu-id="0455c-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="0455c-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="0455c-163">Allgemeine Fehlerkategorie.</span><span class="sxs-lookup"><span data-stu-id="0455c-163">Highlevel failure category.</span></span> <span data-ttu-id="0455c-164">Mögliche Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` und `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="0455c-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="0455c-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="0455c-165">failureReason</span></span>|<span data-ttu-id="0455c-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0455c-166">String</span></span>|<span data-ttu-id="0455c-167">Detaillierte Fehlerursache</span><span class="sxs-lookup"><span data-stu-id="0455c-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="0455c-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="0455c-168">Response</span></span>
<span data-ttu-id="0455c-169">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0455c-169">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0455c-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0455c-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="0455c-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0455c-171">Request</span></span>
<span data-ttu-id="0455c-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0455c-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0455c-173">Reaktion</span><span class="sxs-lookup"><span data-stu-id="0455c-173">Response</span></span>
<span data-ttu-id="0455c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0455c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



