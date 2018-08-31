# <a name="create-devicemanagementpartner"></a><span data-ttu-id="0ec16-101">deviceManagementPartner erstellen</span><span class="sxs-lookup"><span data-stu-id="0ec16-101">Create deviceManagementPartner</span></span>

> <span data-ttu-id="0ec16-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0ec16-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ec16-103">Erstellen eines neuen [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ec16-103">Create a new [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ec16-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0ec16-104">Prerequisites</span></span>
<span data-ttu-id="0ec16-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ec16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0ec16-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ec16-107">Permission type</span></span>|<span data-ttu-id="0ec16-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ec16-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ec16-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ec16-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0ec16-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ec16-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ec16-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ec16-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ec16-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ec16-112">Not supported.</span></span>|
|<span data-ttu-id="0ec16-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ec16-113">Application</span></span>|<span data-ttu-id="0ec16-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ec16-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ec16-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ec16-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="0ec16-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ec16-116">Request headers</span></span>
|<span data-ttu-id="0ec16-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0ec16-117">Header</span></span>|<span data-ttu-id="0ec16-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0ec16-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ec16-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0ec16-119">Authorization</span></span>|<span data-ttu-id="0ec16-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0ec16-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ec16-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0ec16-121">Accept</span></span>|<span data-ttu-id="0ec16-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="0ec16-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ec16-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ec16-123">Request body</span></span>
<span data-ttu-id="0ec16-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementPartner an.</span><span class="sxs-lookup"><span data-stu-id="0ec16-124">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="0ec16-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementPartner erstellen.</span><span class="sxs-lookup"><span data-stu-id="0ec16-125">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="0ec16-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0ec16-126">Property</span></span>|<span data-ttu-id="0ec16-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0ec16-127">Type</span></span>|<span data-ttu-id="0ec16-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ec16-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ec16-129">id</span><span class="sxs-lookup"><span data-stu-id="0ec16-129">id</span></span>|<span data-ttu-id="0ec16-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ec16-130">String</span></span>|<span data-ttu-id="0ec16-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0ec16-131">Not yet documented</span></span>|
|<span data-ttu-id="0ec16-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="0ec16-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="0ec16-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ec16-133">DateTimeOffset</span></span>|<span data-ttu-id="0ec16-134">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="0ec16-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="0ec16-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="0ec16-135">partnerState</span></span>|[<span data-ttu-id="0ec16-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="0ec16-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="0ec16-137">Partnerstatus des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0ec16-137">Partner state of this tenant Possible values are: , , , .</span></span> <span data-ttu-id="0ec16-138">Mögliche Werte: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="0ec16-138">The possible values are `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`, , , , , , or .</span></span>|
|<span data-ttu-id="0ec16-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="0ec16-139">partnerAppType</span></span>|[<span data-ttu-id="0ec16-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="0ec16-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="0ec16-141">Typ der Partneranwendung.</span><span class="sxs-lookup"><span data-stu-id="0ec16-141">Partner App Type.</span></span> <span data-ttu-id="0ec16-142">Mögliche Werte sind: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="0ec16-142">The possible values are `unknown`, `singleTenantApp`, `multiTenantApp`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="0ec16-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="0ec16-143">singleTenantAppId</span></span>|<span data-ttu-id="0ec16-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ec16-144">String</span></span>|<span data-ttu-id="0ec16-145">ID der Partner-App mit einem einzelnen Mandanten</span><span class="sxs-lookup"><span data-stu-id="0ec16-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="0ec16-146">displayName</span><span class="sxs-lookup"><span data-stu-id="0ec16-146">displayName</span></span>|<span data-ttu-id="0ec16-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ec16-147">String</span></span>|<span data-ttu-id="0ec16-148">Anzeigename für Partner</span><span class="sxs-lookup"><span data-stu-id="0ec16-148">Partner display name</span></span>|
|<span data-ttu-id="0ec16-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="0ec16-149">isConfigured</span></span>|<span data-ttu-id="0ec16-150">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0ec16-150">Boolean</span></span>|<span data-ttu-id="0ec16-151">Gibt an, ob Geräteverwaltungspartner konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="0ec16-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="0ec16-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ec16-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="0ec16-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ec16-153">DateTimeOffset</span></span>|<span data-ttu-id="0ec16-154">DateTime in UTC, zu der PartnerDevices entfernt werden</span><span class="sxs-lookup"><span data-stu-id="0ec16-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="0ec16-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="0ec16-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="0ec16-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ec16-156">DateTimeOffset</span></span>|<span data-ttu-id="0ec16-157">DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden</span><span class="sxs-lookup"><span data-stu-id="0ec16-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="0ec16-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ec16-158">Response</span></span>
<span data-ttu-id="0ec16-159">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ec16-159">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ec16-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ec16-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ec16-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ec16-161">Request</span></span>
<span data-ttu-id="0ec16-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ec16-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="0ec16-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ec16-163">Response</span></span>
<span data-ttu-id="0ec16-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ec16-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



