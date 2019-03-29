---
title: MobileAppTroubleshootingEvent erstellen
description: Beschreibt die CREATE mobileAppTroubleshootingEvent-Methode der Microsoft Graph-API für InTune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 89a191f94d68636226b6a8d41be0d9ba962da761
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979263"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="ab3a1-103">MobileAppTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="ab3a1-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="ab3a1-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab3a1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab3a1-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab3a1-107">Erstellen eines neuen [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab3a1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ab3a1-108">Prerequisites</span></span>
<span data-ttu-id="ab3a1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab3a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab3a1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ab3a1-111">Permission type</span></span>|<span data-ttu-id="ab3a1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ab3a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab3a1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ab3a1-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="ab3a1-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="ab3a1-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ab3a1-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab3a1-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ab3a1-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="ab3a1-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ab3a1-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab3a1-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ab3a1-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ab3a1-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab3a1-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab3a1-119">Not supported.</span></span>|
|<span data-ttu-id="ab3a1-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ab3a1-120">Application</span></span>|<span data-ttu-id="ab3a1-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab3a1-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab3a1-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab3a1-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="ab3a1-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ab3a1-123">Request headers</span></span>
|<span data-ttu-id="ab3a1-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ab3a1-124">Header</span></span>|<span data-ttu-id="ab3a1-125">Wert</span><span class="sxs-lookup"><span data-stu-id="ab3a1-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab3a1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab3a1-126">Authorization</span></span>|<span data-ttu-id="ab3a1-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ab3a1-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab3a1-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ab3a1-128">Accept</span></span>|<span data-ttu-id="ab3a1-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ab3a1-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab3a1-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ab3a1-130">Request body</span></span>
<span data-ttu-id="ab3a1-131">Geben Sie im Anforderungstext eine JSON-Darstellung für das mobileAppTroubleshootingEvent-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-131">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="ab3a1-132">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der mobileAppTroubleshootingEvent erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-132">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="ab3a1-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ab3a1-133">Property</span></span>|<span data-ttu-id="ab3a1-134">Typ</span><span class="sxs-lookup"><span data-stu-id="ab3a1-134">Type</span></span>|<span data-ttu-id="ab3a1-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab3a1-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab3a1-136">id</span><span class="sxs-lookup"><span data-stu-id="ab3a1-136">id</span></span>|<span data-ttu-id="ab3a1-137">String</span><span class="sxs-lookup"><span data-stu-id="ab3a1-137">String</span></span>|<span data-ttu-id="ab3a1-138">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="ab3a1-138">The GUID for the object</span></span>|
|<span data-ttu-id="ab3a1-139">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="ab3a1-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="ab3a1-140">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="ab3a1-140">additionalInformation</span></span>|<span data-ttu-id="ab3a1-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ab3a1-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ab3a1-142">Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen zum Problem Behandlungs Ereignis bieten.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="ab3a1-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="ab3a1-143">applicationId</span></span>|<span data-ttu-id="ab3a1-144">String</span><span class="sxs-lookup"><span data-stu-id="ab3a1-144">String</span></span>|<span data-ttu-id="ab3a1-145">InTune-Anwendungsbezeichner.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-145">Intune application identifier.</span></span>|
|<span data-ttu-id="ab3a1-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="ab3a1-146">correlationId</span></span>|<span data-ttu-id="ab3a1-147">String</span><span class="sxs-lookup"><span data-stu-id="ab3a1-147">String</span></span>|<span data-ttu-id="ab3a1-148">ID, die zum Nachverfolgen des Fehlers im Dienst verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="ab3a1-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="ab3a1-149">eventDateTime</span></span>|<span data-ttu-id="ab3a1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab3a1-150">DateTimeOffset</span></span>|<span data-ttu-id="ab3a1-151">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-151">Time when the event occurred .</span></span> |
|<span data-ttu-id="ab3a1-152">eventName</span><span class="sxs-lookup"><span data-stu-id="ab3a1-152">eventName</span></span>|<span data-ttu-id="ab3a1-153">String</span><span class="sxs-lookup"><span data-stu-id="ab3a1-153">String</span></span>|<span data-ttu-id="ab3a1-154">Ereignis Name, der dem Problem Behandlungs Ereignis entspricht.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="ab3a1-155">Optional.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-155">Optional.</span></span>|
|<span data-ttu-id="ab3a1-156">Geschichte</span><span class="sxs-lookup"><span data-stu-id="ab3a1-156">history</span></span>|<span data-ttu-id="ab3a1-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="ab3a1-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="ab3a1-158">InTune-Problem Behandlungs Historie für mobile Anwendungen</span><span class="sxs-lookup"><span data-stu-id="ab3a1-158">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="ab3a1-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ab3a1-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="ab3a1-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab3a1-160">String</span></span>|<span data-ttu-id="ab3a1-161">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="ab3a1-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="ab3a1-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ab3a1-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="ab3a1-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ab3a1-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="ab3a1-164">Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="ab3a1-165">userId</span><span class="sxs-lookup"><span data-stu-id="ab3a1-165">userId</span></span>|<span data-ttu-id="ab3a1-166">String</span><span class="sxs-lookup"><span data-stu-id="ab3a1-166">String</span></span>|<span data-ttu-id="ab3a1-167">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="ab3a1-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab3a1-168">Response</span></span>
<span data-ttu-id="ab3a1-169">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-169">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab3a1-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ab3a1-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab3a1-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab3a1-171">Request</span></span>
<span data-ttu-id="ab3a1-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="ab3a1-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab3a1-173">Response</span></span>
<span data-ttu-id="ab3a1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ab3a1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




