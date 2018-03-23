# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="43fa9-101">Aktion „cleanWindowsDevice“</span><span class="sxs-lookup"><span data-stu-id="43fa9-101">cleanWindowsDevice action</span></span>

> <span data-ttu-id="43fa9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="43fa9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43fa9-103">Diese Aktion bereinigt Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="43fa9-103">Clean Windows device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43fa9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="43fa9-104">Prerequisites</span></span>
<span data-ttu-id="43fa9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43fa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43fa9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43fa9-107">Permission type</span></span>|<span data-ttu-id="43fa9-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43fa9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43fa9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43fa9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="43fa9-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="43fa9-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="43fa9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43fa9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43fa9-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43fa9-112">Not supported.</span></span>|
|<span data-ttu-id="43fa9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43fa9-113">Application</span></span>|<span data-ttu-id="43fa9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43fa9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43fa9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43fa9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="43fa9-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43fa9-116">Request headers</span></span>
|<span data-ttu-id="43fa9-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="43fa9-117">Header</span></span>|<span data-ttu-id="43fa9-118">Wert</span><span class="sxs-lookup"><span data-stu-id="43fa9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43fa9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="43fa9-119">Authorization</span></span>|<span data-ttu-id="43fa9-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="43fa9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="43fa9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="43fa9-121">Accept</span></span>|<span data-ttu-id="43fa9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="43fa9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43fa9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43fa9-123">Request body</span></span>
<span data-ttu-id="43fa9-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="43fa9-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="43fa9-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="43fa9-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="43fa9-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43fa9-126">Property</span></span>|<span data-ttu-id="43fa9-127">Typ</span><span class="sxs-lookup"><span data-stu-id="43fa9-127">Type</span></span>|<span data-ttu-id="43fa9-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43fa9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43fa9-129">keepUserData</span><span class="sxs-lookup"><span data-stu-id="43fa9-129">keepUserData</span></span>|<span data-ttu-id="43fa9-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="43fa9-130">Boolean</span></span>|<span data-ttu-id="43fa9-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="43fa9-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="43fa9-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="43fa9-132">Response</span></span>
<span data-ttu-id="43fa9-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="43fa9-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43fa9-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43fa9-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="43fa9-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43fa9-135">Request</span></span>
<span data-ttu-id="43fa9-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43fa9-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="43fa9-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="43fa9-137">Response</span></span>
<span data-ttu-id="43fa9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43fa9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



