# <a name="update-user"></a><span data-ttu-id="a6fb1-101">Benutzer aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a6fb1-101">Update user</span></span>

> <span data-ttu-id="a6fb1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a6fb1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6fb1-103">Aktualisieren der Eigenschaften eines [user](../resources/intune_shared_user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6fb1-103">Update the properties of a [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6fb1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a6fb1-104">Prerequisites</span></span>
<span data-ttu-id="a6fb1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6fb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a6fb1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6fb1-107">Permission type</span></span>|<span data-ttu-id="a6fb1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6fb1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6fb1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6fb1-109">Delegated (work or school account)</span></span>| <span data-ttu-id="a6fb1-110">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="a6fb1-110">_varies by context_</span></span>|
| <span data-ttu-id="a6fb1-111">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="a6fb1-111">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="a6fb1-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6fb1-112">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="a6fb1-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="a6fb1-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="a6fb1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6fb1-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="a6fb1-115">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="a6fb1-115">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="a6fb1-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6fb1-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="a6fb1-117">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="a6fb1-117">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="a6fb1-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6fb1-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="a6fb1-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6fb1-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6fb1-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6fb1-120">Not supported.</span></span>|
|<span data-ttu-id="a6fb1-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6fb1-121">Application</span></span>|<span data-ttu-id="a6fb1-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6fb1-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6fb1-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6fb1-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="a6fb1-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6fb1-124">Request headers</span></span>
|<span data-ttu-id="a6fb1-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a6fb1-125">Header</span></span>|<span data-ttu-id="a6fb1-126">Wert</span><span class="sxs-lookup"><span data-stu-id="a6fb1-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6fb1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6fb1-127">Authorization</span></span>|<span data-ttu-id="a6fb1-128">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a6fb1-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6fb1-129">Accept</span><span class="sxs-lookup"><span data-stu-id="a6fb1-129">Accept</span></span>|<span data-ttu-id="a6fb1-130">application/json</span><span class="sxs-lookup"><span data-stu-id="a6fb1-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6fb1-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6fb1-131">Request body</span></span>
<span data-ttu-id="a6fb1-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/intune_shared_user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a6fb1-132">In the request body, supply a JSON representation for the [user](../resources/intune_shared_user.md) object.</span></span>

<span data-ttu-id="a6fb1-133">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [user](../resources/intune_shared_user.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a6fb1-133">The following table shows the properties that are required when you create the [user](../resources/intune_shared_user.md).</span></span>

|<span data-ttu-id="a6fb1-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6fb1-134">Property</span></span>|<span data-ttu-id="a6fb1-135">Typ</span><span class="sxs-lookup"><span data-stu-id="a6fb1-135">Type</span></span>|<span data-ttu-id="a6fb1-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6fb1-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6fb1-137">id</span><span class="sxs-lookup"><span data-stu-id="a6fb1-137">id</span></span>|<span data-ttu-id="a6fb1-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a6fb1-138">String</span></span>|<span data-ttu-id="a6fb1-139">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="a6fb1-139">Unique identifier of the user.</span></span>|
|<span data-ttu-id="a6fb1-140">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="a6fb1-140">**Onboarding**</span></span>|
|<span data-ttu-id="a6fb1-141">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="a6fb1-141">deviceEnrollmentLimit</span></span>|<span data-ttu-id="a6fb1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a6fb1-142">Int32</span></span>|<span data-ttu-id="a6fb1-143">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="a6fb1-143">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="a6fb1-144">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="a6fb1-144">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="a6fb1-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6fb1-145">Response</span></span>
<span data-ttu-id="a6fb1-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [user](../resources/intune_shared_user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6fb1-146">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6fb1-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6fb1-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6fb1-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6fb1-148">Request</span></span>
<span data-ttu-id="a6fb1-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6fb1-149">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="a6fb1-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6fb1-150">Response</span></span>
<span data-ttu-id="a6fb1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6fb1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



