# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="875fd-101">Funktion „downloadApplePushNotificationCertificateSigningRequest“</span><span class="sxs-lookup"><span data-stu-id="875fd-101">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="875fd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="875fd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="875fd-103">Diese Funktion lädt die Signieranforderung für das Apple Push Notification-Zertifikat herunter.</span><span class="sxs-lookup"><span data-stu-id="875fd-103">Download Apple push notification certificate signing request</span></span>
## <a name="prerequisites"></a><span data-ttu-id="875fd-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="875fd-104">Prerequisites</span></span>
<span data-ttu-id="875fd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="875fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="875fd-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="875fd-107">Permission type</span></span>|<span data-ttu-id="875fd-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="875fd-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="875fd-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="875fd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="875fd-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="875fd-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="875fd-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="875fd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="875fd-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="875fd-112">Not supported.</span></span>|
|<span data-ttu-id="875fd-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="875fd-113">Application</span></span>|<span data-ttu-id="875fd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="875fd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="875fd-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="875fd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="875fd-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="875fd-116">Request headers</span></span>
|<span data-ttu-id="875fd-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="875fd-117">Header</span></span>|<span data-ttu-id="875fd-118">Wert</span><span class="sxs-lookup"><span data-stu-id="875fd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="875fd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="875fd-119">Authorization</span></span>|<span data-ttu-id="875fd-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="875fd-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="875fd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="875fd-121">Accept</span></span>|<span data-ttu-id="875fd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="875fd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="875fd-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="875fd-123">Request body</span></span>
<span data-ttu-id="875fd-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="875fd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="875fd-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="875fd-125">Response</span></span>
<span data-ttu-id="875fd-126">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="875fd-126">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="875fd-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="875fd-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="875fd-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="875fd-128">Request</span></span>
<span data-ttu-id="875fd-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="875fd-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="875fd-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="875fd-130">Response</span></span>
<span data-ttu-id="875fd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="875fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```



