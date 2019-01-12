---
title: Aktualisieren von „deviceManagement“
description: Aktualisieren der Eigenschaften eines deviceManagement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e7351eb15a194c68c4bd3b7abc59d866b5f4f237
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985970"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="892ae-103">Aktualisieren von „deviceManagement“</span><span class="sxs-lookup"><span data-stu-id="892ae-103">Update deviceManagement</span></span>

> <span data-ttu-id="892ae-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="892ae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="892ae-105">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="892ae-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="892ae-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="892ae-106">Prerequisites</span></span>
<span data-ttu-id="892ae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="892ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="892ae-109">Berechtigung&nbsp;Typ&nbsp;(durch&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="892ae-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="892ae-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="892ae-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="892ae-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="892ae-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="892ae-112">&nbsp;&nbsp; Überwachung</span><span class="sxs-lookup"><span data-stu-id="892ae-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="892ae-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-114">&nbsp;&nbsp; Begriffe des Unternehmens</span><span class="sxs-lookup"><span data-stu-id="892ae-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="892ae-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-116">&nbsp;&nbsp; Corporate Registrierung</span><span class="sxs-lookup"><span data-stu-id="892ae-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="892ae-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="892ae-118">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="892ae-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="892ae-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-120">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="892ae-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="892ae-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-122">&nbsp;&nbsp; Endpoint Protection.</span><span class="sxs-lookup"><span data-stu-id="892ae-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="892ae-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-124">&nbsp;&nbsp; Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="892ae-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="892ae-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-126">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="892ae-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="892ae-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-128">&nbsp;&nbsp; Rollenbasierte Zugriffssteuerung</span><span class="sxs-lookup"><span data-stu-id="892ae-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="892ae-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-130">&nbsp;&nbsp; Remoteunterstützung</span><span class="sxs-lookup"><span data-stu-id="892ae-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="892ae-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-132">&nbsp;&nbsp; Telekommunikation Ausgaben Management</span><span class="sxs-lookup"><span data-stu-id="892ae-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="892ae-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-134">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="892ae-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="892ae-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-136">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="892ae-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="892ae-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ae-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="892ae-138">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="892ae-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="892ae-139">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="892ae-139">Not supported.</span></span>|
| <span data-ttu-id="892ae-140">Anwendung</span><span class="sxs-lookup"><span data-stu-id="892ae-140">Application</span></span> | <span data-ttu-id="892ae-141">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="892ae-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="892ae-142">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="892ae-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="892ae-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="892ae-143">Request headers</span></span>
|<span data-ttu-id="892ae-144">Header</span><span class="sxs-lookup"><span data-stu-id="892ae-144">Header</span></span>|<span data-ttu-id="892ae-145">Wert</span><span class="sxs-lookup"><span data-stu-id="892ae-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="892ae-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="892ae-146">Authorization</span></span>|<span data-ttu-id="892ae-147">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="892ae-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="892ae-148">Annehmen</span><span class="sxs-lookup"><span data-stu-id="892ae-148">Accept</span></span>|<span data-ttu-id="892ae-149">application/json</span><span class="sxs-lookup"><span data-stu-id="892ae-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="892ae-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="892ae-150">Request body</span></span>
<span data-ttu-id="892ae-151">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="892ae-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="892ae-152">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="892ae-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="892ae-153">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="892ae-153">Property</span></span>|<span data-ttu-id="892ae-154">Typ</span><span class="sxs-lookup"><span data-stu-id="892ae-154">Type</span></span>|<span data-ttu-id="892ae-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="892ae-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="892ae-156">id</span><span class="sxs-lookup"><span data-stu-id="892ae-156">id</span></span>|<span data-ttu-id="892ae-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="892ae-157">String</span></span>|<span data-ttu-id="892ae-158">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="892ae-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="892ae-159">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="892ae-159">**Device configuration**</span></span>|
|<span data-ttu-id="892ae-160">settings</span><span class="sxs-lookup"><span data-stu-id="892ae-160">settings</span></span>|[<span data-ttu-id="892ae-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="892ae-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="892ae-162">Einstellungen auf Kontoebene</span><span class="sxs-lookup"><span data-stu-id="892ae-162">Account level settings.</span></span>|
|<span data-ttu-id="892ae-163">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="892ae-163">**Device management**</span></span>|
|<span data-ttu-id="892ae-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="892ae-164">subscriptionState</span></span>|[<span data-ttu-id="892ae-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="892ae-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="892ae-166">Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="892ae-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="892ae-167">Die möglichen Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="892ae-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="892ae-168">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="892ae-168">**Onboarding**</span></span>|
|<span data-ttu-id="892ae-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="892ae-169">intuneBrand</span></span>|[<span data-ttu-id="892ae-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="892ae-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="892ae-171">„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.</span><span class="sxs-lookup"><span data-stu-id="892ae-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="892ae-172">Anforderung Body-Eigenschaft Unterstützung variiert je nach Workflow.</span><span class="sxs-lookup"><span data-stu-id="892ae-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="892ae-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="892ae-173">Response</span></span>
<span data-ttu-id="892ae-174">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="892ae-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="892ae-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="892ae-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="892ae-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="892ae-176">Request</span></span>
<span data-ttu-id="892ae-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="892ae-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a><span data-ttu-id="892ae-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="892ae-178">Response</span></span>

<span data-ttu-id="892ae-179">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="892ae-179">Here is an example of the response.</span></span> <span data-ttu-id="892ae-180">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="892ae-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="892ae-181">Zurückgegebene Eigenschaften variieren je nach Workflow und Kontext.</span><span class="sxs-lookup"><span data-stu-id="892ae-181">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```



