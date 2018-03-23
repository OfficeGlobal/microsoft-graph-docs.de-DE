# <a name="update-userinstallstatesummary"></a><span data-ttu-id="96b64-101">Aktualisieren von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="96b64-101">Update userInstallStateSummary</span></span>

> <span data-ttu-id="96b64-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="96b64-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96b64-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="96b64-103">Update the properties of a [calendar](../resources/intune_books_userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96b64-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="96b64-104">Prerequisites</span></span>
<span data-ttu-id="96b64-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96b64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96b64-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96b64-107">Permission type</span></span>|<span data-ttu-id="96b64-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96b64-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96b64-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96b64-109">Delegated (work or school account)</span></span>|<span data-ttu-id="96b64-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96b64-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96b64-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96b64-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96b64-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96b64-112">Not supported.</span></span>|
|<span data-ttu-id="96b64-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96b64-113">Application</span></span>|<span data-ttu-id="96b64-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96b64-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96b64-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96b64-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="96b64-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96b64-116">Request headers</span></span>
|<span data-ttu-id="96b64-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="96b64-117">Header</span></span>|<span data-ttu-id="96b64-118">Wert</span><span class="sxs-lookup"><span data-stu-id="96b64-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96b64-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="96b64-119">Authorization</span></span>|<span data-ttu-id="96b64-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="96b64-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="96b64-121">Accept</span><span class="sxs-lookup"><span data-stu-id="96b64-121">Accept</span></span>|<span data-ttu-id="96b64-122">application/json</span><span class="sxs-lookup"><span data-stu-id="96b64-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96b64-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96b64-123">Request body</span></span>
<span data-ttu-id="96b64-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="96b64-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_books_userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="96b64-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="96b64-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="96b64-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96b64-126">Property</span></span>|<span data-ttu-id="96b64-127">Typ</span><span class="sxs-lookup"><span data-stu-id="96b64-127">Type</span></span>|<span data-ttu-id="96b64-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96b64-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96b64-129">id</span><span class="sxs-lookup"><span data-stu-id="96b64-129">id</span></span>|<span data-ttu-id="96b64-130">String</span><span class="sxs-lookup"><span data-stu-id="96b64-130">String</span></span>|<span data-ttu-id="96b64-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="96b64-131">Key of the setting.</span></span>|
|<span data-ttu-id="96b64-132">userName</span><span class="sxs-lookup"><span data-stu-id="96b64-132">UserName</span></span>|<span data-ttu-id="96b64-133">String</span><span class="sxs-lookup"><span data-stu-id="96b64-133">String</span></span>|<span data-ttu-id="96b64-134">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="96b64-134">User name.</span></span>|
|<span data-ttu-id="96b64-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96b64-135">installedDeviceCount</span></span>|<span data-ttu-id="96b64-136">Int32</span><span class="sxs-lookup"><span data-stu-id="96b64-136">Int32</span></span>|<span data-ttu-id="96b64-137">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="96b64-137">Installed Device Count.</span></span>|
|<span data-ttu-id="96b64-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96b64-138">failedDeviceCount</span></span>|<span data-ttu-id="96b64-139">Int32</span><span class="sxs-lookup"><span data-stu-id="96b64-139">Int32</span></span>|<span data-ttu-id="96b64-140">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="96b64-140">Failed Device Count.</span></span>|
|<span data-ttu-id="96b64-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96b64-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="96b64-142">Int32</span><span class="sxs-lookup"><span data-stu-id="96b64-142">Int32</span></span>|<span data-ttu-id="96b64-143">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="96b64-143">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="96b64-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="96b64-144">Response</span></span>
<span data-ttu-id="96b64-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="96b64-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_books_userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96b64-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96b64-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="96b64-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96b64-147">Request</span></span>
<span data-ttu-id="96b64-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96b64-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
Content-type: application/json
Content-length: 127

{
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="96b64-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="96b64-149">Response</span></span>
<span data-ttu-id="96b64-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96b64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



