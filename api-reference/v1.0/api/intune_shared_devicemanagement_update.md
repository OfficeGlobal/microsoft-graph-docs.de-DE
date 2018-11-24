# <a name="update-devicemanagement"></a><span data-ttu-id="46e54-101">Aktualisieren von „deviceManagement“</span><span class="sxs-lookup"><span data-stu-id="46e54-101">Update deviceManagement</span></span>

> <span data-ttu-id="46e54-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="46e54-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46e54-103">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_shared_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="46e54-103">Update the properties of a [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46e54-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46e54-104">Prerequisites</span></span>
<span data-ttu-id="46e54-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="46e54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="46e54-107">Berechtigung&nbsp;Typ&nbsp;(durch&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="46e54-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="46e54-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46e54-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="46e54-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46e54-109">Delegated (work or school account)</span></span> |
| <span data-ttu-id="46e54-110">&nbsp;&nbsp; Überwachung</span><span class="sxs-lookup"><span data-stu-id="46e54-110">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="46e54-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-111">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-112">&nbsp;&nbsp; Begriffe des Unternehmens</span><span class="sxs-lookup"><span data-stu-id="46e54-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="46e54-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-113">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-114">&nbsp;&nbsp; Corporate Registrierung</span><span class="sxs-lookup"><span data-stu-id="46e54-114">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="46e54-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="46e54-116">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="46e54-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="46e54-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-117">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-118">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="46e54-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="46e54-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-120">&nbsp;&nbsp; Endpoint Protection.</span><span class="sxs-lookup"><span data-stu-id="46e54-120">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="46e54-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-122">&nbsp;&nbsp; Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="46e54-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="46e54-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-123">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-124">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="46e54-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="46e54-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-126">&nbsp;&nbsp; Rollenbasierte Zugriffssteuerung</span><span class="sxs-lookup"><span data-stu-id="46e54-126">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="46e54-127">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-127">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-128">&nbsp;&nbsp; Remoteunterstützung</span><span class="sxs-lookup"><span data-stu-id="46e54-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="46e54-129">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-129">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-130">&nbsp;&nbsp; Telekommunikation Ausgaben Management</span><span class="sxs-lookup"><span data-stu-id="46e54-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="46e54-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-132">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="46e54-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="46e54-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-133">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-134">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="46e54-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="46e54-135">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e54-135">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="46e54-136">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46e54-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46e54-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46e54-137">Not supported.</span></span>|
| <span data-ttu-id="46e54-138">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46e54-138">Application</span></span> | <span data-ttu-id="46e54-139">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46e54-139">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46e54-140">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46e54-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="46e54-141">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46e54-141">Request headers</span></span>
|<span data-ttu-id="46e54-142">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="46e54-142">Header</span></span>|<span data-ttu-id="46e54-143">Wert</span><span class="sxs-lookup"><span data-stu-id="46e54-143">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46e54-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="46e54-144">Authorization</span></span>|<span data-ttu-id="46e54-145">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="46e54-145">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46e54-146">Accept</span><span class="sxs-lookup"><span data-stu-id="46e54-146">Accept</span></span>|<span data-ttu-id="46e54-147">application/json</span><span class="sxs-lookup"><span data-stu-id="46e54-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46e54-148">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46e54-148">Request body</span></span>
<span data-ttu-id="46e54-149">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="46e54-149">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

<span data-ttu-id="46e54-150">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="46e54-150">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_shared_devicemanagement.md).</span></span>

|<span data-ttu-id="46e54-151">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46e54-151">Property</span></span>|<span data-ttu-id="46e54-152">Typ</span><span class="sxs-lookup"><span data-stu-id="46e54-152">Type</span></span>|<span data-ttu-id="46e54-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46e54-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46e54-154">id</span><span class="sxs-lookup"><span data-stu-id="46e54-154">id</span></span>|<span data-ttu-id="46e54-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46e54-155">String</span></span>|<span data-ttu-id="46e54-156">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="46e54-156">Unique Identifier for the device</span></span>|
|<span data-ttu-id="46e54-157">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="46e54-157">**Device configuration**</span></span>|
|<span data-ttu-id="46e54-158">settings</span><span class="sxs-lookup"><span data-stu-id="46e54-158">settings</span></span>|[<span data-ttu-id="46e54-159">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="46e54-159">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="46e54-160">Einstellungen auf Kontoebene</span><span class="sxs-lookup"><span data-stu-id="46e54-160">Account level settings.</span></span>|
|<span data-ttu-id="46e54-161">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="46e54-161">**Device management**</span></span>|
|<span data-ttu-id="46e54-162">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="46e54-162">subscriptionState</span></span>|[<span data-ttu-id="46e54-163">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="46e54-163">deviceManagementSubscriptionState</span></span>](../resources/intune_devices_devicemanagementsubscriptionstate.md)|<span data-ttu-id="46e54-164">Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="46e54-164">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="46e54-165">Die möglichen Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="46e54-165">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="46e54-166">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="46e54-166">**Onboarding**</span></span>|
|<span data-ttu-id="46e54-167">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="46e54-167">intuneBrand</span></span>|[<span data-ttu-id="46e54-168">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="46e54-168">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="46e54-169">„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.</span><span class="sxs-lookup"><span data-stu-id="46e54-169">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="46e54-170">Anforderung Body-Eigenschaft Unterstützung variiert je nach Workflow.</span><span class="sxs-lookup"><span data-stu-id="46e54-170">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="46e54-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="46e54-171">Response</span></span>
<span data-ttu-id="46e54-172">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="46e54-172">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46e54-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46e54-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="46e54-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46e54-174">Request</span></span>
<span data-ttu-id="46e54-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46e54-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46e54-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="46e54-176">Response</span></span>

<span data-ttu-id="46e54-177">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="46e54-177">Here is an example of the response.</span></span> <span data-ttu-id="46e54-178">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="46e54-178">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="46e54-179">Zurückgegebene Eigenschaften variieren je nach Workflow und Kontext.</span><span class="sxs-lookup"><span data-stu-id="46e54-179">Returned properties vary according to workflow and context.</span></span>

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



