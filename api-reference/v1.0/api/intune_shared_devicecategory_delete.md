# <a name="delete-devicecategory"></a><span data-ttu-id="f9c16-101">deviceCategory löschen</span><span class="sxs-lookup"><span data-stu-id="f9c16-101">Delete deviceCategory</span></span>

> <span data-ttu-id="f9c16-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f9c16-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9c16-103">Löscht ein [deviceCategory](../resources/intune_shared_devicecategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="f9c16-103">Deletes a [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9c16-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f9c16-104">Prerequisites</span></span>
<span data-ttu-id="f9c16-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9c16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9c16-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9c16-107">Permission type</span></span>|<span data-ttu-id="f9c16-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9c16-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9c16-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9c16-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f9c16-110">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="f9c16-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f9c16-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c16-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9c16-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9c16-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9c16-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9c16-113">Not supported.</span></span>|
|<span data-ttu-id="f9c16-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9c16-114">Application</span></span>|<span data-ttu-id="f9c16-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9c16-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9c16-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9c16-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f9c16-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9c16-117">Request headers</span></span>
|<span data-ttu-id="f9c16-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f9c16-118">Header</span></span>|<span data-ttu-id="f9c16-119">Wert</span><span class="sxs-lookup"><span data-stu-id="f9c16-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9c16-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9c16-120">Authorization</span></span>|<span data-ttu-id="f9c16-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f9c16-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9c16-122">Accept</span><span class="sxs-lookup"><span data-stu-id="f9c16-122">Accept</span></span>|<span data-ttu-id="f9c16-123">application/json</span><span class="sxs-lookup"><span data-stu-id="f9c16-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9c16-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9c16-124">Request body</span></span>
<span data-ttu-id="f9c16-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f9c16-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9c16-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9c16-126">Response</span></span>
<span data-ttu-id="f9c16-127">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9c16-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9c16-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9c16-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9c16-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9c16-129">Request</span></span>
<span data-ttu-id="f9c16-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9c16-130">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="f9c16-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9c16-131">Response</span></span>
<span data-ttu-id="f9c16-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9c16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



