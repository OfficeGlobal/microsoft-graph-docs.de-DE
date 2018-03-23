# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="9a97d-101">Funktion „deviceConfigurationUserActivity“</span><span class="sxs-lookup"><span data-stu-id="9a97d-101">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="9a97d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9a97d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a97d-103">Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="9a97d-103">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a97d-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9a97d-104">Prerequisites</span></span>
<span data-ttu-id="9a97d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a97d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a97d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a97d-107">Permission type</span></span>|<span data-ttu-id="9a97d-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a97d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a97d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a97d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9a97d-110">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a97d-110">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9a97d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a97d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a97d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a97d-112">Not supported.</span></span>|
|<span data-ttu-id="9a97d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a97d-113">Application</span></span>|<span data-ttu-id="9a97d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a97d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a97d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a97d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="9a97d-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a97d-116">Request headers</span></span>
|<span data-ttu-id="9a97d-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9a97d-117">Header</span></span>|<span data-ttu-id="9a97d-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9a97d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a97d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a97d-119">Authorization</span></span>|<span data-ttu-id="9a97d-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9a97d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9a97d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9a97d-121">Accept</span></span>|<span data-ttu-id="9a97d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9a97d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a97d-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a97d-123">Request body</span></span>
<span data-ttu-id="9a97d-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9a97d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a97d-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a97d-125">Response</span></span>
<span data-ttu-id="9a97d-126">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune_deviceconfig_report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9a97d-126">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/intune_deviceconfig_report.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a97d-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a97d-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a97d-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a97d-128">Request</span></span>
<span data-ttu-id="9a97d-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a97d-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="9a97d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a97d-130">Response</span></span>
<span data-ttu-id="9a97d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a97d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



