# <a name="update-devicemanagement"></a><span data-ttu-id="2f7f9-101">Aktualisieren von „deviceManagement“</span><span class="sxs-lookup"><span data-stu-id="2f7f9-101">Update deviceManagement</span></span>

> <span data-ttu-id="2f7f9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f7f9-103">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_shared_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-103">Update the properties of a [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f7f9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f7f9-104">Prerequisites</span></span>
<span data-ttu-id="2f7f9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f7f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="2f7f9-107">Berechtigung &nbsp; Typ &nbsp; (vom Workflow &nbsp;)</span><span class="sxs-lookup"><span data-stu-id="2f7f9-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="2f7f9-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f7f9-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="2f7f9-109">Delegiert (Geschäfts- oder Schulkonto)</span><span class="sxs-lookup"><span data-stu-id="2f7f9-109">Delegated (work or school account)</span></span> |
| <span data-ttu-id="2f7f9-110">&nbsp; &nbsp; Überwachung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-110">&nbsp; &nbsp;Auditing</span></span> | <span data-ttu-id="2f7f9-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-111">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-112">&nbsp; &nbsp; Unternehmensbedingungen</span><span class="sxs-lookup"><span data-stu-id="2f7f9-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="2f7f9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-114">&nbsp; &nbsp; Unternehmens-Registrierung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-114">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="2f7f9-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="2f7f9-116">&nbsp; &nbsp; Geräte-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="2f7f9-116">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="2f7f9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-117">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-118">&nbsp; &nbsp; Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-118">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="2f7f9-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-120">&nbsp; &nbsp; Endpunkt-Schutz</span><span class="sxs-lookup"><span data-stu-id="2f7f9-120">&nbsp; &nbsp;Endpoint Protection</span></span> | <span data-ttu-id="2f7f9-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-122">&nbsp; &nbsp; Registrierung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-122">&nbsp; &nbsp;Enrollment</span></span> | <span data-ttu-id="2f7f9-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-123">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-124">&nbsp; &nbsp; Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-124">&nbsp; &nbsp;Notification</span></span> | <span data-ttu-id="2f7f9-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-126">&nbsp; &nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="2f7f9-126">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="2f7f9-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-128">&nbsp; &nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="2f7f9-128">&nbsp; &nbsp;RBAC</span></span> | <span data-ttu-id="2f7f9-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-130">&nbsp; &nbsp; Remote-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-130">remote assistance,</span></span> | <span data-ttu-id="2f7f9-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-132">&nbsp; &nbsp; Telecom-Ausgaben-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-132">&nbsp; &nbsp;Telecom expense management partner</span></span> | <span data-ttu-id="2f7f9-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-134">&nbsp; &nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-134">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="2f7f9-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-136">&nbsp; &nbsp; Windows Information Schutz</span><span class="sxs-lookup"><span data-stu-id="2f7f9-136">Windows information protection</span></span> | <span data-ttu-id="2f7f9-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7f9-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="2f7f9-138">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f7f9-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f7f9-139">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f7f9-139">Not supported.</span></span>|
| <span data-ttu-id="2f7f9-140">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-140">Application</span></span> | <span data-ttu-id="2f7f9-141">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f7f9-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f7f9-142">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="2f7f9-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f7f9-143">Request headers</span></span>
|<span data-ttu-id="2f7f9-144">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f7f9-144">Header</span></span>|<span data-ttu-id="2f7f9-145">Wert</span><span class="sxs-lookup"><span data-stu-id="2f7f9-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f7f9-146">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-146">Authorization</span></span>|<span data-ttu-id="2f7f9-147">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f7f9-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f7f9-148">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="2f7f9-148">Accept</span></span>|<span data-ttu-id="2f7f9-149">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="2f7f9-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f7f9-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f7f9-150">Request body</span></span>
<span data-ttu-id="2f7f9-151">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

<span data-ttu-id="2f7f9-152">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_shared_devicemanagement.md).</span></span>

|<span data-ttu-id="2f7f9-153">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f7f9-153">Property</span></span>|<span data-ttu-id="2f7f9-154">Typ</span><span class="sxs-lookup"><span data-stu-id="2f7f9-154">Type</span></span>|<span data-ttu-id="2f7f9-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f7f9-156">ID</span><span class="sxs-lookup"><span data-stu-id="2f7f9-156">id</span></span>|<span data-ttu-id="2f7f9-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f7f9-157">String</span></span>|<span data-ttu-id="2f7f9-158">Eindeutiger Bezeichner für das Gerät</span><span class="sxs-lookup"><span data-stu-id="2f7f9-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="2f7f9-159">**Geräte-Konfiguration**</span><span class="sxs-lookup"><span data-stu-id="2f7f9-159">**Device configuration**</span></span>|
|<span data-ttu-id="2f7f9-160">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="2f7f9-160">settings</span></span>|[<span data-ttu-id="2f7f9-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="2f7f9-161">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="2f7f9-162">Einstellungen auf Kontoebene.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-162">Account level settings.</span></span>|
|<span data-ttu-id="2f7f9-163">**Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="2f7f9-163">**Device management**</span></span>|
|<span data-ttu-id="2f7f9-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="2f7f9-164">subscriptionState</span></span>|[<span data-ttu-id="2f7f9-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="2f7f9-165">deviceManagementSubscriptionState</span></span>](../resources/intune_devices_devicemanagementsubscriptionstate.md)|<span data-ttu-id="2f7f9-166">Zustand des Abonnements bei der Verwaltung des mobilen Gerätes des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="2f7f9-167">Mögliche Werte: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-167">The possible values are `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`, , , , , or .</span></span>|
|<span data-ttu-id="2f7f9-168">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="2f7f9-168">**On-boarding**</span></span>|
|<span data-ttu-id="2f7f9-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="2f7f9-169">intuneBrand</span></span>|[<span data-ttu-id="2f7f9-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="2f7f9-170">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="2f7f9-171">„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst werden.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="2f7f9-172">Die Anforderung des Body-Eigenschaft-Supports variiert je nach Workflow.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-172">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="2f7f9-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f7f9-173">Response</span></span>
<span data-ttu-id="2f7f9-174">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f7f9-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f7f9-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f7f9-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f7f9-176">Request</span></span>
<span data-ttu-id="2f7f9-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f7f9-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f7f9-178">Response</span></span>

<span data-ttu-id="2f7f9-179">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-179">Here is an example of the response.</span></span> <span data-ttu-id="2f7f9-180">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen gekürzt.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2f7f9-181">Zurückgegebene Eigenschaften variieren je nach Workflow und Kontext.</span><span class="sxs-lookup"><span data-stu-id="2f7f9-181">Returned properties vary according to workflow and context.</span></span>

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



