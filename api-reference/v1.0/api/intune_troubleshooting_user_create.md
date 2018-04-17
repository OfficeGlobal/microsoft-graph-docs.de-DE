# <a name="create-user"></a><span data-ttu-id="0f96f-101">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="0f96f-101">Create user</span></span>

> <span data-ttu-id="0f96f-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f96f-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f96f-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f96f-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f96f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0f96f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f96f-105">Dient zum Erstellen eines neuen [user](../resources/intune_troubleshooting_user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0f96f-105">Create a new [user](../resources/intune_troubleshooting_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f96f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0f96f-106">Prerequisites</span></span>
<span data-ttu-id="0f96f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f96f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0f96f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f96f-109">Permission type</span></span>|<span data-ttu-id="0f96f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f96f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f96f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f96f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f96f-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f96f-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0f96f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f96f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f96f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f96f-114">Not supported.</span></span>|
|<span data-ttu-id="0f96f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f96f-115">Application</span></span>|<span data-ttu-id="0f96f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f96f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f96f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f96f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="0f96f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f96f-118">Request headers</span></span>
|<span data-ttu-id="0f96f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0f96f-119">Header</span></span>|<span data-ttu-id="0f96f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0f96f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f96f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f96f-121">Authorization</span></span>|<span data-ttu-id="0f96f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0f96f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f96f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0f96f-123">Accept</span></span>|<span data-ttu-id="0f96f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f96f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f96f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f96f-125">Request body</span></span>
<span data-ttu-id="0f96f-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="0f96f-126">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="0f96f-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0f96f-127">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="0f96f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f96f-128">Property</span></span>|<span data-ttu-id="0f96f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0f96f-129">Type</span></span>|<span data-ttu-id="0f96f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f96f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f96f-131">id</span><span class="sxs-lookup"><span data-stu-id="0f96f-131">id</span></span>|<span data-ttu-id="0f96f-132">String</span><span class="sxs-lookup"><span data-stu-id="0f96f-132">String</span></span>|<span data-ttu-id="0f96f-133">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="0f96f-133">Unique Identifier for the user</span></span>|



## <a name="response"></a><span data-ttu-id="0f96f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f96f-134">Response</span></span>
<span data-ttu-id="0f96f-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/intune_troubleshooting_user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f96f-135">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f96f-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f96f-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f96f-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f96f-137">Request</span></span>
<span data-ttu-id="0f96f-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f96f-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="0f96f-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f96f-139">Response</span></span>
<span data-ttu-id="0f96f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f96f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



