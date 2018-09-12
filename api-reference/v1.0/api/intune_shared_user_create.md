# <a name="create-user"></a><span data-ttu-id="775f9-101">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="775f9-101">Create user</span></span>

> <span data-ttu-id="775f9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="775f9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="775f9-103">Dient zum Erstellen eines neuen [user](../resources/intune_shared_user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="775f9-103">Create a new [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="775f9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="775f9-104">Prerequisites</span></span>
<span data-ttu-id="775f9-105">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="775f9-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="775f9-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="775f9-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="775f9-107">Die spezifische erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="775f9-107">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="775f9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="775f9-108">Permission type</span></span>|<span data-ttu-id="775f9-109">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="775f9-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="775f9-110">Delegiert (Geschäfts- oder Schulkonto)</span><span class="sxs-lookup"><span data-stu-id="775f9-110">Delegated (work or school account)</span></span>| <span data-ttu-id="775f9-111">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="775f9-111">_varies by context_</span></span> |
| <span data-ttu-id="775f9-112">&nbsp; &nbsp; Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="775f9-112">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="775f9-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="775f9-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="775f9-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="775f9-114">.mam</span></span> | <span data-ttu-id="775f9-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="775f9-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="775f9-116">&nbsp; &nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="775f9-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="775f9-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="775f9-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="775f9-118">&nbsp; &nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="775f9-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="775f9-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="775f9-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="775f9-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="775f9-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="775f9-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="775f9-121">Not supported.</span></span>|
|<span data-ttu-id="775f9-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="775f9-122">Application</span></span>|<span data-ttu-id="775f9-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="775f9-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="775f9-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="775f9-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="775f9-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="775f9-125">Request headers</span></span>
|<span data-ttu-id="775f9-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="775f9-126">Header</span></span>|<span data-ttu-id="775f9-127">Wert</span><span class="sxs-lookup"><span data-stu-id="775f9-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="775f9-128">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="775f9-128">Authorization</span></span>|<span data-ttu-id="775f9-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="775f9-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="775f9-130">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="775f9-130">Accept</span></span>|<span data-ttu-id="775f9-131">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="775f9-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="775f9-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="775f9-132">Request body</span></span>
<span data-ttu-id="775f9-133">Geben Sie im Anforderungstext eine JSON-Darstellung des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="775f9-133">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="775f9-134">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="775f9-134">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="775f9-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="775f9-135">Property</span></span>|<span data-ttu-id="775f9-136">Typ</span><span class="sxs-lookup"><span data-stu-id="775f9-136">Type</span></span>|<span data-ttu-id="775f9-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="775f9-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="775f9-138">ID</span><span class="sxs-lookup"><span data-stu-id="775f9-138">id</span></span>|<span data-ttu-id="775f9-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="775f9-139">String</span></span>|<span data-ttu-id="775f9-140">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="775f9-140">Unique identifier of the user.</span></span>|
|<span data-ttu-id="775f9-141">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="775f9-141">**On-boarding**</span></span>|
|<span data-ttu-id="775f9-142">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="775f9-142">deviceEnrollmentLimit</span></span>|<span data-ttu-id="775f9-143">Int32</span><span class="sxs-lookup"><span data-stu-id="775f9-143">Int32</span></span>|<span data-ttu-id="775f9-144">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="775f9-144">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="775f9-145">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="775f9-145">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="775f9-146">Die Anforderung der Body-Eigenschaft-Unterstützung variiert je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="775f9-146">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="775f9-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="775f9-147">Response</span></span>
<span data-ttu-id="775f9-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/intune_shared_user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="775f9-148">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="775f9-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="775f9-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="775f9-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="775f9-150">Request</span></span>
<span data-ttu-id="775f9-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="775f9-151">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="775f9-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="775f9-152">Response</span></span>
<span data-ttu-id="775f9-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="775f9-153">Here is an example of the response.</span></span> <span data-ttu-id="775f9-154">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="775f9-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="775f9-155">Die von einem tatsächlichen Aufruf zurückgegebenen Eigenschaften variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="775f9-155">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



