# <a name="update-ebookinstallsummary"></a><span data-ttu-id="e678f-101">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e678f-101">Update eBookInstallSummary</span></span>

> <span data-ttu-id="e678f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e678f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e678f-103">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e678f-103">Update the properties of a [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e678f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e678f-104">Prerequisites</span></span>
<span data-ttu-id="e678f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e678f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e678f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e678f-107">Permission type</span></span>|<span data-ttu-id="e678f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e678f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e678f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e678f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e678f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e678f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e678f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e678f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e678f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e678f-112">Not supported.</span></span>|
|<span data-ttu-id="e678f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e678f-113">Application</span></span>|<span data-ttu-id="e678f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e678f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e678f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e678f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="e678f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e678f-116">Request headers</span></span>
|<span data-ttu-id="e678f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e678f-117">Header</span></span>|<span data-ttu-id="e678f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e678f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e678f-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e678f-119">Authorization</span></span>|<span data-ttu-id="e678f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e678f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e678f-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="e678f-121">Accept</span></span>|<span data-ttu-id="e678f-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="e678f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e678f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e678f-123">Request body</span></span>
<span data-ttu-id="e678f-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="e678f-124">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="e678f-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e678f-125">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span></span>

|<span data-ttu-id="e678f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e678f-126">Property</span></span>|<span data-ttu-id="e678f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e678f-127">Type</span></span>|<span data-ttu-id="e678f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e678f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e678f-129">ID</span><span class="sxs-lookup"><span data-stu-id="e678f-129">id</span></span>|<span data-ttu-id="e678f-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e678f-130">String</span></span>|<span data-ttu-id="e678f-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e678f-131">Key of the entity.</span></span>|
|<span data-ttu-id="e678f-132">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e678f-132">installedDeviceCount</span></span>|<span data-ttu-id="e678f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e678f-133">Int32</span></span>|<span data-ttu-id="e678f-134">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="e678f-134">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="e678f-135">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e678f-135">failedDeviceCount</span></span>|<span data-ttu-id="e678f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e678f-136">Int32</span></span>|<span data-ttu-id="e678f-137">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="e678f-137">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="e678f-138">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e678f-138">notInstalledDeviceCount</span></span>|<span data-ttu-id="e678f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e678f-139">Int32</span></span>|<span data-ttu-id="e678f-140">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="e678f-140">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="e678f-141">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="e678f-141">installedUserCount</span></span>|<span data-ttu-id="e678f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e678f-142">Int32</span></span>|<span data-ttu-id="e678f-143">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="e678f-143">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="e678f-144">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="e678f-144">failedUserCount</span></span>|<span data-ttu-id="e678f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e678f-145">Int32</span></span>|<span data-ttu-id="e678f-146">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="e678f-146">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="e678f-147">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="e678f-147">notInstalledUserCount</span></span>|<span data-ttu-id="e678f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e678f-148">Int32</span></span>|<span data-ttu-id="e678f-149">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="e678f-149">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="e678f-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="e678f-150">Response</span></span>
<span data-ttu-id="e678f-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e678f-151">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e678f-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e678f-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="e678f-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e678f-153">Request</span></span>
<span data-ttu-id="e678f-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e678f-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="e678f-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="e678f-155">Response</span></span>
<span data-ttu-id="e678f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e678f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```








