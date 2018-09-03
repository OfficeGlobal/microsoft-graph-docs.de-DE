# <a name="wipe-action"></a><span data-ttu-id="c0f48-101">Aktion „wipe“</span><span class="sxs-lookup"><span data-stu-id="c0f48-101">wipe action</span></span>

> <span data-ttu-id="c0f48-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0f48-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0f48-103">Mit dieser Aktion lässt sich ein Gerät zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="c0f48-103">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0f48-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0f48-104">Prerequisites</span></span>
<span data-ttu-id="c0f48-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c0f48-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0f48-107">Permission type</span></span>|<span data-ttu-id="c0f48-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0f48-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0f48-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0f48-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c0f48-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c0f48-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c0f48-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0f48-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0f48-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0f48-112">Not supported.</span></span>|
|<span data-ttu-id="c0f48-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0f48-113">Application</span></span>|<span data-ttu-id="c0f48-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0f48-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0f48-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0f48-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="c0f48-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0f48-116">Request headers</span></span>
|<span data-ttu-id="c0f48-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c0f48-117">Header</span></span>|<span data-ttu-id="c0f48-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c0f48-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0f48-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c0f48-119">Authorization</span></span>|<span data-ttu-id="c0f48-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0f48-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0f48-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="c0f48-121">Accept</span></span>|<span data-ttu-id="c0f48-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="c0f48-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0f48-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0f48-123">Request body</span></span>
<span data-ttu-id="c0f48-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="c0f48-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c0f48-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="c0f48-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c0f48-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0f48-126">Property</span></span>|<span data-ttu-id="c0f48-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c0f48-127">Type</span></span>|<span data-ttu-id="c0f48-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0f48-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0f48-129">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="c0f48-129">keepEnrollmentData</span></span>|<span data-ttu-id="c0f48-130">boolesch</span><span class="sxs-lookup"><span data-stu-id="c0f48-130">Boolean</span></span>|<span data-ttu-id="c0f48-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c0f48-131">Not yet documented</span></span>|
|<span data-ttu-id="c0f48-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="c0f48-132">keepUserData</span></span>|<span data-ttu-id="c0f48-133">boolesch</span><span class="sxs-lookup"><span data-stu-id="c0f48-133">Boolean</span></span>|<span data-ttu-id="c0f48-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c0f48-134">Not yet documented</span></span>|
|<span data-ttu-id="c0f48-135">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="c0f48-135">macOsUnlockCode</span></span>|<span data-ttu-id="c0f48-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0f48-136">String</span></span>|<span data-ttu-id="c0f48-137">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c0f48-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c0f48-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0f48-138">Response</span></span>
<span data-ttu-id="c0f48-139">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="c0f48-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0f48-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0f48-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0f48-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0f48-141">Request</span></span>
<span data-ttu-id="c0f48-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0f48-142">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe
Content-type: application/json

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="c0f48-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0f48-143">Response</span></span>
<span data-ttu-id="c0f48-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0f48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "response" } -->
``` http
HTTP/1.1 204 No Content
```



