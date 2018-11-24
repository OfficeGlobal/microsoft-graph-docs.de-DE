# <a name="update-devicemanagementpartner"></a><span data-ttu-id="4a98b-101">deviceManagementPartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4a98b-101">Update deviceManagementPartner</span></span>

> <span data-ttu-id="4a98b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4a98b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a98b-103">Aktualisieren der Eigenschaften eines [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4a98b-103">Update the properties of a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a98b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4a98b-104">Prerequisites</span></span>
<span data-ttu-id="4a98b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a98b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a98b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a98b-107">Permission type</span></span>|<span data-ttu-id="4a98b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a98b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a98b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a98b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4a98b-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a98b-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4a98b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a98b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a98b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a98b-112">Not supported.</span></span>|
|<span data-ttu-id="4a98b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a98b-113">Application</span></span>|<span data-ttu-id="4a98b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a98b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a98b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a98b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="4a98b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a98b-116">Request headers</span></span>
|<span data-ttu-id="4a98b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4a98b-117">Header</span></span>|<span data-ttu-id="4a98b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4a98b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a98b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a98b-119">Authorization</span></span>|<span data-ttu-id="4a98b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4a98b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a98b-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4a98b-121">Accept</span></span>|<span data-ttu-id="4a98b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4a98b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a98b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a98b-123">Request body</span></span>
<span data-ttu-id="4a98b-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) an.</span><span class="sxs-lookup"><span data-stu-id="4a98b-124">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="4a98b-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4a98b-125">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span></span>

|<span data-ttu-id="4a98b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4a98b-126">Property</span></span>|<span data-ttu-id="4a98b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4a98b-127">Type</span></span>|<span data-ttu-id="4a98b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a98b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a98b-129">id</span><span class="sxs-lookup"><span data-stu-id="4a98b-129">id</span></span>|<span data-ttu-id="4a98b-130">String</span><span class="sxs-lookup"><span data-stu-id="4a98b-130">String</span></span>|<span data-ttu-id="4a98b-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4a98b-131">Not yet documented</span></span>|
|<span data-ttu-id="4a98b-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4a98b-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4a98b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a98b-133">DateTimeOffset</span></span>|<span data-ttu-id="4a98b-134">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="4a98b-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="4a98b-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="4a98b-135">partnerState</span></span>|[<span data-ttu-id="4a98b-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="4a98b-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="4a98b-137">Partner-Status, der diesen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4a98b-137">Partner state of this tenant.</span></span> <span data-ttu-id="4a98b-138">Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4a98b-138">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="4a98b-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="4a98b-139">partnerAppType</span></span>|[<span data-ttu-id="4a98b-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="4a98b-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="4a98b-141">Partner-App-Typ.</span><span class="sxs-lookup"><span data-stu-id="4a98b-141">Partner App type.</span></span> <span data-ttu-id="4a98b-142">Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="4a98b-142">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="4a98b-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="4a98b-143">singleTenantAppId</span></span>|<span data-ttu-id="4a98b-144">String</span><span class="sxs-lookup"><span data-stu-id="4a98b-144">String</span></span>|<span data-ttu-id="4a98b-145">ID der Partner-App mit einem einzelnen Mandanten</span><span class="sxs-lookup"><span data-stu-id="4a98b-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="4a98b-146">displayName</span><span class="sxs-lookup"><span data-stu-id="4a98b-146">displayName</span></span>|<span data-ttu-id="4a98b-147">String</span><span class="sxs-lookup"><span data-stu-id="4a98b-147">String</span></span>|<span data-ttu-id="4a98b-148">Anzeigename für Partner</span><span class="sxs-lookup"><span data-stu-id="4a98b-148">Partner display name</span></span>|
|<span data-ttu-id="4a98b-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="4a98b-149">isConfigured</span></span>|<span data-ttu-id="4a98b-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4a98b-150">Boolean</span></span>|<span data-ttu-id="4a98b-151">Gibt an, ob Geräteverwaltungspartner konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="4a98b-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="4a98b-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a98b-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="4a98b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a98b-153">DateTimeOffset</span></span>|<span data-ttu-id="4a98b-154">DateTime in UTC, zu der PartnerDevices entfernt werden</span><span class="sxs-lookup"><span data-stu-id="4a98b-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="4a98b-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="4a98b-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="4a98b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a98b-156">DateTimeOffset</span></span>|<span data-ttu-id="4a98b-157">DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden</span><span class="sxs-lookup"><span data-stu-id="4a98b-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="4a98b-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a98b-158">Response</span></span>
<span data-ttu-id="4a98b-159">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a98b-159">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a98b-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a98b-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a98b-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a98b-161">Request</span></span>
<span data-ttu-id="4a98b-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a98b-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
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

### <a name="response"></a><span data-ttu-id="4a98b-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a98b-163">Response</span></span>
<span data-ttu-id="4a98b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a98b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



