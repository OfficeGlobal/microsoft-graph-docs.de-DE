# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="a2e82-101">Aktualisieren von „applePushNotificationCertificate“</span><span class="sxs-lookup"><span data-stu-id="a2e82-101">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="a2e82-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a2e82-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2e82-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="a2e82-103">Update the properties of a [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2e82-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a2e82-104">Prerequisites</span></span>
<span data-ttu-id="a2e82-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2e82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2e82-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2e82-107">Permission type</span></span>|<span data-ttu-id="a2e82-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2e82-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2e82-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2e82-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a2e82-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e82-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a2e82-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2e82-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2e82-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2e82-112">Not supported.</span></span>|
|<span data-ttu-id="a2e82-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2e82-113">Application</span></span>|<span data-ttu-id="a2e82-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2e82-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2e82-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2e82-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="a2e82-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2e82-116">Request headers</span></span>
|<span data-ttu-id="a2e82-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a2e82-117">Header</span></span>|<span data-ttu-id="a2e82-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a2e82-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2e82-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a2e82-119">Authorization</span></span>|<span data-ttu-id="a2e82-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a2e82-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2e82-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="a2e82-121">Accept</span></span>|<span data-ttu-id="a2e82-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="a2e82-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2e82-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2e82-123">Request body</span></span>
<span data-ttu-id="a2e82-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) an.</span><span class="sxs-lookup"><span data-stu-id="a2e82-124">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="a2e82-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a2e82-125">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="a2e82-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2e82-126">Property</span></span>|<span data-ttu-id="a2e82-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a2e82-127">Type</span></span>|<span data-ttu-id="a2e82-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2e82-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e82-129">ID</span><span class="sxs-lookup"><span data-stu-id="a2e82-129">id</span></span>|<span data-ttu-id="a2e82-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2e82-130">String</span></span>|<span data-ttu-id="a2e82-131">Eindeutiger Bezeichner für das Zertifikat</span><span class="sxs-lookup"><span data-stu-id="a2e82-131">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="a2e82-132">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="a2e82-132">appleIdentifier</span></span>|<span data-ttu-id="a2e82-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2e82-133">String</span></span>|<span data-ttu-id="a2e82-134">Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="a2e82-134">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="a2e82-135">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="a2e82-135">topicIdentifier</span></span>|<span data-ttu-id="a2e82-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2e82-136">String</span></span>|<span data-ttu-id="a2e82-137">Thema-ID</span><span class="sxs-lookup"><span data-stu-id="a2e82-137">Topic Id.</span></span>|
|<span data-ttu-id="a2e82-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2e82-138">lastModifiedDateTime</span></span>|<span data-ttu-id="a2e82-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2e82-139">DateTimeOffset</span></span>|<span data-ttu-id="a2e82-140">Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="a2e82-140">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a2e82-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a2e82-141">expirationDateTime</span></span>|<span data-ttu-id="a2e82-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2e82-142">DateTimeOffset</span></span>|<span data-ttu-id="a2e82-143">Datum und Uhrzeit des Ablaufs des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="a2e82-143">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a2e82-144">certificate</span><span class="sxs-lookup"><span data-stu-id="a2e82-144">certificate</span></span>|<span data-ttu-id="a2e82-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2e82-145">String</span></span>|<span data-ttu-id="a2e82-146">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a2e82-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a2e82-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2e82-147">Response</span></span>
<span data-ttu-id="a2e82-148">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a2e82-148">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2e82-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2e82-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2e82-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2e82-150">Request</span></span>
<span data-ttu-id="a2e82-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2e82-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 264

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="a2e82-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2e82-152">Response</span></span>
<span data-ttu-id="a2e82-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2e82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```








