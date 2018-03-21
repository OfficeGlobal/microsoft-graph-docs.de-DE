# <a name="create-user"></a><span data-ttu-id="875f8-101">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="875f8-101">Create User</span></span>

> <span data-ttu-id="875f8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="875f8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="875f8-103">Erstellen eines neuen [user](../resources/intune_onboarding_user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="875f8-103">Create a new user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="875f8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="875f8-104">Prerequisites</span></span>
<span data-ttu-id="875f8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="875f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="875f8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="875f8-107">Permission type</span></span>|<span data-ttu-id="875f8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="875f8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="875f8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="875f8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="875f8-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="875f8-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="875f8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="875f8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="875f8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="875f8-112">Not supported.</span></span>|
|<span data-ttu-id="875f8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="875f8-113">Application</span></span>|<span data-ttu-id="875f8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="875f8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="875f8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="875f8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="875f8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="875f8-116">Request headers</span></span>
|<span data-ttu-id="875f8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="875f8-117">Header</span></span>|<span data-ttu-id="875f8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="875f8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="875f8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="875f8-119">Authorization</span></span>|<span data-ttu-id="875f8-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="875f8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="875f8-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="875f8-121">Accept</span></span>|<span data-ttu-id="875f8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="875f8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="875f8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="875f8-123">Request body</span></span>
<span data-ttu-id="875f8-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="875f8-124">In the request body, supply a JSON representation of user object.</span></span>

<span data-ttu-id="875f8-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="875f8-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="875f8-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="875f8-126">Property</span></span>|<span data-ttu-id="875f8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="875f8-127">Type</span></span>|<span data-ttu-id="875f8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="875f8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="875f8-129">id</span><span class="sxs-lookup"><span data-stu-id="875f8-129">id</span></span>|<span data-ttu-id="875f8-130">String</span><span class="sxs-lookup"><span data-stu-id="875f8-130">String</span></span>|<span data-ttu-id="875f8-131">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="875f8-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="875f8-132">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="875f8-132">deviceEnrollmentLimit</span></span>|<span data-ttu-id="875f8-133">Int32</span><span class="sxs-lookup"><span data-stu-id="875f8-133">Int32</span></span>|<span data-ttu-id="875f8-134">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="875f8-134">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="875f8-135">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="875f8-135">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="875f8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="875f8-136">Response</span></span>
<span data-ttu-id="875f8-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/intune_onboarding_user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="875f8-137">If successful, this method returns a `201 Created` response code and [user](../resources/intune_onboarding_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="875f8-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="875f8-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="875f8-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="875f8-139">Request</span></span>
<span data-ttu-id="875f8-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="875f8-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.user",
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="875f8-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="875f8-141">Response</span></span>
<span data-ttu-id="875f8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="875f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```



