# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="25d51-101">updateWindowsDeviceAccount-Aktion</span><span class="sxs-lookup"><span data-stu-id="25d51-101">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="25d51-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="25d51-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25d51-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="25d51-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="25d51-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="25d51-104">Prerequisites</span></span>
<span data-ttu-id="25d51-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="25d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="25d51-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25d51-107">Permission type</span></span>|<span data-ttu-id="25d51-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25d51-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25d51-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25d51-109">Delegated (work or school account)</span></span>|<span data-ttu-id="25d51-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="25d51-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="25d51-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25d51-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25d51-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25d51-112">Not supported.</span></span>|
|<span data-ttu-id="25d51-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25d51-113">Application</span></span>|<span data-ttu-id="25d51-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25d51-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25d51-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25d51-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="25d51-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="25d51-116">Request headers</span></span>
|<span data-ttu-id="25d51-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="25d51-117">Header</span></span>|<span data-ttu-id="25d51-118">Wert</span><span class="sxs-lookup"><span data-stu-id="25d51-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25d51-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="25d51-119">Authorization</span></span>|<span data-ttu-id="25d51-120">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25d51-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25d51-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="25d51-121">Accept</span></span>|<span data-ttu-id="25d51-122">application/json</span><span class="sxs-lookup"><span data-stu-id="25d51-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25d51-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25d51-123">Request body</span></span>
<span data-ttu-id="25d51-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Parameters an.</span><span class="sxs-lookup"><span data-stu-id="25d51-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="25d51-125">Die folgende Tabelle zeigt die Parameter, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="25d51-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="25d51-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="25d51-126">Property</span></span>|<span data-ttu-id="25d51-127">Typ</span><span class="sxs-lookup"><span data-stu-id="25d51-127">Type</span></span>|<span data-ttu-id="25d51-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25d51-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25d51-129">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="25d51-129">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="25d51-130">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="25d51-130">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune_devices_updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="25d51-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="25d51-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="25d51-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="25d51-132">Response</span></span>
<span data-ttu-id="25d51-133">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25d51-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="25d51-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="25d51-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="25d51-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25d51-135">Request</span></span>
<span data-ttu-id="25d51-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="25d51-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="25d51-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="25d51-137">Response</span></span>
<span data-ttu-id="25d51-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25d51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



