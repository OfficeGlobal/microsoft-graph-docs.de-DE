# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="cb8d2-101">Erstellen von mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="cb8d2-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="cb8d2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb8d2-103">Erstellt neue Objekte des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="cb8d2-103">Create a new [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb8d2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cb8d2-104">Prerequisites</span></span>
<span data-ttu-id="cb8d2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb8d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cb8d2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb8d2-107">Permission type</span></span>|<span data-ttu-id="cb8d2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb8d2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb8d2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb8d2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cb8d2-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb8d2-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cb8d2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb8d2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb8d2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb8d2-112">Not supported.</span></span>|
|<span data-ttu-id="cb8d2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb8d2-113">Application</span></span>|<span data-ttu-id="cb8d2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb8d2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb8d2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb8d2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="cb8d2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb8d2-116">Request headers</span></span>
|<span data-ttu-id="cb8d2-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cb8d2-117">Header</span></span>|<span data-ttu-id="cb8d2-118">Wert</span><span class="sxs-lookup"><span data-stu-id="cb8d2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb8d2-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cb8d2-119">Authorization</span></span>|<span data-ttu-id="cb8d2-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cb8d2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb8d2-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="cb8d2-121">Accept</span></span>|<span data-ttu-id="cb8d2-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="cb8d2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb8d2-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb8d2-123">Request body</span></span>
<span data-ttu-id="cb8d2-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs mobileThreatDefenseConnector an.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-124">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="cb8d2-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs mobileThreatDefenseConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-125">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="cb8d2-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb8d2-126">Property</span></span>|<span data-ttu-id="cb8d2-127">Typ</span><span class="sxs-lookup"><span data-stu-id="cb8d2-127">Type</span></span>|<span data-ttu-id="cb8d2-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb8d2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb8d2-129">id</span><span class="sxs-lookup"><span data-stu-id="cb8d2-129">id</span></span>|<span data-ttu-id="cb8d2-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb8d2-130">String</span></span>|<span data-ttu-id="cb8d2-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="cb8d2-131">Not yet documented</span></span>|
|<span data-ttu-id="cb8d2-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="cb8d2-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="cb8d2-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb8d2-133">DateTimeOffset</span></span>|<span data-ttu-id="cb8d2-134">DateTime des letzten vom Datensynchronisierungspartner empfangenen Heartbeats</span><span class="sxs-lookup"><span data-stu-id="cb8d2-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="cb8d2-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="cb8d2-135">partnerState</span></span>|[<span data-ttu-id="cb8d2-136">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="cb8d2-136">mobileThreatPartnerTenantState</span></span>](../resources/intune_onboarding_mobilethreatpartnertenantstate.md)|<span data-ttu-id="cb8d2-137">Daten Sync Partner-Zustand für dieses Konto.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-137">Data Sync Partner state for this account Possible values are: , , , .</span></span> <span data-ttu-id="cb8d2-138">Mögliche Werte sind: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-138">The possible values are `unavailable`, `available`, `enabled`, `unresponsive`, , , , , , , , or .</span></span>|
|<span data-ttu-id="cb8d2-139">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="cb8d2-139">androidEnabled</span></span>|<span data-ttu-id="cb8d2-140">boolesch</span><span class="sxs-lookup"><span data-stu-id="cb8d2-140">Boolean</span></span>|<span data-ttu-id="cb8d2-141">Legen Sie für Android fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-141">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="cb8d2-142">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="cb8d2-142">iosEnabled</span></span>|<span data-ttu-id="cb8d2-143">boolesch</span><span class="sxs-lookup"><span data-stu-id="cb8d2-143">Boolean</span></span>|<span data-ttu-id="cb8d2-144">Für iOS: Rufen Sie ab oder legen Sie fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-144">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="cb8d2-145">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="cb8d2-145">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="cb8d2-146">boolesch</span><span class="sxs-lookup"><span data-stu-id="cb8d2-146">Boolean</span></span>|<span data-ttu-id="cb8d2-147">Für Android: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-147">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="cb8d2-148">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="cb8d2-148">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="cb8d2-149">boolesch</span><span class="sxs-lookup"><span data-stu-id="cb8d2-149">Boolean</span></span>|<span data-ttu-id="cb8d2-150">Für iOS: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-150">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="cb8d2-151">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="cb8d2-151">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="cb8d2-152">boolesch</span><span class="sxs-lookup"><span data-stu-id="cb8d2-152">Boolean</span></span>|<span data-ttu-id="cb8d2-153">Rufen Sie ab bzw. legen Sie fest, ob Geräte auf den aktivierten Plattformen, die nicht die Mindestversionsanforderungen des Datensynchronisierungspartners erfüllen, blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-153">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="cb8d2-154">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="cb8d2-154">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="cb8d2-155">Int32</span><span class="sxs-lookup"><span data-stu-id="cb8d2-155">Int32</span></span>|<span data-ttu-id="cb8d2-156">Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-156">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="cb8d2-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb8d2-157">Response</span></span>
<span data-ttu-id="cb8d2-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-158">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb8d2-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb8d2-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb8d2-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb8d2-160">Request</span></span>
<span data-ttu-id="cb8d2-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="cb8d2-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb8d2-162">Response</span></span>
<span data-ttu-id="cb8d2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb8d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



