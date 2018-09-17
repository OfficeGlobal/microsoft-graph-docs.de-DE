# <a name="windowsdefenderscan-action"></a><span data-ttu-id="257fd-101">windowsDefenderScan-Aktion</span><span class="sxs-lookup"><span data-stu-id="257fd-101">windowsDefenderScan action</span></span>

> <span data-ttu-id="257fd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="257fd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="257fd-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="257fd-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="257fd-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="257fd-104">Prerequisites</span></span>
<span data-ttu-id="257fd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="257fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="257fd-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="257fd-107">Permission type</span></span>|<span data-ttu-id="257fd-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="257fd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="257fd-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="257fd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="257fd-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="257fd-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="257fd-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="257fd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="257fd-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="257fd-112">Not supported.</span></span>|
|<span data-ttu-id="257fd-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="257fd-113">Application</span></span>|<span data-ttu-id="257fd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="257fd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="257fd-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="257fd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="257fd-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="257fd-116">Request headers</span></span>
|<span data-ttu-id="257fd-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="257fd-117">Header</span></span>|<span data-ttu-id="257fd-118">Wert</span><span class="sxs-lookup"><span data-stu-id="257fd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="257fd-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="257fd-119">Authorization</span></span>|<span data-ttu-id="257fd-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="257fd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="257fd-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="257fd-121">Accept</span></span>|<span data-ttu-id="257fd-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="257fd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="257fd-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="257fd-123">Request body</span></span>
<span data-ttu-id="257fd-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="257fd-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="257fd-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="257fd-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="257fd-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="257fd-126">Property</span></span>|<span data-ttu-id="257fd-127">Typ</span><span class="sxs-lookup"><span data-stu-id="257fd-127">Type</span></span>|<span data-ttu-id="257fd-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="257fd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="257fd-129">quickScan</span><span class="sxs-lookup"><span data-stu-id="257fd-129">quickScan</span></span>|<span data-ttu-id="257fd-130">Boolesch</span><span class="sxs-lookup"><span data-stu-id="257fd-130">Boolean</span></span>|<span data-ttu-id="257fd-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="257fd-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="257fd-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="257fd-132">Response</span></span>
<span data-ttu-id="257fd-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="257fd-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="257fd-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="257fd-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="257fd-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="257fd-135">Request</span></span>
<span data-ttu-id="257fd-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="257fd-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="257fd-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="257fd-137">Response</span></span>
<span data-ttu-id="257fd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="257fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








