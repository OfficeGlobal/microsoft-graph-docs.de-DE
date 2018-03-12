# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="38025-101">updateWindowsDeviceAccount-Aktion</span><span class="sxs-lookup"><span data-stu-id="38025-101">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="38025-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="38025-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38025-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="38025-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38025-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="38025-104">Prerequisites</span></span>
<span data-ttu-id="38025-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38025-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="38025-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38025-107">Permission type</span></span>|<span data-ttu-id="38025-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38025-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38025-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38025-109">Delegated (work or school account)</span></span>|<span data-ttu-id="38025-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="38025-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="38025-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38025-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38025-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38025-112">Not supported.</span></span>|
|<span data-ttu-id="38025-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38025-113">Application</span></span>|<span data-ttu-id="38025-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38025-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38025-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38025-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="38025-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38025-116">Request headers</span></span>
|<span data-ttu-id="38025-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="38025-117">Header</span></span>|<span data-ttu-id="38025-118">Wert</span><span class="sxs-lookup"><span data-stu-id="38025-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38025-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="38025-119">Authorization</span></span>|<span data-ttu-id="38025-120">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38025-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="38025-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="38025-121">Accept</span></span>|<span data-ttu-id="38025-122">application/json</span><span class="sxs-lookup"><span data-stu-id="38025-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38025-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38025-123">Request body</span></span>
<span data-ttu-id="38025-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Parameters an.</span><span class="sxs-lookup"><span data-stu-id="38025-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="38025-125">Die folgende Tabelle zeigt die Parameter, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="38025-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="38025-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38025-126">Property</span></span>|<span data-ttu-id="38025-127">Typ</span><span class="sxs-lookup"><span data-stu-id="38025-127">Type</span></span>|<span data-ttu-id="38025-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38025-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38025-129">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="38025-129">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="38025-130">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="38025-130">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune_devices_updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="38025-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="38025-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="38025-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="38025-132">Response</span></span>
<span data-ttu-id="38025-133">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38025-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="38025-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38025-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="38025-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38025-135">Request</span></span>
<span data-ttu-id="38025-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38025-136">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38025-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="38025-137">Response</span></span>
<span data-ttu-id="38025-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38025-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



