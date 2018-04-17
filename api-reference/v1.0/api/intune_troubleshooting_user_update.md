# <a name="update-user"></a><span data-ttu-id="81648-101">Benutzer aktualisieren</span><span class="sxs-lookup"><span data-stu-id="81648-101">Update user</span></span>

> <span data-ttu-id="81648-102">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="81648-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81648-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81648-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81648-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="81648-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81648-105">Aktualisieren der Eigenschaften eines [user](../resources/intune_troubleshooting_user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="81648-105">Update the properties of a [user](../resources/intune_troubleshooting_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81648-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="81648-106">Prerequisites</span></span>
<span data-ttu-id="81648-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81648-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81648-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="81648-109">Permission type</span></span>|<span data-ttu-id="81648-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="81648-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81648-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="81648-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81648-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81648-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="81648-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="81648-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81648-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81648-114">Not supported.</span></span>|
|<span data-ttu-id="81648-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="81648-115">Application</span></span>|<span data-ttu-id="81648-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81648-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81648-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="81648-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="81648-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="81648-118">Request headers</span></span>
|<span data-ttu-id="81648-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="81648-119">Header</span></span>|<span data-ttu-id="81648-120">Wert</span><span class="sxs-lookup"><span data-stu-id="81648-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81648-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="81648-121">Authorization</span></span>|<span data-ttu-id="81648-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="81648-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81648-123">Accept</span><span class="sxs-lookup"><span data-stu-id="81648-123">Accept</span></span>|<span data-ttu-id="81648-124">application/json</span><span class="sxs-lookup"><span data-stu-id="81648-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81648-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="81648-125">Request body</span></span>
<span data-ttu-id="81648-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/intune_troubleshooting_user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="81648-126">In the request body, supply a JSON representation for the [user](../resources/intune_troubleshooting_user.md) object.</span></span>

<span data-ttu-id="81648-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [user](../resources/intune_troubleshooting_user.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="81648-127">The following table shows the properties that are required when you create the [user](../resources/intune_troubleshooting_user.md).</span></span>

|<span data-ttu-id="81648-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81648-128">Property</span></span>|<span data-ttu-id="81648-129">Typ</span><span class="sxs-lookup"><span data-stu-id="81648-129">Type</span></span>|<span data-ttu-id="81648-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81648-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81648-131">id</span><span class="sxs-lookup"><span data-stu-id="81648-131">id</span></span>|<span data-ttu-id="81648-132">String</span><span class="sxs-lookup"><span data-stu-id="81648-132">String</span></span>|<span data-ttu-id="81648-133">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="81648-133">Unique Identifier for the user</span></span>|



## <a name="response"></a><span data-ttu-id="81648-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="81648-134">Response</span></span>
<span data-ttu-id="81648-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [user](../resources/intune_troubleshooting_user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81648-135">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81648-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="81648-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="81648-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="81648-137">Request</span></span>
<span data-ttu-id="81648-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="81648-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="81648-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="81648-139">Response</span></span>
<span data-ttu-id="81648-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81648-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



