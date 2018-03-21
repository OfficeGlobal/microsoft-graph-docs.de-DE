# <a name="update-user"></a><span data-ttu-id="558a7-101">Benutzer aktualisieren</span><span class="sxs-lookup"><span data-stu-id="558a7-101">Update user</span></span>

> <span data-ttu-id="558a7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="558a7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="558a7-103">Aktualisieren der Eigenschaften eines [user](../resources/intune_onboarding_user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="558a7-103">Update the properties of a user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="558a7-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="558a7-104">Prerequisites</span></span>
<span data-ttu-id="558a7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="558a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="558a7-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="558a7-107">Permission type</span></span>|<span data-ttu-id="558a7-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="558a7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="558a7-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="558a7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="558a7-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="558a7-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="558a7-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="558a7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="558a7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="558a7-112">Not supported.</span></span>|
|<span data-ttu-id="558a7-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="558a7-113">Application</span></span>|<span data-ttu-id="558a7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="558a7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="558a7-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="558a7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="558a7-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="558a7-116">Request headers</span></span>
|<span data-ttu-id="558a7-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="558a7-117">Header</span></span>|<span data-ttu-id="558a7-118">Wert</span><span class="sxs-lookup"><span data-stu-id="558a7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="558a7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="558a7-119">Authorization</span></span>|<span data-ttu-id="558a7-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="558a7-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="558a7-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="558a7-121">Accept</span></span>|<span data-ttu-id="558a7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="558a7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="558a7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="558a7-123">Request body</span></span>
<span data-ttu-id="558a7-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/intune_onboarding_user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="558a7-124">In the request body, supply a JSON representation of [user](../resources/intune_onboarding_user.md) object.</span></span>

<span data-ttu-id="558a7-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [user](../resources/intune_onboarding_user.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="558a7-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="558a7-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="558a7-126">Property</span></span>|<span data-ttu-id="558a7-127">Typ</span><span class="sxs-lookup"><span data-stu-id="558a7-127">Type</span></span>|<span data-ttu-id="558a7-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="558a7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="558a7-129">id</span><span class="sxs-lookup"><span data-stu-id="558a7-129">id</span></span>|<span data-ttu-id="558a7-130">String</span><span class="sxs-lookup"><span data-stu-id="558a7-130">String</span></span>|<span data-ttu-id="558a7-131">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="558a7-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="558a7-132">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="558a7-132">deviceEnrollmentLimit</span></span>|<span data-ttu-id="558a7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="558a7-133">Int32</span></span>|<span data-ttu-id="558a7-134">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="558a7-134">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="558a7-135">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="558a7-135">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="558a7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="558a7-136">Response</span></span>
<span data-ttu-id="558a7-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [user](../resources/intune_onboarding_user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="558a7-137">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="558a7-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="558a7-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="558a7-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="558a7-139">Request</span></span>
<span data-ttu-id="558a7-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="558a7-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 34

{
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="558a7-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="558a7-141">Response</span></span>
<span data-ttu-id="558a7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="558a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```



