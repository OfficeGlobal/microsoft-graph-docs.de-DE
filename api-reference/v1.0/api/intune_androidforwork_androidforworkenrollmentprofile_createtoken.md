# <a name="createtoken-action"></a><span data-ttu-id="7556f-101">Aktion „createToken“</span><span class="sxs-lookup"><span data-stu-id="7556f-101">createToken action</span></span>

> <span data-ttu-id="7556f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7556f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7556f-103">Diese Aktion ist noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="7556f-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7556f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7556f-104">Prerequisites</span></span>
<span data-ttu-id="7556f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7556f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7556f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7556f-107">Permission type</span></span>|<span data-ttu-id="7556f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7556f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7556f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7556f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7556f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7556f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7556f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7556f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7556f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7556f-112">Not supported.</span></span>|
|<span data-ttu-id="7556f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7556f-113">Application</span></span>|<span data-ttu-id="7556f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7556f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7556f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7556f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken
```

## <a name="request-headers"></a><span data-ttu-id="7556f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7556f-116">Request headers</span></span>
|<span data-ttu-id="7556f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7556f-117">Header</span></span>|<span data-ttu-id="7556f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="7556f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7556f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7556f-119">Authorization</span></span>|<span data-ttu-id="7556f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7556f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7556f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7556f-121">Accept</span></span>|<span data-ttu-id="7556f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7556f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7556f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7556f-123">Request body</span></span>
<span data-ttu-id="7556f-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="7556f-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="7556f-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="7556f-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7556f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7556f-126">Property</span></span>|<span data-ttu-id="7556f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7556f-127">Type</span></span>|<span data-ttu-id="7556f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7556f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7556f-129">tokenValidityInSeconds</span><span class="sxs-lookup"><span data-stu-id="7556f-129">tokenValidityInSeconds</span></span>|<span data-ttu-id="7556f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="7556f-130">Int32</span></span>|<span data-ttu-id="7556f-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7556f-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7556f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7556f-132">Response</span></span>
<span data-ttu-id="7556f-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="7556f-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7556f-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7556f-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="7556f-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7556f-135">Request</span></span>
<span data-ttu-id="7556f-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7556f-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken

Content-type: application/json
Content-length: 35

{
  "tokenValidityInSeconds": 6
}
```

### <a name="response"></a><span data-ttu-id="7556f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7556f-137">Response</span></span>
<span data-ttu-id="7556f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7556f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



