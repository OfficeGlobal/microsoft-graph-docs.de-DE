# <a name="completesignup-action"></a><span data-ttu-id="8e01b-101">Aktion „completeSignup“</span><span class="sxs-lookup"><span data-stu-id="8e01b-101">completeSignup action</span></span>

> <span data-ttu-id="8e01b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e01b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e01b-103">Diese Aktion schließt den Fluss zur Registrierung in der Android for Work-Verwaltung ab.</span><span class="sxs-lookup"><span data-stu-id="8e01b-103">Completes the sign-up flow for Android for Work management.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e01b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e01b-104">Prerequisites</span></span>
<span data-ttu-id="8e01b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e01b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e01b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e01b-107">Permission type</span></span>|<span data-ttu-id="8e01b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e01b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e01b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e01b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8e01b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e01b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e01b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e01b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e01b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e01b-112">Not supported.</span></span>|
|<span data-ttu-id="8e01b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e01b-113">Application</span></span>|<span data-ttu-id="8e01b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e01b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e01b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e01b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/completeSignup
```

## <a name="request-headers"></a><span data-ttu-id="8e01b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e01b-116">Request headers</span></span>
|<span data-ttu-id="8e01b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8e01b-117">Header</span></span>|<span data-ttu-id="8e01b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8e01b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e01b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e01b-119">Authorization</span></span>|<span data-ttu-id="8e01b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e01b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8e01b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8e01b-121">Accept</span></span>|<span data-ttu-id="8e01b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8e01b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e01b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e01b-123">Request body</span></span>
<span data-ttu-id="8e01b-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="8e01b-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="8e01b-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="8e01b-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8e01b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e01b-126">Property</span></span>|<span data-ttu-id="8e01b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8e01b-127">Type</span></span>|<span data-ttu-id="8e01b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e01b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e01b-129">enterpriseToken</span><span class="sxs-lookup"><span data-stu-id="8e01b-129">enterpriseToken</span></span>|<span data-ttu-id="8e01b-130">String</span><span class="sxs-lookup"><span data-stu-id="8e01b-130">String</span></span>|<span data-ttu-id="8e01b-131">Unternehmenstoken, das nach dem erfolgreichen Abschluss der Registrierung an die Rückruf-URL angefügt wird</span><span class="sxs-lookup"><span data-stu-id="8e01b-131">The Enterprise token appended to the callback URL after successfully completing sign-up.</span></span>|



## <a name="response"></a><span data-ttu-id="8e01b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e01b-132">Response</span></span>
<span data-ttu-id="8e01b-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="8e01b-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8e01b-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e01b-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e01b-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e01b-135">Request</span></span>
<span data-ttu-id="8e01b-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e01b-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings/completeSignup

Content-type: application/json
Content-length: 51

{
  "enterpriseToken": "Enterprise Token value"
}
```

### <a name="response"></a><span data-ttu-id="8e01b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e01b-137">Response</span></span>
<span data-ttu-id="8e01b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e01b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



