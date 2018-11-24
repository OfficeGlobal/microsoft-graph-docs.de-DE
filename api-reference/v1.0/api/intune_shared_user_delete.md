# <a name="delete-user"></a><span data-ttu-id="47d24-101">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="47d24-101">Delete user</span></span>

> <span data-ttu-id="47d24-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="47d24-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47d24-103">Löscht ein [user](../resources/intune_shared_user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="47d24-103">Deletes a [user](../resources/intune_shared_user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47d24-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="47d24-104">Prerequisites</span></span>
<span data-ttu-id="47d24-105">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="47d24-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="47d24-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="47d24-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="47d24-107">Die spezifische erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="47d24-107">The specific permission required depends on context.</span></span>

|<span data-ttu-id="47d24-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47d24-108">Permission type</span></span>|<span data-ttu-id="47d24-109">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47d24-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47d24-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47d24-110">Delegated (work or school account)</span></span>| <span data-ttu-id="47d24-111">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="47d24-111">_varies by context_</span></span>|
| <span data-ttu-id="47d24-112">&nbsp;&nbsp; Geräte</span><span class="sxs-lookup"><span data-stu-id="47d24-112">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="47d24-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d24-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="47d24-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="47d24-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="47d24-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d24-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="47d24-116">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="47d24-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="47d24-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d24-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="47d24-118">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="47d24-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="47d24-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d24-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="47d24-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47d24-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47d24-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47d24-121">Not supported.</span></span>|
|<span data-ttu-id="47d24-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47d24-122">Application</span></span>|<span data-ttu-id="47d24-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47d24-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47d24-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47d24-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="47d24-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47d24-125">Request headers</span></span>
|<span data-ttu-id="47d24-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="47d24-126">Header</span></span>|<span data-ttu-id="47d24-127">Wert</span><span class="sxs-lookup"><span data-stu-id="47d24-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47d24-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="47d24-128">Authorization</span></span>|<span data-ttu-id="47d24-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="47d24-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47d24-130">Accept</span><span class="sxs-lookup"><span data-stu-id="47d24-130">Accept</span></span>|<span data-ttu-id="47d24-131">application/json</span><span class="sxs-lookup"><span data-stu-id="47d24-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47d24-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47d24-132">Request body</span></span>
<span data-ttu-id="47d24-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="47d24-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47d24-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="47d24-134">Response</span></span>
<span data-ttu-id="47d24-135">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47d24-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="47d24-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47d24-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="47d24-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47d24-137">Request</span></span>
<span data-ttu-id="47d24-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47d24-138">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="47d24-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="47d24-139">Response</span></span>
<span data-ttu-id="47d24-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47d24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



