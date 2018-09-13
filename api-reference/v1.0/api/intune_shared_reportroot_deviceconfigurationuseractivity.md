# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="c95bb-101">Funktion „deviceConfigurationUserActivity“</span><span class="sxs-lookup"><span data-stu-id="c95bb-101">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="c95bb-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c95bb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c95bb-103">Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="c95bb-103">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c95bb-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c95bb-104">Prerequisites</span></span>
<span data-ttu-id="c95bb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c95bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c95bb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c95bb-107">Permission type</span></span>|<span data-ttu-id="c95bb-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c95bb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c95bb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c95bb-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c95bb-110">&nbsp; &nbsp; deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c95bb-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="c95bb-111">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c95bb-111">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c95bb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c95bb-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c95bb-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c95bb-113">Not supported.</span></span>|
|<span data-ttu-id="c95bb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c95bb-114">Application</span></span>|<span data-ttu-id="c95bb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c95bb-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c95bb-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c95bb-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="c95bb-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c95bb-117">Request headers</span></span>
|<span data-ttu-id="c95bb-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c95bb-118">Header</span></span>|<span data-ttu-id="c95bb-119">Wert</span><span class="sxs-lookup"><span data-stu-id="c95bb-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c95bb-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c95bb-120">Authorization</span></span>|<span data-ttu-id="c95bb-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c95bb-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c95bb-122">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="c95bb-122">Accept</span></span>|<span data-ttu-id="c95bb-123">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="c95bb-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c95bb-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c95bb-124">Request body</span></span>
<span data-ttu-id="c95bb-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c95bb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c95bb-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="c95bb-126">Response</span></span>
<span data-ttu-id="c95bb-127">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune_shared_report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c95bb-127">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c95bb-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c95bb-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="c95bb-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c95bb-129">Request</span></span>
<span data-ttu-id="c95bb-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c95bb-130">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="c95bb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c95bb-131">Response</span></span>
<span data-ttu-id="c95bb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c95bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








