# <a name="update-user"></a><span data-ttu-id="3660c-101">Aktualisieren von „user“</span><span class="sxs-lookup"><span data-stu-id="3660c-101">Update user</span></span>

> <span data-ttu-id="3660c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3660c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3660c-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [user](../resources/intune_mam_user.md).</span><span class="sxs-lookup"><span data-stu-id="3660c-103">Update the properties of a user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3660c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3660c-104">Prerequisites</span></span>
<span data-ttu-id="3660c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3660c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3660c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3660c-107">Permission type</span></span>|<span data-ttu-id="3660c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3660c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3660c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3660c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3660c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3660c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3660c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3660c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3660c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3660c-112">Not supported.</span></span>|
|<span data-ttu-id="3660c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3660c-113">Application</span></span>|<span data-ttu-id="3660c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3660c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3660c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3660c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="3660c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3660c-116">Request headers</span></span>
|<span data-ttu-id="3660c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3660c-117">Header</span></span>|<span data-ttu-id="3660c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3660c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3660c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3660c-119">Authorization</span></span>|<span data-ttu-id="3660c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3660c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3660c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3660c-121">Accept</span></span>|<span data-ttu-id="3660c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3660c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3660c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3660c-123">Request body</span></span>
<span data-ttu-id="3660c-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [user](../resources/intune_mam_user.md) an.</span><span class="sxs-lookup"><span data-stu-id="3660c-124">In the request body, supply a JSON representation of [user](../resources/intune_mam_user.md) object.</span></span>

<span data-ttu-id="3660c-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [user](../resources/intune_mam_user.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3660c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="3660c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3660c-126">Property</span></span>|<span data-ttu-id="3660c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3660c-127">Type</span></span>|<span data-ttu-id="3660c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3660c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3660c-129">id</span><span class="sxs-lookup"><span data-stu-id="3660c-129">id</span></span>|<span data-ttu-id="3660c-130">String</span><span class="sxs-lookup"><span data-stu-id="3660c-130">String</span></span>|<span data-ttu-id="3660c-131">Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="3660c-131">The user identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="3660c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3660c-132">Response</span></span>
<span data-ttu-id="3660c-133">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [user](../resources/intune_mam_user.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3660c-133">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3660c-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3660c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="3660c-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3660c-135">Request</span></span>
<span data-ttu-id="3660c-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3660c-136">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="3660c-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="3660c-137">Response</span></span>
<span data-ttu-id="3660c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3660c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



