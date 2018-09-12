# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="f2288-101">ManagedDeviceEnrollmentFailureDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="f2288-101">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="f2288-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f2288-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2288-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f2288-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2288-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f2288-104">Prerequisites</span></span>
<span data-ttu-id="f2288-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f2288-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2288-107">Permission type</span></span>|<span data-ttu-id="f2288-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2288-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2288-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2288-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f2288-110">&nbsp; &nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="f2288-110">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="f2288-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2288-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f2288-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2288-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2288-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2288-113">Not supported.</span></span>|
|<span data-ttu-id="f2288-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2288-114">Application</span></span>|<span data-ttu-id="f2288-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2288-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2288-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2288-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="f2288-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2288-117">Request headers</span></span>
|<span data-ttu-id="f2288-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f2288-118">Header</span></span>|<span data-ttu-id="f2288-119">Wert</span><span class="sxs-lookup"><span data-stu-id="f2288-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2288-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f2288-120">Authorization</span></span>|<span data-ttu-id="f2288-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f2288-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2288-122">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f2288-122">Accept</span></span>|<span data-ttu-id="f2288-123">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="f2288-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2288-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2288-124">Request body</span></span>
<span data-ttu-id="f2288-125">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="f2288-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f2288-126">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f2288-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f2288-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f2288-127">Property</span></span>|<span data-ttu-id="f2288-128">Typ</span><span class="sxs-lookup"><span data-stu-id="f2288-128">Type</span></span>|<span data-ttu-id="f2288-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2288-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2288-130">skip</span><span class="sxs-lookup"><span data-stu-id="f2288-130">skip</span></span>|<span data-ttu-id="f2288-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f2288-131">Int32</span></span>|<span data-ttu-id="f2288-132">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f2288-132">Not yet documented</span></span>|
|<span data-ttu-id="f2288-133">top</span><span class="sxs-lookup"><span data-stu-id="f2288-133">top</span></span>|<span data-ttu-id="f2288-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f2288-134">Int32</span></span>|<span data-ttu-id="f2288-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f2288-135">Not yet documented</span></span>|
|<span data-ttu-id="f2288-136">filter</span><span class="sxs-lookup"><span data-stu-id="f2288-136">filter</span></span>|<span data-ttu-id="f2288-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2288-137">String</span></span>|<span data-ttu-id="f2288-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f2288-138">Not yet documented</span></span>|
|<span data-ttu-id="f2288-139">skipToken</span><span class="sxs-lookup"><span data-stu-id="f2288-139">skipToken</span></span>|<span data-ttu-id="f2288-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2288-140">String</span></span>|<span data-ttu-id="f2288-141">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f2288-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f2288-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2288-142">Response</span></span>
<span data-ttu-id="f2288-143">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune_shared_report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f2288-143">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2288-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2288-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2288-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2288-145">Request</span></span>
<span data-ttu-id="f2288-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2288-146">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f2288-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2288-147">Response</span></span>
<span data-ttu-id="f2288-148">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="f2288-148">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f2288-149">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2288-149">All of the properties will be returned from an actual call.</span></span>

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




