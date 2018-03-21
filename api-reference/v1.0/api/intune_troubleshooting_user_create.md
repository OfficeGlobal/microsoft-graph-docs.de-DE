# <a name="create-user"></a><span data-ttu-id="a33f1-101">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="a33f1-101">Create User</span></span>

> <span data-ttu-id="a33f1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a33f1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a33f1-103">Dient zum Erstellen eines neuen [user](../resources/intune_troubleshooting_user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a33f1-103">Create a new user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a33f1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a33f1-104">Prerequisites</span></span>
<span data-ttu-id="a33f1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a33f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a33f1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a33f1-107">Permission type</span></span>|<span data-ttu-id="a33f1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a33f1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a33f1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a33f1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a33f1-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a33f1-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a33f1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a33f1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a33f1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a33f1-112">Not supported.</span></span>|
|<span data-ttu-id="a33f1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a33f1-113">Application</span></span>|<span data-ttu-id="a33f1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a33f1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a33f1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a33f1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="a33f1-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a33f1-116">Request headers</span></span>
|<span data-ttu-id="a33f1-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a33f1-117">Header</span></span>|<span data-ttu-id="a33f1-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a33f1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a33f1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a33f1-119">Authorization</span></span>|<span data-ttu-id="a33f1-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a33f1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a33f1-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a33f1-121">Accept</span></span>|<span data-ttu-id="a33f1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a33f1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a33f1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a33f1-123">Request body</span></span>
<span data-ttu-id="a33f1-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="a33f1-124">In the request body, supply a JSON representation of user object.</span></span>

<span data-ttu-id="a33f1-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a33f1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a33f1-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a33f1-126">Property</span></span>|<span data-ttu-id="a33f1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a33f1-127">Type</span></span>|<span data-ttu-id="a33f1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a33f1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a33f1-129">id</span><span class="sxs-lookup"><span data-stu-id="a33f1-129">id</span></span>|<span data-ttu-id="a33f1-130">String</span><span class="sxs-lookup"><span data-stu-id="a33f1-130">String</span></span>|<span data-ttu-id="a33f1-131">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="a33f1-131">Unique identifier for the lab user.</span></span>|



## <a name="response"></a><span data-ttu-id="a33f1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a33f1-132">Response</span></span>
<span data-ttu-id="a33f1-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/intune_troubleshooting_user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a33f1-133">If successful, this method returns a `201 Created` response code and [user](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a33f1-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a33f1-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="a33f1-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a33f1-135">Request</span></span>
<span data-ttu-id="a33f1-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a33f1-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="a33f1-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="a33f1-137">Response</span></span>
<span data-ttu-id="a33f1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a33f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



