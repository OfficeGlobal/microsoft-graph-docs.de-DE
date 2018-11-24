# <a name="list-users"></a><span data-ttu-id="a456c-101">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="a456c-101">List users</span></span>

> <span data-ttu-id="a456c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a456c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a456c-103">Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune_shared_user.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="a456c-103">List properties and relationships of the [user](../resources/intune_shared_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a456c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a456c-104">Prerequisites</span></span>
<span data-ttu-id="a456c-105">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="a456c-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a456c-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a456c-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="a456c-107">Die jeweilige Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="a456c-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="a456c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a456c-108">Permission type</span></span>|<span data-ttu-id="a456c-109">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a456c-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a456c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a456c-110">Delegated (work or school account)</span></span>| <span data-ttu-id="a456c-111">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="a456c-111">_varies by context_</span></span>|
| <span data-ttu-id="a456c-112">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="a456c-112">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="a456c-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a456c-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="a456c-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="a456c-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="a456c-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a456c-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="a456c-116">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="a456c-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="a456c-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a456c-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="a456c-118">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="a456c-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="a456c-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a456c-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="a456c-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a456c-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a456c-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a456c-121">Not supported.</span></span>|
|<span data-ttu-id="a456c-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a456c-122">Application</span></span>|<span data-ttu-id="a456c-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a456c-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a456c-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a456c-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="a456c-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a456c-125">Request headers</span></span>
|<span data-ttu-id="a456c-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a456c-126">Header</span></span>|<span data-ttu-id="a456c-127">Wert</span><span class="sxs-lookup"><span data-stu-id="a456c-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a456c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a456c-128">Authorization</span></span>|<span data-ttu-id="a456c-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a456c-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a456c-130">Accept</span><span class="sxs-lookup"><span data-stu-id="a456c-130">Accept</span></span>|<span data-ttu-id="a456c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a456c-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a456c-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a456c-132">Request body</span></span>
<span data-ttu-id="a456c-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a456c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a456c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a456c-134">Response</span></span>
<span data-ttu-id="a456c-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/intune_shared_user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a456c-135">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune_shared_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a456c-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a456c-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="a456c-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a456c-137">Request</span></span>
<span data-ttu-id="a456c-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a456c-138">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="a456c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a456c-139">Response</span></span>
<span data-ttu-id="a456c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a456c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



