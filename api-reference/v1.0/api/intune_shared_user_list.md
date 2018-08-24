# <a name="list-users"></a><span data-ttu-id="8ded0-101">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="8ded0-101">List users</span></span>

> <span data-ttu-id="8ded0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8ded0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ded0-103">Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune_shared_user.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8ded0-103">List properties and relationships of the [user](../resources/intune_shared_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ded0-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8ded0-104">Prerequisites</span></span>
<span data-ttu-id="8ded0-105">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="8ded0-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="8ded0-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ded0-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="8ded0-107">Die jeweilige Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="8ded0-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="8ded0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ded0-108">Permission type</span></span>|<span data-ttu-id="8ded0-109">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ded0-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ded0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ded0-110">Delegated (work or school account)</span></span>| <span data-ttu-id="8ded0-111">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="8ded0-111">_varies by context_</span></span>|
| <span data-ttu-id="8ded0-112">&nbsp; &nbsp; Geräte</span><span class="sxs-lookup"><span data-stu-id="8ded0-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="8ded0-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ded0-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="8ded0-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="8ded0-114">.mam</span></span> | <span data-ttu-id="8ded0-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ded0-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="8ded0-116">&nbsp; &nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="8ded0-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="8ded0-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ded0-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8ded0-118">&nbsp; &nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="8ded0-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="8ded0-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ded0-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="8ded0-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ded0-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ded0-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ded0-121">Not supported.</span></span>|
|<span data-ttu-id="8ded0-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ded0-122">Application</span></span>|<span data-ttu-id="8ded0-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ded0-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ded0-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ded0-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="8ded0-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ded0-125">Request headers</span></span>
|<span data-ttu-id="8ded0-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8ded0-126">Header</span></span>|<span data-ttu-id="8ded0-127">Wert</span><span class="sxs-lookup"><span data-stu-id="8ded0-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ded0-128">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8ded0-128">Authorization</span></span>|<span data-ttu-id="8ded0-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8ded0-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ded0-130">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="8ded0-130">Accept</span></span>|<span data-ttu-id="8ded0-131">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="8ded0-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ded0-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ded0-132">Request body</span></span>
<span data-ttu-id="8ded0-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8ded0-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ded0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ded0-134">Response</span></span>
<span data-ttu-id="8ded0-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/intune_shared_user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ded0-135">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune_shared_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ded0-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ded0-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ded0-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ded0-137">Request</span></span>
<span data-ttu-id="8ded0-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ded0-138">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="8ded0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ded0-139">Response</span></span>
<span data-ttu-id="8ded0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ded0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



