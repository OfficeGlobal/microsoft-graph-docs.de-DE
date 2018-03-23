# <a name="create-user"></a><span data-ttu-id="c203b-101">Erstellen von „user“</span><span class="sxs-lookup"><span data-stu-id="c203b-101">Create User</span></span>

> <span data-ttu-id="c203b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c203b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c203b-103">Diese Methode erstellt ein neues Objekt des Typs [user](../resources/intune_mam_user.md).</span><span class="sxs-lookup"><span data-stu-id="c203b-103">Create a new user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c203b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c203b-104">Prerequisites</span></span>
<span data-ttu-id="c203b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c203b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c203b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c203b-107">Permission type</span></span>|<span data-ttu-id="c203b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c203b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c203b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c203b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c203b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c203b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c203b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c203b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c203b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c203b-112">Not supported.</span></span>|
|<span data-ttu-id="c203b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c203b-113">Application</span></span>|<span data-ttu-id="c203b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c203b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c203b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c203b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="c203b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c203b-116">Request headers</span></span>
|<span data-ttu-id="c203b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c203b-117">Header</span></span>|<span data-ttu-id="c203b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c203b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c203b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c203b-119">Authorization</span></span>|<span data-ttu-id="c203b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c203b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c203b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c203b-121">Accept</span></span>|<span data-ttu-id="c203b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c203b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c203b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c203b-123">Request body</span></span>
<span data-ttu-id="c203b-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="c203b-124">In the request body, supply a JSON representation of user object.</span></span>

<span data-ttu-id="c203b-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c203b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="c203b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c203b-126">Property</span></span>|<span data-ttu-id="c203b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c203b-127">Type</span></span>|<span data-ttu-id="c203b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c203b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c203b-129">id</span><span class="sxs-lookup"><span data-stu-id="c203b-129">id</span></span>|<span data-ttu-id="c203b-130">String</span><span class="sxs-lookup"><span data-stu-id="c203b-130">String</span></span>|<span data-ttu-id="c203b-131">Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="c203b-131">The user identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="c203b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c203b-132">Response</span></span>
<span data-ttu-id="c203b-133">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [user](../resources/intune_mam_user.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c203b-133">If successful, this method returns a `201 Created` response code and [user](../resources/intune_mam_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c203b-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c203b-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="c203b-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c203b-135">Request</span></span>
<span data-ttu-id="c203b-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c203b-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="c203b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c203b-137">Response</span></span>
<span data-ttu-id="c203b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c203b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



