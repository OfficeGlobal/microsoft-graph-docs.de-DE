# <a name="update-devicemanagementpartner"></a><span data-ttu-id="80f50-101">deviceManagementPartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="80f50-101">Update deviceManagementPartner</span></span>

> <span data-ttu-id="80f50-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80f50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80f50-103">Aktualisieren der Eigenschaften eines [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="80f50-103">Update the properties of a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80f50-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80f50-104">Prerequisites</span></span>
<span data-ttu-id="80f50-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="80f50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80f50-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80f50-107">Permission type</span></span>|<span data-ttu-id="80f50-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80f50-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80f50-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80f50-109">Delegated (work or school account)</span></span>|<span data-ttu-id="80f50-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80f50-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="80f50-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80f50-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80f50-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80f50-112">Not supported.</span></span>|
|<span data-ttu-id="80f50-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80f50-113">Application</span></span>|<span data-ttu-id="80f50-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80f50-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80f50-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80f50-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="80f50-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80f50-116">Request headers</span></span>
|<span data-ttu-id="80f50-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="80f50-117">Header</span></span>|<span data-ttu-id="80f50-118">Wert</span><span class="sxs-lookup"><span data-stu-id="80f50-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80f50-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="80f50-119">Authorization</span></span>|<span data-ttu-id="80f50-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80f50-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80f50-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="80f50-121">Accept</span></span>|<span data-ttu-id="80f50-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="80f50-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80f50-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80f50-123">Request body</span></span>
<span data-ttu-id="80f50-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) an.</span><span class="sxs-lookup"><span data-stu-id="80f50-124">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="80f50-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="80f50-125">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span></span>

|<span data-ttu-id="80f50-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80f50-126">Property</span></span>|<span data-ttu-id="80f50-127">Typ</span><span class="sxs-lookup"><span data-stu-id="80f50-127">Type</span></span>|<span data-ttu-id="80f50-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80f50-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80f50-129">ID</span><span class="sxs-lookup"><span data-stu-id="80f50-129">id</span></span>|<span data-ttu-id="80f50-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f50-130">String</span></span>|<span data-ttu-id="80f50-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="80f50-131">Not yet documented</span></span>|
|<span data-ttu-id="80f50-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="80f50-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="80f50-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80f50-133">DateTimeOffset</span></span>|<span data-ttu-id="80f50-134">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="80f50-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="80f50-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="80f50-135">partnerState</span></span>|[<span data-ttu-id="80f50-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="80f50-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="80f50-137">Partnerstatus dieses Mandanten.</span><span class="sxs-lookup"><span data-stu-id="80f50-137">Partner state of this tenant Possible values are: , , , .</span></span> <span data-ttu-id="80f50-138">Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="80f50-138">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="80f50-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="80f50-139">partnerAppType</span></span>|[<span data-ttu-id="80f50-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="80f50-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="80f50-141">Typ der Partner-App.</span><span class="sxs-lookup"><span data-stu-id="80f50-141">Partner App Type.</span></span> <span data-ttu-id="80f50-142">Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="80f50-142">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="80f50-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="80f50-143">singleTenantAppId</span></span>|<span data-ttu-id="80f50-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f50-144">String</span></span>|<span data-ttu-id="80f50-145">ID der Partner-App mit einem einzelnen Mandanten</span><span class="sxs-lookup"><span data-stu-id="80f50-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="80f50-146">displayName</span><span class="sxs-lookup"><span data-stu-id="80f50-146">displayName</span></span>|<span data-ttu-id="80f50-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f50-147">String</span></span>|<span data-ttu-id="80f50-148">Anzeigename für Partner</span><span class="sxs-lookup"><span data-stu-id="80f50-148">Partner display name</span></span>|
|<span data-ttu-id="80f50-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="80f50-149">isConfigured</span></span>|<span data-ttu-id="80f50-150">Boolesch</span><span class="sxs-lookup"><span data-stu-id="80f50-150">Boolean</span></span>|<span data-ttu-id="80f50-151">Gibt an, ob Geräteverwaltungspartner konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="80f50-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="80f50-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="80f50-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="80f50-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80f50-153">DateTimeOffset</span></span>|<span data-ttu-id="80f50-154">DateTime in UTC, zu der PartnerDevices entfernt werden</span><span class="sxs-lookup"><span data-stu-id="80f50-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="80f50-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="80f50-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="80f50-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80f50-156">DateTimeOffset</span></span>|<span data-ttu-id="80f50-157">DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden</span><span class="sxs-lookup"><span data-stu-id="80f50-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="80f50-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="80f50-158">Response</span></span>
<span data-ttu-id="80f50-159">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80f50-159">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80f50-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80f50-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="80f50-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80f50-161">Request</span></span>
<span data-ttu-id="80f50-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80f50-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 440

{
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="80f50-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="80f50-163">Response</span></span>
<span data-ttu-id="80f50-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80f50-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```








