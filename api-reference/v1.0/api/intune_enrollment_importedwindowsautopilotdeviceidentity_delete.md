# <a name="delete-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="63108-101">importedWindowsAutopilotDeviceIdentity löschen</span><span class="sxs-lookup"><span data-stu-id="63108-101">Delete importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="63108-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="63108-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63108-103">Löscht eine [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="63108-103">Deletes a [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63108-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="63108-104">Prerequisites</span></span>
<span data-ttu-id="63108-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="63108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63108-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63108-107">Permission type</span></span>|<span data-ttu-id="63108-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63108-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63108-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63108-109">Delegated (work or school account)</span></span>|<span data-ttu-id="63108-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63108-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63108-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63108-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63108-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63108-112">Not supported.</span></span>|
|<span data-ttu-id="63108-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63108-113">Application</span></span>|<span data-ttu-id="63108-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63108-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63108-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63108-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="63108-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63108-116">Request headers</span></span>
|<span data-ttu-id="63108-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="63108-117">Header</span></span>|<span data-ttu-id="63108-118">Wert</span><span class="sxs-lookup"><span data-stu-id="63108-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63108-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="63108-119">Authorization</span></span>|<span data-ttu-id="63108-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="63108-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63108-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="63108-121">Accept</span></span>|<span data-ttu-id="63108-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="63108-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63108-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="63108-123">Request body</span></span>
<span data-ttu-id="63108-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="63108-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63108-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="63108-125">Response</span></span>
<span data-ttu-id="63108-126">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63108-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63108-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="63108-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="63108-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63108-128">Request</span></span>
<span data-ttu-id="63108-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63108-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="63108-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="63108-130">Response</span></span>
<span data-ttu-id="63108-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63108-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



