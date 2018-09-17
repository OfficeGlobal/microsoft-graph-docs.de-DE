# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="7bcfc-101">ManagedDeviceEnrollmentTopFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="7bcfc-101">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="7bcfc-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7bcfc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bcfc-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7bcfc-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7bcfc-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7bcfc-104">Prerequisites</span></span>
<span data-ttu-id="7bcfc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7bcfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7bcfc-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7bcfc-107">Permission type</span></span>|<span data-ttu-id="7bcfc-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7bcfc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bcfc-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7bcfc-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7bcfc-110">&nbsp; &nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="7bcfc-110">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="7bcfc-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bcfc-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7bcfc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7bcfc-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bcfc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7bcfc-113">Not supported.</span></span>|
|<span data-ttu-id="7bcfc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7bcfc-114">Application</span></span>|<span data-ttu-id="7bcfc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7bcfc-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bcfc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bcfc-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="7bcfc-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7bcfc-117">Request headers</span></span>
|<span data-ttu-id="7bcfc-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7bcfc-118">Header</span></span>|<span data-ttu-id="7bcfc-119">Wert</span><span class="sxs-lookup"><span data-stu-id="7bcfc-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bcfc-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7bcfc-120">Authorization</span></span>|<span data-ttu-id="7bcfc-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7bcfc-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bcfc-122">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="7bcfc-122">Accept</span></span>|<span data-ttu-id="7bcfc-123">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="7bcfc-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bcfc-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7bcfc-124">Request body</span></span>
<span data-ttu-id="7bcfc-125">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="7bcfc-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7bcfc-126">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="7bcfc-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7bcfc-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7bcfc-127">Property</span></span>|<span data-ttu-id="7bcfc-128">Typ</span><span class="sxs-lookup"><span data-stu-id="7bcfc-128">Type</span></span>|<span data-ttu-id="7bcfc-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bcfc-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bcfc-130">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7bcfc-130">period</span></span>|<span data-ttu-id="7bcfc-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7bcfc-131">String</span></span>|<span data-ttu-id="7bcfc-132">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7bcfc-132">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7bcfc-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bcfc-133">Response</span></span>
<span data-ttu-id="7bcfc-134">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune_shared_report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7bcfc-134">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bcfc-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7bcfc-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="7bcfc-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bcfc-136">Request</span></span>
<span data-ttu-id="7bcfc-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7bcfc-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7bcfc-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bcfc-138">Response</span></span>
<span data-ttu-id="7bcfc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7bcfc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




