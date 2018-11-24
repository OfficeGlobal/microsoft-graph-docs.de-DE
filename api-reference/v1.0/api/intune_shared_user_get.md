# <a name="get-user"></a><span data-ttu-id="c62a8-101">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="c62a8-101">Get user</span></span>

> <span data-ttu-id="c62a8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c62a8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c62a8-103">Lesen von Eigenschaften und Beziehungen des [user](../resources/intune_shared_user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c62a8-103">Read properties and relationships of the [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c62a8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c62a8-104">Prerequisites</span></span>
<span data-ttu-id="c62a8-105">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="c62a8-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c62a8-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c62a8-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="c62a8-107">Die jeweilige Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="c62a8-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="c62a8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c62a8-108">Permission type</span></span>|<span data-ttu-id="c62a8-109">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c62a8-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c62a8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c62a8-110">Delegated (work or school account)</span></span>| <span data-ttu-id="c62a8-111">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="c62a8-111">_varies by context_</span></span>|
| <span data-ttu-id="c62a8-112">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="c62a8-112">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="c62a8-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62a8-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="c62a8-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="c62a8-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="c62a8-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62a8-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="c62a8-116">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="c62a8-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="c62a8-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62a8-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c62a8-118">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="c62a8-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="c62a8-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62a8-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="c62a8-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c62a8-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c62a8-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c62a8-121">Not supported.</span></span>|
|<span data-ttu-id="c62a8-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c62a8-122">Application</span></span>|<span data-ttu-id="c62a8-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c62a8-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c62a8-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c62a8-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c62a8-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c62a8-125">Optional query parameters</span></span>
<span data-ttu-id="c62a8-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c62a8-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c62a8-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c62a8-127">Request headers</span></span>
|<span data-ttu-id="c62a8-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c62a8-128">Header</span></span>|<span data-ttu-id="c62a8-129">Wert</span><span class="sxs-lookup"><span data-stu-id="c62a8-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c62a8-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="c62a8-130">Authorization</span></span>|<span data-ttu-id="c62a8-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c62a8-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c62a8-132">Accept</span><span class="sxs-lookup"><span data-stu-id="c62a8-132">Accept</span></span>|<span data-ttu-id="c62a8-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c62a8-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c62a8-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c62a8-134">Request body</span></span>
<span data-ttu-id="c62a8-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c62a8-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c62a8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c62a8-136">Response</span></span>
<span data-ttu-id="c62a8-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/intune_shared_user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c62a8-137">If successful, this method returns a `200 OK` response code and [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c62a8-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c62a8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c62a8-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c62a8-139">Request</span></span>
<span data-ttu-id="c62a8-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c62a8-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="c62a8-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="c62a8-141">Response</span></span>
<span data-ttu-id="c62a8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c62a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



