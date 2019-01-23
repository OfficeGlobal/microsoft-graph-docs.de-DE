---
title: MobileAppTroubleshootingEvent aktualisieren
description: Beschreibt die MobileAppTroubleshootingEvent Update-Methode, die Microsoft Graph-API für Intune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10bf103a3e796cb5a9e84f1c87ff0571c0bbf551
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430099"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="dcadd-103">MobileAppTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dcadd-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="dcadd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="dcadd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dcadd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dcadd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dcadd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcadd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcadd-107">Aktualisieren Sie die Eigenschaften eines [MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dcadd-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcadd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dcadd-108">Prerequisites</span></span>
<span data-ttu-id="dcadd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dcadd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dcadd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dcadd-111">Permission type</span></span>|<span data-ttu-id="dcadd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dcadd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcadd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dcadd-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="dcadd-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="dcadd-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="dcadd-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcadd-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dcadd-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="dcadd-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="dcadd-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcadd-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dcadd-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dcadd-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcadd-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dcadd-119">Not supported.</span></span>|
|<span data-ttu-id="dcadd-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dcadd-120">Application</span></span>|<span data-ttu-id="dcadd-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dcadd-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcadd-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcadd-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="dcadd-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dcadd-123">Request headers</span></span>
|<span data-ttu-id="dcadd-124">Header</span><span class="sxs-lookup"><span data-stu-id="dcadd-124">Header</span></span>|<span data-ttu-id="dcadd-125">Wert</span><span class="sxs-lookup"><span data-stu-id="dcadd-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcadd-126">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="dcadd-126">Authorization</span></span>|<span data-ttu-id="dcadd-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dcadd-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcadd-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dcadd-128">Accept</span></span>|<span data-ttu-id="dcadd-129">application/json</span><span class="sxs-lookup"><span data-stu-id="dcadd-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcadd-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dcadd-130">Request body</span></span>
<span data-ttu-id="dcadd-131">Geben Sie im Textkörper Anforderung für das Objekt [MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="dcadd-131">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="dcadd-132">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="dcadd-132">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="dcadd-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dcadd-133">Property</span></span>|<span data-ttu-id="dcadd-134">Typ</span><span class="sxs-lookup"><span data-stu-id="dcadd-134">Type</span></span>|<span data-ttu-id="dcadd-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dcadd-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcadd-136">id</span><span class="sxs-lookup"><span data-stu-id="dcadd-136">id</span></span>|<span data-ttu-id="dcadd-137">String</span><span class="sxs-lookup"><span data-stu-id="dcadd-137">String</span></span>|<span data-ttu-id="dcadd-138">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="dcadd-138">The GUID for the object</span></span>|
|<span data-ttu-id="dcadd-139">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="dcadd-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="dcadd-140">zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="dcadd-140">additionalInformation</span></span>|<span data-ttu-id="dcadd-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="dcadd-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="dcadd-142">Eine Reihe von Schlüssel und String-Wert-Paare bietet zusätzliche Informationen für die Problembehandlung bei-Ereignis.</span><span class="sxs-lookup"><span data-stu-id="dcadd-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="dcadd-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="dcadd-143">applicationId</span></span>|<span data-ttu-id="dcadd-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dcadd-144">String</span></span>|<span data-ttu-id="dcadd-145">Intune Anwendungsbezeichner.</span><span class="sxs-lookup"><span data-stu-id="dcadd-145">Intune application identifier.</span></span>|
|<span data-ttu-id="dcadd-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="dcadd-146">correlationId</span></span>|<span data-ttu-id="dcadd-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dcadd-147">String</span></span>|<span data-ttu-id="dcadd-148">ID für den Fehler in den Dienst tracing verwendet.</span><span class="sxs-lookup"><span data-stu-id="dcadd-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="dcadd-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="dcadd-149">eventDateTime</span></span>|<span data-ttu-id="dcadd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcadd-150">DateTimeOffset</span></span>|<span data-ttu-id="dcadd-151">Zeit, die das Ereignis auftrat.</span><span class="sxs-lookup"><span data-stu-id="dcadd-151">Time when the event occurred.</span></span> |
|<span data-ttu-id="dcadd-152">Ereignisname</span><span class="sxs-lookup"><span data-stu-id="dcadd-152">eventName</span></span>|<span data-ttu-id="dcadd-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dcadd-153">String</span></span>|<span data-ttu-id="dcadd-154">Name des Ereignisses, das Ereignis Problembehandlung entspricht.</span><span class="sxs-lookup"><span data-stu-id="dcadd-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="dcadd-155">Optional.</span><span class="sxs-lookup"><span data-stu-id="dcadd-155">Optional.</span></span>|
|<span data-ttu-id="dcadd-156">Verlauf</span><span class="sxs-lookup"><span data-stu-id="dcadd-156">history</span></span>|<span data-ttu-id="dcadd-157">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="dcadd-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="dcadd-158">Problembehandlung bei Historienelement Intune Mobile-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="dcadd-158">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="dcadd-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="dcadd-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="dcadd-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dcadd-160">String</span></span>|<span data-ttu-id="dcadd-161">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="dcadd-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="dcadd-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="dcadd-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="dcadd-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="dcadd-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="dcadd-164">Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.</span><span class="sxs-lookup"><span data-stu-id="dcadd-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="dcadd-165">userId</span><span class="sxs-lookup"><span data-stu-id="dcadd-165">userId</span></span>|<span data-ttu-id="dcadd-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dcadd-166">String</span></span>|<span data-ttu-id="dcadd-167">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="dcadd-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="dcadd-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcadd-168">Response</span></span>
<span data-ttu-id="dcadd-169">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dcadd-169">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcadd-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dcadd-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcadd-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcadd-171">Request</span></span>
<span data-ttu-id="dcadd-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dcadd-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="dcadd-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcadd-173">Response</span></span>
<span data-ttu-id="dcadd-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dcadd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




