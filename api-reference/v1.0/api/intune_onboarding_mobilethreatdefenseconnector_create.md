# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="be54f-101">Erstellen von mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="be54f-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="be54f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="be54f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be54f-103">Erstellt neue Objekte des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="be54f-103">Create a new [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be54f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="be54f-104">Prerequisites</span></span>
<span data-ttu-id="be54f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="be54f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="be54f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be54f-107">Permission type</span></span>|<span data-ttu-id="be54f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be54f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be54f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be54f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="be54f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be54f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="be54f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be54f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be54f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be54f-112">Not supported.</span></span>|
|<span data-ttu-id="be54f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be54f-113">Application</span></span>|<span data-ttu-id="be54f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be54f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be54f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be54f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="be54f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be54f-116">Request headers</span></span>
|<span data-ttu-id="be54f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="be54f-117">Header</span></span>|<span data-ttu-id="be54f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="be54f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be54f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="be54f-119">Authorization</span></span>|<span data-ttu-id="be54f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="be54f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be54f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="be54f-121">Accept</span></span>|<span data-ttu-id="be54f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="be54f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be54f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be54f-123">Request body</span></span>
<span data-ttu-id="be54f-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs mobileThreatDefenseConnector an.</span><span class="sxs-lookup"><span data-stu-id="be54f-124">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="be54f-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs mobileThreatDefenseConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="be54f-125">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="be54f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be54f-126">Property</span></span>|<span data-ttu-id="be54f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="be54f-127">Type</span></span>|<span data-ttu-id="be54f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be54f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be54f-129">id</span><span class="sxs-lookup"><span data-stu-id="be54f-129">id</span></span>|<span data-ttu-id="be54f-130">String</span><span class="sxs-lookup"><span data-stu-id="be54f-130">String</span></span>|<span data-ttu-id="be54f-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="be54f-131">Not yet documented</span></span>|
|<span data-ttu-id="be54f-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="be54f-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="be54f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be54f-133">DateTimeOffset</span></span>|<span data-ttu-id="be54f-134">DateTime des letzten vom Datensynchronisierungspartner empfangenen Heartbeats</span><span class="sxs-lookup"><span data-stu-id="be54f-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="be54f-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="be54f-135">partnerState</span></span>|<span data-ttu-id="be54f-136">String</span><span class="sxs-lookup"><span data-stu-id="be54f-136">String</span></span>|<span data-ttu-id="be54f-137">Status des Datensynchronisierungspartners für dieses Konto. Mögliche Werte sind: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="be54f-137">Data Sync Partner state for this account Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="be54f-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="be54f-138">androidEnabled</span></span>|<span data-ttu-id="be54f-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="be54f-139">Boolean</span></span>|<span data-ttu-id="be54f-140">Legen Sie für Android fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="be54f-140">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="be54f-141">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="be54f-141">iosEnabled</span></span>|<span data-ttu-id="be54f-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="be54f-142">Boolean</span></span>|<span data-ttu-id="be54f-143">Für iOS: Rufen Sie ab oder legen Sie fest, ob Daten vom Datensynchronisierungspartner während der Konformitätsbewertung verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="be54f-143">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="be54f-144">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="be54f-144">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="be54f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="be54f-145">Boolean</span></span>|<span data-ttu-id="be54f-146">Für Android: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="be54f-146">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="be54f-147">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="be54f-147">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="be54f-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="be54f-148">Boolean</span></span>|<span data-ttu-id="be54f-149">Für iOS: Legen Sie fest, ob Intune Daten vom Datensynchronisierungspartner empfangen muss, bevor ein Gerät als kompatibel markiert wird.</span><span class="sxs-lookup"><span data-stu-id="be54f-149">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="be54f-150">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="be54f-150">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="be54f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="be54f-151">Boolean</span></span>|<span data-ttu-id="be54f-152">Rufen Sie ab bzw. legen Sie fest, ob Geräte auf den aktivierten Plattformen, die nicht die Mindestversionsanforderungen des Datensynchronisierungspartners erfüllen, blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="be54f-152">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="be54f-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="be54f-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="be54f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="be54f-154">Int32</span></span>|<span data-ttu-id="be54f-155">Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.</span><span class="sxs-lookup"><span data-stu-id="be54f-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="be54f-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="be54f-156">Response</span></span>
<span data-ttu-id="be54f-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="be54f-157">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be54f-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be54f-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="be54f-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be54f-159">Request</span></span>
<span data-ttu-id="be54f-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be54f-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be54f-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="be54f-161">Response</span></span>
<span data-ttu-id="be54f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be54f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



