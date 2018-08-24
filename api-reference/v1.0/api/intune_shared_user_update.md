# <a name="update-user"></a><span data-ttu-id="96263-101">Benutzer aktualisieren</span><span class="sxs-lookup"><span data-stu-id="96263-101">Update user</span></span>

> <span data-ttu-id="96263-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="96263-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96263-103">Aktualisieren der Eigenschaften eines [user](../resources/intune_shared_user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="96263-103">Update the properties of a [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96263-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="96263-104">Prerequisites</span></span>
<span data-ttu-id="96263-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96263-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96263-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96263-107">Permission type</span></span>|<span data-ttu-id="96263-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96263-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96263-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96263-109">Delegated (work or school account)</span></span>| <span data-ttu-id="96263-110">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="96263-110">_varies by context_</span></span>|
| <span data-ttu-id="96263-111">&nbsp; &nbsp; Geräte</span><span class="sxs-lookup"><span data-stu-id="96263-111">&nbsp;&nbsp;</span></span> | <span data-ttu-id="96263-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96263-112">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="96263-113">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="96263-113">.mam</span></span> | <span data-ttu-id="96263-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96263-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="96263-115">&nbsp; &nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="96263-115">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="96263-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96263-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="96263-117">&nbsp; &nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="96263-117">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="96263-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96263-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="96263-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96263-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96263-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96263-120">Not supported.</span></span>|
|<span data-ttu-id="96263-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96263-121">Application</span></span>|<span data-ttu-id="96263-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96263-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96263-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96263-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="96263-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96263-124">Request headers</span></span>
|<span data-ttu-id="96263-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="96263-125">Header</span></span>|<span data-ttu-id="96263-126">Wert</span><span class="sxs-lookup"><span data-stu-id="96263-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96263-127">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="96263-127">Authorization</span></span>|<span data-ttu-id="96263-128">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="96263-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96263-129">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="96263-129">Accept</span></span>|<span data-ttu-id="96263-130">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="96263-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96263-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96263-131">Request body</span></span>
<span data-ttu-id="96263-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/intune_shared_user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="96263-132">In the request body, supply a JSON representation for the [user](../resources/intune_shared_user.md) object.</span></span>

<span data-ttu-id="96263-133">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [user](../resources/intune_shared_user.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="96263-133">The following table shows the properties that are required when you create the [user](../resources/intune_shared_user.md).</span></span>

|<span data-ttu-id="96263-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96263-134">Property</span></span>|<span data-ttu-id="96263-135">Typ</span><span class="sxs-lookup"><span data-stu-id="96263-135">Type</span></span>|<span data-ttu-id="96263-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96263-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96263-137">id</span><span class="sxs-lookup"><span data-stu-id="96263-137">id</span></span>|<span data-ttu-id="96263-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96263-138">String</span></span>|<span data-ttu-id="96263-139">Eindeutige Kennung für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="96263-139">Unique identifier of the user.</span></span>|
|<span data-ttu-id="96263-140">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="96263-140">**On-boarding**</span></span>|
|<span data-ttu-id="96263-141">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="96263-141">deviceEnrollmentLimit</span></span>|<span data-ttu-id="96263-142">Int32</span><span class="sxs-lookup"><span data-stu-id="96263-142">Int32</span></span>|<span data-ttu-id="96263-143">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="96263-143">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="96263-144">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="96263-144">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="96263-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="96263-145">Response</span></span>
<span data-ttu-id="96263-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [user](../resources/intune_shared_user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96263-146">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96263-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96263-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="96263-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96263-148">Request</span></span>
<span data-ttu-id="96263-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96263-149">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="96263-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="96263-150">Response</span></span>
<span data-ttu-id="96263-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96263-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



