# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="2a7f2-101">Erstellen von mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="2a7f2-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="2a7f2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a7f2-103">Erstellt neue Objekte des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f2-103">Create a new [plannerBucket](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a7f2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2a7f2-104">Prerequisites</span></span>
<span data-ttu-id="2a7f2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a7f2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a7f2-107">Permission type</span></span>|<span data-ttu-id="2a7f2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a7f2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a7f2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a7f2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a7f2-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a7f2-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a7f2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a7f2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a7f2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a7f2-112">Not supported.</span></span>|
|<span data-ttu-id="2a7f2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a7f2-113">Application</span></span>|<span data-ttu-id="2a7f2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a7f2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a7f2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a7f2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="2a7f2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a7f2-116">Request headers</span></span>
|<span data-ttu-id="2a7f2-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2a7f2-117">Header</span></span>|<span data-ttu-id="2a7f2-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2a7f2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a7f2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a7f2-119">Authorization</span></span>|<span data-ttu-id="2a7f2-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a7f2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a7f2-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2a7f2-121">Accept</span></span>|<span data-ttu-id="2a7f2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2a7f2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a7f2-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a7f2-123">Request body</span></span>
<span data-ttu-id="2a7f2-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs mobileThreatDefenseConnector an.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="2a7f2-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs mobileThreatDefenseConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="2a7f2-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a7f2-126">Property</span></span>|<span data-ttu-id="2a7f2-127">Typ</span><span class="sxs-lookup"><span data-stu-id="2a7f2-127">Type</span></span>|<span data-ttu-id="2a7f2-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a7f2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a7f2-129">id</span><span class="sxs-lookup"><span data-stu-id="2a7f2-129">id</span></span>|<span data-ttu-id="2a7f2-130">String</span><span class="sxs-lookup"><span data-stu-id="2a7f2-130">String</span></span>|<span data-ttu-id="2a7f2-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2a7f2-131">Not yet documented</span></span>|
|<span data-ttu-id="2a7f2-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="2a7f2-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="2a7f2-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a7f2-133">DateTimeOffset</span></span>|<span data-ttu-id="2a7f2-134">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to MTP“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="2a7f2-134">Timestamp of last heartbeat after admin enabled option Connect to MTP</span></span>|
|<span data-ttu-id="2a7f2-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="2a7f2-135">partnerState</span></span>|<span data-ttu-id="2a7f2-136">String</span><span class="sxs-lookup"><span data-stu-id="2a7f2-136">String</span></span>|<span data-ttu-id="2a7f2-137">Partnerstatus des Mandanten. Mögliche Werte sind: `unavailable`, `available`, `enabled` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-137">Partner state of this tenant Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="2a7f2-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="2a7f2-138">androidEnabled</span></span>|<span data-ttu-id="2a7f2-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a7f2-139">Boolean</span></span>|<span data-ttu-id="2a7f2-140">Aktiviert oder deaktiviert Android.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-140">Android Toggle On or Off</span></span>|
|<span data-ttu-id="2a7f2-141">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2a7f2-141">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2a7f2-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a7f2-142">Boolean</span></span>|<span data-ttu-id="2a7f2-143">Für Android. Erlaubt es dem Administrator, festzulegen, dass Daten vom Datensynchronisierungspartner empfangen werden müssen, bevor Konformität angenommen wird.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-143">For Android, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="2a7f2-144">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2a7f2-144">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2a7f2-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a7f2-145">Boolean</span></span>|<span data-ttu-id="2a7f2-146">Für iOS. Erlaubt es dem Administrator, festzulegen, dass Daten vom Datensynchronisierungspartner empfangen werden müssen, bevor Konformität angenommen wird.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-146">For IOS, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="2a7f2-147">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="2a7f2-147">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="2a7f2-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a7f2-148">Boolean</span></span>|<span data-ttu-id="2a7f2-149">Erlaubt es dem Administrator, Geräte mit den aktivierten Plattformen zu blockieren, wenn sie die Mindestanforderungen an die Version nicht erfüllen.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-149">Allows admin to block devices on the enabled platforms that do not meet minimum version requirements</span></span>|
|<span data-ttu-id="2a7f2-150">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="2a7f2-150">iosEnabled</span></span>|<span data-ttu-id="2a7f2-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a7f2-151">Boolean</span></span>|<span data-ttu-id="2a7f2-152">Aktiviert oder deaktiviert iOS.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-152">IOS Toggle On or Off</span></span>|
|<span data-ttu-id="2a7f2-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="2a7f2-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="2a7f2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2a7f2-154">Int32</span></span>|<span data-ttu-id="2a7f2-155">Erlaubt das Abrufen oder das Festlegen des für die betreffende Partnerintegration geltenden Zeitraums in Tagen, während dessen ein Nichtreagieren des Mandanten toleriert wird.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="2a7f2-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a7f2-156">Response</span></span>
<span data-ttu-id="2a7f2-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-157">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a7f2-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a7f2-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a7f2-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a7f2-159">Request</span></span>
<span data-ttu-id="2a7f2-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="2a7f2-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a7f2-161">Response</span></span>
<span data-ttu-id="2a7f2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a7f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



