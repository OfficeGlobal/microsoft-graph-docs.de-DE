# <a name="get-devicemanagement"></a><span data-ttu-id="8bb68-101">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="8bb68-101">Get deviceManagement</span></span>

> <span data-ttu-id="8bb68-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8bb68-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bb68-103">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_shared_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8bb68-103">Read properties and relationships of the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8bb68-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8bb68-104">Prerequisites</span></span>
<span data-ttu-id="8bb68-p101">Eine der nachfolgenden Berechtigungen ist zum Aufrufen dieser API erforderlich. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8bb68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="8bb68-107">Berechtigung &nbsp; Typ &nbsp; (vom Workflow &nbsp;)</span><span class="sxs-lookup"><span data-stu-id="8bb68-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="8bb68-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8bb68-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="8bb68-109">Delegiert (Arbeits- oder Schulkonto)</span><span class="sxs-lookup"><span data-stu-id="8bb68-109">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="8bb68-110">&nbsp; &nbsp; Überwachung</span><span class="sxs-lookup"><span data-stu-id="8bb68-110">&nbsp; &nbsp;Auditing</span></span> | <span data-ttu-id="8bb68-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="8bb68-112">&nbsp; &nbsp; Unternehmensbedingungen:</span><span class="sxs-lookup"><span data-stu-id="8bb68-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="8bb68-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8bb68-114">&nbsp; &nbsp; Aufgabe für die Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="8bb68-114">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="8bb68-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="8bb68-116">&nbsp; &nbsp; Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="8bb68-116">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="8bb68-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="8bb68-118">&nbsp; &nbsp; Registrierung</span><span class="sxs-lookup"><span data-stu-id="8bb68-118">&nbsp; &nbsp;Enrollment</span></span> | <span data-ttu-id="8bb68-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8bb68-120">&nbsp; &nbsp; Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="8bb68-120">NOTIFICATION</span></span> | <span data-ttu-id="8bb68-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8bb68-122">&nbsp; &nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="8bb68-122">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="8bb68-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8bb68-124">&nbsp; &nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="8bb68-124">&nbsp; &nbsp;RBAC</span></span> | <span data-ttu-id="8bb68-125">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-125">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="8bb68-126">&nbsp; &nbsp; Remote-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="8bb68-126">remote assistance,</span></span> | <span data-ttu-id="8bb68-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8bb68-128">&nbsp; &nbsp; Telecom-Spesenverwaltung</span><span class="sxs-lookup"><span data-stu-id="8bb68-128">&nbsp; &nbsp;Telecom expense management partner</span></span> | <span data-ttu-id="8bb68-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8bb68-130">&nbsp; &nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="8bb68-130">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="8bb68-131">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-131">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="8bb68-132">&nbsp; &nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="8bb68-132">Windows information protection</span></span> | <span data-ttu-id="8bb68-133">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb68-133">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="8bb68-134">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8bb68-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb68-135">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8bb68-135">Not supported.</span></span>|
| <span data-ttu-id="8bb68-136">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8bb68-136">Application</span></span> | <span data-ttu-id="8bb68-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8bb68-137">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="8bb68-138">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bb68-138">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8bb68-139">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8bb68-139">Optional query parameters</span></span>
<span data-ttu-id="8bb68-140">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8bb68-140">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8bb68-141">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8bb68-141">Request headers</span></span>
|<span data-ttu-id="8bb68-142">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8bb68-142">Header</span></span>|<span data-ttu-id="8bb68-143">Wert</span><span class="sxs-lookup"><span data-stu-id="8bb68-143">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bb68-144">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8bb68-144">Authorization</span></span>|<span data-ttu-id="8bb68-145">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8bb68-145">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bb68-146">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="8bb68-146">Accept</span></span>|<span data-ttu-id="8bb68-147">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="8bb68-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bb68-148">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8bb68-148">Request body</span></span>
<span data-ttu-id="8bb68-149">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8bb68-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bb68-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bb68-150">Response</span></span>
<span data-ttu-id="8bb68-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8bb68-151">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bb68-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8bb68-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="8bb68-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bb68-153">Request</span></span>
<span data-ttu-id="8bb68-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8bb68-154">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="8bb68-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bb68-155">Response</span></span>
<span data-ttu-id="8bb68-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8bb68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
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
}
```



