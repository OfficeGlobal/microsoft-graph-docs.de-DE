# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="2414f-101">verifyWindowsEnrollmentAutoDiscovery-Funktion</span><span class="sxs-lookup"><span data-stu-id="2414f-101">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="2414f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2414f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2414f-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2414f-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2414f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2414f-104">Prerequisites</span></span>
<span data-ttu-id="2414f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2414f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2414f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2414f-107">Permission type</span></span>|<span data-ttu-id="2414f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2414f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2414f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2414f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2414f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2414f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2414f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2414f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2414f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2414f-112">Not supported.</span></span>|
|<span data-ttu-id="2414f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2414f-113">Application</span></span>|<span data-ttu-id="2414f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2414f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2414f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2414f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="2414f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2414f-116">Request headers</span></span>
|<span data-ttu-id="2414f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2414f-117">Header</span></span>|<span data-ttu-id="2414f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2414f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2414f-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2414f-119">Authorization</span></span>|<span data-ttu-id="2414f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2414f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2414f-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="2414f-121">Accept</span></span>|<span data-ttu-id="2414f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2414f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2414f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2414f-123">Request body</span></span>
<span data-ttu-id="2414f-124">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="2414f-124">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2414f-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="2414f-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2414f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2414f-126">Property</span></span>|<span data-ttu-id="2414f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="2414f-127">Type</span></span>|<span data-ttu-id="2414f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2414f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2414f-129">Domänname</span><span class="sxs-lookup"><span data-stu-id="2414f-129">domainName</span></span>|<span data-ttu-id="2414f-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2414f-130">String</span></span>|<span data-ttu-id="2414f-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2414f-131">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="2414f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2414f-132">Response</span></span>
<span data-ttu-id="2414f-133">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und ein boolescher Wert im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2414f-133">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2414f-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2414f-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="2414f-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2414f-135">Request</span></span>
<span data-ttu-id="2414f-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2414f-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2414f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="2414f-137">Response</span></span>
<span data-ttu-id="2414f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2414f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



