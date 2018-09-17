# <a name="create-userinstallstatesummary"></a><span data-ttu-id="ec1fc-101">Erstellen von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="ec1fc-101">Create userInstallStateSummary</span></span>

> <span data-ttu-id="ec1fc-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ec1fc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec1fc-103">Diese Methode erstellt ein neues Objekt des Typs [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ec1fc-103">Create a new [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec1fc-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ec1fc-104">Prerequisites</span></span>
<span data-ttu-id="ec1fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec1fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ec1fc-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec1fc-107">Permission type</span></span>|<span data-ttu-id="ec1fc-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec1fc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec1fc-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec1fc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ec1fc-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec1fc-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec1fc-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec1fc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec1fc-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec1fc-112">Not supported.</span></span>|
|<span data-ttu-id="ec1fc-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec1fc-113">Application</span></span>|<span data-ttu-id="ec1fc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec1fc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec1fc-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec1fc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="ec1fc-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec1fc-116">Request headers</span></span>
|<span data-ttu-id="ec1fc-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ec1fc-117">Header</span></span>|<span data-ttu-id="ec1fc-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ec1fc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec1fc-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ec1fc-119">Authorization</span></span>|<span data-ttu-id="ec1fc-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ec1fc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec1fc-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="ec1fc-121">Accept</span></span>|<span data-ttu-id="ec1fc-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="ec1fc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec1fc-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec1fc-123">Request body</span></span>
<span data-ttu-id="ec1fc-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „userInstallStateSummary“ an.</span><span class="sxs-lookup"><span data-stu-id="ec1fc-124">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="ec1fc-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „userInstallStateSummary“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ec1fc-125">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="ec1fc-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec1fc-126">Property</span></span>|<span data-ttu-id="ec1fc-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ec1fc-127">Type</span></span>|<span data-ttu-id="ec1fc-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec1fc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec1fc-129">ID</span><span class="sxs-lookup"><span data-stu-id="ec1fc-129">id</span></span>|<span data-ttu-id="ec1fc-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec1fc-130">String</span></span>|<span data-ttu-id="ec1fc-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ec1fc-131">Key of the entity.</span></span>|
|<span data-ttu-id="ec1fc-132">userName</span><span class="sxs-lookup"><span data-stu-id="ec1fc-132">userName</span></span>|<span data-ttu-id="ec1fc-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec1fc-133">String</span></span>|<span data-ttu-id="ec1fc-134">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="ec1fc-134">User name.</span></span>|
|<span data-ttu-id="ec1fc-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec1fc-135">installedDeviceCount</span></span>|<span data-ttu-id="ec1fc-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ec1fc-136">Int32</span></span>|<span data-ttu-id="ec1fc-137">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="ec1fc-137">Installed Device Count.</span></span>|
|<span data-ttu-id="ec1fc-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec1fc-138">failedDeviceCount</span></span>|<span data-ttu-id="ec1fc-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ec1fc-139">Int32</span></span>|<span data-ttu-id="ec1fc-140">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="ec1fc-140">Failed Device Count.</span></span>|
|<span data-ttu-id="ec1fc-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec1fc-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="ec1fc-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ec1fc-142">Int32</span></span>|<span data-ttu-id="ec1fc-143">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="ec1fc-143">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="ec1fc-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec1fc-144">Response</span></span>
<span data-ttu-id="ec1fc-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ec1fc-145">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec1fc-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec1fc-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec1fc-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec1fc-147">Request</span></span>
<span data-ttu-id="ec1fc-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec1fc-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="ec1fc-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec1fc-149">Response</span></span>
<span data-ttu-id="ec1fc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec1fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```








