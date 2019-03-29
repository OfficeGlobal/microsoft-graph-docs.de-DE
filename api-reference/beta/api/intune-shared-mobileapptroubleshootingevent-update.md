---
title: MobileAppTroubleshootingEvent aktualisieren
description: Beschreibt die Update mobileAppTroubleshootingEvent-Methode der Microsoft Graph-API für InTune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05163b0251690c990454e671ebab6aaf26fa02ad
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957479"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="eebee-103">MobileAppTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="eebee-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="eebee-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="eebee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eebee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eebee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eebee-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eebee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eebee-107">Aktualisieren der Eigenschaften eines [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="eebee-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eebee-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eebee-108">Prerequisites</span></span>
<span data-ttu-id="eebee-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eebee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eebee-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eebee-111">Permission type</span></span>|<span data-ttu-id="eebee-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eebee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eebee-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eebee-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="eebee-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="eebee-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="eebee-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eebee-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="eebee-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="eebee-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="eebee-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eebee-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="eebee-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eebee-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eebee-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eebee-119">Not supported.</span></span>|
|<span data-ttu-id="eebee-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eebee-120">Application</span></span>|<span data-ttu-id="eebee-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eebee-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eebee-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eebee-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="eebee-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eebee-123">Request headers</span></span>
|<span data-ttu-id="eebee-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eebee-124">Header</span></span>|<span data-ttu-id="eebee-125">Wert</span><span class="sxs-lookup"><span data-stu-id="eebee-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eebee-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="eebee-126">Authorization</span></span>|<span data-ttu-id="eebee-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eebee-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eebee-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eebee-128">Accept</span></span>|<span data-ttu-id="eebee-129">application/json</span><span class="sxs-lookup"><span data-stu-id="eebee-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eebee-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eebee-130">Request body</span></span>
<span data-ttu-id="eebee-131">Geben Sie im Anforderungstext eine JSON-Darstellung für das [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="eebee-131">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="eebee-132">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="eebee-132">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="eebee-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eebee-133">Property</span></span>|<span data-ttu-id="eebee-134">Typ</span><span class="sxs-lookup"><span data-stu-id="eebee-134">Type</span></span>|<span data-ttu-id="eebee-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eebee-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eebee-136">id</span><span class="sxs-lookup"><span data-stu-id="eebee-136">id</span></span>|<span data-ttu-id="eebee-137">String</span><span class="sxs-lookup"><span data-stu-id="eebee-137">String</span></span>|<span data-ttu-id="eebee-138">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="eebee-138">The GUID for the object</span></span>|
|<span data-ttu-id="eebee-139">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="eebee-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="eebee-140">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="eebee-140">additionalInformation</span></span>|<span data-ttu-id="eebee-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="eebee-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="eebee-142">Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen zum Problem Behandlungs Ereignis bieten.</span><span class="sxs-lookup"><span data-stu-id="eebee-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="eebee-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="eebee-143">applicationId</span></span>|<span data-ttu-id="eebee-144">String</span><span class="sxs-lookup"><span data-stu-id="eebee-144">String</span></span>|<span data-ttu-id="eebee-145">InTune-Anwendungsbezeichner.</span><span class="sxs-lookup"><span data-stu-id="eebee-145">Intune application identifier.</span></span>|
|<span data-ttu-id="eebee-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="eebee-146">correlationId</span></span>|<span data-ttu-id="eebee-147">String</span><span class="sxs-lookup"><span data-stu-id="eebee-147">String</span></span>|<span data-ttu-id="eebee-148">ID, die zum Nachverfolgen des Fehlers im Dienst verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="eebee-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="eebee-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="eebee-149">eventDateTime</span></span>|<span data-ttu-id="eebee-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eebee-150">DateTimeOffset</span></span>|<span data-ttu-id="eebee-151">Zeitpunkt, zu dem das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="eebee-151">Time when the event occurred.</span></span> |
|<span data-ttu-id="eebee-152">eventName</span><span class="sxs-lookup"><span data-stu-id="eebee-152">eventName</span></span>|<span data-ttu-id="eebee-153">String</span><span class="sxs-lookup"><span data-stu-id="eebee-153">String</span></span>|<span data-ttu-id="eebee-154">Ereignis Name, der dem Problem Behandlungs Ereignis entspricht.</span><span class="sxs-lookup"><span data-stu-id="eebee-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="eebee-155">Optional.</span><span class="sxs-lookup"><span data-stu-id="eebee-155">Optional.</span></span>|
|<span data-ttu-id="eebee-156">Geschichte</span><span class="sxs-lookup"><span data-stu-id="eebee-156">history</span></span>|<span data-ttu-id="eebee-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="eebee-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="eebee-158">InTune-Problembehandlung für mobile Anwendungen.</span><span class="sxs-lookup"><span data-stu-id="eebee-158">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="eebee-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="eebee-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="eebee-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eebee-160">String</span></span>|<span data-ttu-id="eebee-161">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="eebee-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="eebee-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="eebee-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="eebee-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="eebee-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="eebee-164">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="eebee-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="eebee-165">userId</span><span class="sxs-lookup"><span data-stu-id="eebee-165">userId</span></span>|<span data-ttu-id="eebee-166">String</span><span class="sxs-lookup"><span data-stu-id="eebee-166">String</span></span>|<span data-ttu-id="eebee-167">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="eebee-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="eebee-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="eebee-168">Response</span></span>
<span data-ttu-id="eebee-169">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eebee-169">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eebee-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eebee-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="eebee-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eebee-171">Request</span></span>
<span data-ttu-id="eebee-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eebee-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="eebee-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="eebee-173">Response</span></span>
<span data-ttu-id="eebee-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eebee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




