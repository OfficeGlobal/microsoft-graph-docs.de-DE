# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="8817f-101">Aktion „wipeManagedAppRegistrationsByDeviceTag“</span><span class="sxs-lookup"><span data-stu-id="8817f-101">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="8817f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8817f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8817f-103">Diese Aktion stößt einen Zurücksetzungsvorgang für eine App-Registrierung mit dem jeweils angegebenen Gerätetag an.</span><span class="sxs-lookup"><span data-stu-id="8817f-103">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8817f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8817f-104">Prerequisites</span></span>
<span data-ttu-id="8817f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8817f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8817f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8817f-107">Permission type</span></span>|<span data-ttu-id="8817f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8817f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8817f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8817f-109">Delegated (work or school account)</span></span>| <span data-ttu-id="8817f-110">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="8817f-110">_varies by context_</span></span> |
| <span data-ttu-id="8817f-111">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="8817f-111">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="8817f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8817f-112">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="8817f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8817f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8817f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8817f-114">Not supported.</span></span>|
|<span data-ttu-id="8817f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8817f-115">Application</span></span>|<span data-ttu-id="8817f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8817f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8817f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8817f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="8817f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8817f-118">Request headers</span></span>
|<span data-ttu-id="8817f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8817f-119">Header</span></span>|<span data-ttu-id="8817f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8817f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8817f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8817f-121">Authorization</span></span>|<span data-ttu-id="8817f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8817f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8817f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8817f-123">Accept</span></span>|<span data-ttu-id="8817f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8817f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8817f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8817f-125">Request body</span></span>
<span data-ttu-id="8817f-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="8817f-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8817f-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="8817f-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8817f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8817f-128">Property</span></span>|<span data-ttu-id="8817f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8817f-129">Type</span></span>|<span data-ttu-id="8817f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8817f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8817f-131">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8817f-131">deviceTag</span></span>|<span data-ttu-id="8817f-132">String</span><span class="sxs-lookup"><span data-stu-id="8817f-132">String</span></span>|<span data-ttu-id="8817f-133">Gerätetag</span><span class="sxs-lookup"><span data-stu-id="8817f-133">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="8817f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8817f-134">Response</span></span>
<span data-ttu-id="8817f-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="8817f-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8817f-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8817f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="8817f-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8817f-137">Request</span></span>
<span data-ttu-id="8817f-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8817f-138">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="8817f-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="8817f-139">Response</span></span>
<span data-ttu-id="8817f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8817f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



