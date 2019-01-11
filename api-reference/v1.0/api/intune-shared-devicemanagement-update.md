---
title: Aktualisieren von „deviceManagement“
description: Aktualisieren der Eigenschaften eines deviceManagement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e88b6379e340865adeb41bb0430fd8eecc8f0b69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860683"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="542df-103">Aktualisieren von „deviceManagement“</span><span class="sxs-lookup"><span data-stu-id="542df-103">Update deviceManagement</span></span>

> <span data-ttu-id="542df-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="542df-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="542df-105">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="542df-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="542df-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="542df-106">Prerequisites</span></span>
<span data-ttu-id="542df-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="542df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="542df-109">Berechtigung&nbsp;Typ&nbsp;(durch&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="542df-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="542df-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="542df-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="542df-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="542df-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="542df-112">&nbsp;&nbsp; Überwachung</span><span class="sxs-lookup"><span data-stu-id="542df-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="542df-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-114">&nbsp;&nbsp; Begriffe des Unternehmens</span><span class="sxs-lookup"><span data-stu-id="542df-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="542df-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-116">&nbsp;&nbsp; Corporate Registrierung</span><span class="sxs-lookup"><span data-stu-id="542df-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="542df-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="542df-118">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="542df-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="542df-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-120">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="542df-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="542df-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-122">&nbsp;&nbsp; Endpoint Protection.</span><span class="sxs-lookup"><span data-stu-id="542df-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="542df-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-124">&nbsp;&nbsp; Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="542df-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="542df-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-126">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="542df-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="542df-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-128">&nbsp;&nbsp; Rollenbasierte Zugriffssteuerung</span><span class="sxs-lookup"><span data-stu-id="542df-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="542df-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-130">&nbsp;&nbsp; Remoteunterstützung</span><span class="sxs-lookup"><span data-stu-id="542df-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="542df-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-132">&nbsp;&nbsp; Telekommunikation Ausgaben Management</span><span class="sxs-lookup"><span data-stu-id="542df-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="542df-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-134">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="542df-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="542df-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-136">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="542df-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="542df-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542df-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="542df-138">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="542df-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="542df-139">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="542df-139">Not supported.</span></span>|
| <span data-ttu-id="542df-140">Anwendung</span><span class="sxs-lookup"><span data-stu-id="542df-140">Application</span></span> | <span data-ttu-id="542df-141">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="542df-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="542df-142">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="542df-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="542df-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="542df-143">Request headers</span></span>
|<span data-ttu-id="542df-144">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="542df-144">Header</span></span>|<span data-ttu-id="542df-145">Wert</span><span class="sxs-lookup"><span data-stu-id="542df-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="542df-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="542df-146">Authorization</span></span>|<span data-ttu-id="542df-147">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="542df-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="542df-148">Annehmen</span><span class="sxs-lookup"><span data-stu-id="542df-148">Accept</span></span>|<span data-ttu-id="542df-149">application/json</span><span class="sxs-lookup"><span data-stu-id="542df-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="542df-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="542df-150">Request body</span></span>
<span data-ttu-id="542df-151">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="542df-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="542df-152">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="542df-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="542df-153">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="542df-153">Property</span></span>|<span data-ttu-id="542df-154">Typ</span><span class="sxs-lookup"><span data-stu-id="542df-154">Type</span></span>|<span data-ttu-id="542df-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="542df-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="542df-156">id</span><span class="sxs-lookup"><span data-stu-id="542df-156">id</span></span>|<span data-ttu-id="542df-157">String</span><span class="sxs-lookup"><span data-stu-id="542df-157">String</span></span>|<span data-ttu-id="542df-158">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="542df-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="542df-159">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="542df-159">**Device configuration**</span></span>|
|<span data-ttu-id="542df-160">settings</span><span class="sxs-lookup"><span data-stu-id="542df-160">settings</span></span>|[<span data-ttu-id="542df-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="542df-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="542df-162">Einstellungen auf Kontoebene</span><span class="sxs-lookup"><span data-stu-id="542df-162">Account level settings.</span></span>|
|<span data-ttu-id="542df-163">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="542df-163">**Device management**</span></span>|
|<span data-ttu-id="542df-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="542df-164">subscriptionState</span></span>|[<span data-ttu-id="542df-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="542df-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="542df-166">Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="542df-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="542df-167">Die möglichen Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="542df-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="542df-168">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="542df-168">**Onboarding**</span></span>|
|<span data-ttu-id="542df-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="542df-169">intuneBrand</span></span>|[<span data-ttu-id="542df-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="542df-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="542df-171">„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.</span><span class="sxs-lookup"><span data-stu-id="542df-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="542df-172">Anforderung Body-Eigenschaft Unterstützung variiert je nach Workflow.</span><span class="sxs-lookup"><span data-stu-id="542df-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="542df-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="542df-173">Response</span></span>
<span data-ttu-id="542df-174">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="542df-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="542df-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="542df-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="542df-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="542df-176">Request</span></span>
<span data-ttu-id="542df-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="542df-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="542df-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="542df-178">Response</span></span>

<span data-ttu-id="542df-179">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="542df-179">Here is an example of the response.</span></span> <span data-ttu-id="542df-180">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="542df-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="542df-181">Zurückgegebene Eigenschaften variieren je nach Workflow und Kontext.</span><span class="sxs-lookup"><span data-stu-id="542df-181">Returned properties vary according to workflow and context.</span></span>

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



