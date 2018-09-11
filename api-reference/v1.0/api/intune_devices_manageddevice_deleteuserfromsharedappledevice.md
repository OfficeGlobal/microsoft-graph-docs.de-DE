# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="71372-101">deleteUserFromSharedAppleDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="71372-101">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="71372-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71372-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71372-103">Benutzer von freigegebenem Apple-Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="71372-103">Delete user from shared Apple device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71372-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71372-104">Prerequisites</span></span>
<span data-ttu-id="71372-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71372-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71372-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71372-107">Permission type</span></span>|<span data-ttu-id="71372-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71372-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71372-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71372-109">Delegated (work or school account)</span></span>|<span data-ttu-id="71372-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="71372-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="71372-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71372-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71372-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71372-112">Not supported.</span></span>|
|<span data-ttu-id="71372-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71372-113">Application</span></span>|<span data-ttu-id="71372-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71372-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71372-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71372-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="71372-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71372-116">Request headers</span></span>
|<span data-ttu-id="71372-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71372-117">Header</span></span>|<span data-ttu-id="71372-118">Wert</span><span class="sxs-lookup"><span data-stu-id="71372-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71372-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="71372-119">Authorization</span></span>|<span data-ttu-id="71372-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71372-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71372-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="71372-121">Accept</span></span>|<span data-ttu-id="71372-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="71372-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71372-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71372-123">Request body</span></span>
<span data-ttu-id="71372-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="71372-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="71372-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="71372-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="71372-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71372-126">Property</span></span>|<span data-ttu-id="71372-127">Typ</span><span class="sxs-lookup"><span data-stu-id="71372-127">Type</span></span>|<span data-ttu-id="71372-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71372-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71372-129">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="71372-129">userPrincipalName</span></span>|<span data-ttu-id="71372-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="71372-130">String</span></span>|<span data-ttu-id="71372-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="71372-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="71372-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="71372-132">Response</span></span>
<span data-ttu-id="71372-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="71372-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="71372-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71372-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="71372-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71372-135">Request</span></span>
<span data-ttu-id="71372-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71372-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="71372-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="71372-137">Response</span></span>
<span data-ttu-id="71372-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71372-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








