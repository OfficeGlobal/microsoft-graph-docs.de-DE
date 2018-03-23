# <a name="requestsignupurl-action"></a><span data-ttu-id="01923-101">Aktion „requestSignupUrl“</span><span class="sxs-lookup"><span data-stu-id="01923-101">requestSignupUrl action</span></span>

> <span data-ttu-id="01923-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="01923-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01923-103">Diese Aktion generiert eine Registrierungs-URL, die zur Registrierung in der Android for Work-Verwaltung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="01923-103">Generates a sign-up URL that is used to enroll in Android for Work management.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01923-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="01923-104">Prerequisites</span></span>
<span data-ttu-id="01923-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01923-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01923-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="01923-107">Permission type</span></span>|<span data-ttu-id="01923-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="01923-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01923-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="01923-109">Delegated (work or school account)</span></span>|<span data-ttu-id="01923-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01923-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01923-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="01923-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01923-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01923-112">Not supported.</span></span>|
|<span data-ttu-id="01923-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="01923-113">Application</span></span>|<span data-ttu-id="01923-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01923-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01923-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="01923-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="01923-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="01923-116">Request headers</span></span>
|<span data-ttu-id="01923-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="01923-117">Header</span></span>|<span data-ttu-id="01923-118">Wert</span><span class="sxs-lookup"><span data-stu-id="01923-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01923-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="01923-119">Authorization</span></span>|<span data-ttu-id="01923-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="01923-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="01923-121">Accept</span><span class="sxs-lookup"><span data-stu-id="01923-121">Accept</span></span>|<span data-ttu-id="01923-122">application/json</span><span class="sxs-lookup"><span data-stu-id="01923-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01923-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="01923-123">Request body</span></span>
<span data-ttu-id="01923-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="01923-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="01923-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="01923-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="01923-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01923-126">Property</span></span>|<span data-ttu-id="01923-127">Typ</span><span class="sxs-lookup"><span data-stu-id="01923-127">Type</span></span>|<span data-ttu-id="01923-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01923-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01923-129">hostName</span><span class="sxs-lookup"><span data-stu-id="01923-129">hostname</span></span>|<span data-ttu-id="01923-130">String</span><span class="sxs-lookup"><span data-stu-id="01923-130">String</span></span>|<span data-ttu-id="01923-131">Hostname der Rückruf-URL, auf die der Browser nach dem erfolgreichen Abschluss der Registrierung umgeleitet wird</span><span class="sxs-lookup"><span data-stu-id="01923-131">The hostname of the callback URL to which the browser will be redirected after successfully completing sign-up.</span></span>|



## <a name="response"></a><span data-ttu-id="01923-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="01923-132">Response</span></span>
<span data-ttu-id="01923-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="01923-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01923-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="01923-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="01923-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="01923-135">Request</span></span>
<span data-ttu-id="01923-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="01923-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="01923-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="01923-137">Response</span></span>
<span data-ttu-id="01923-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01923-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```



