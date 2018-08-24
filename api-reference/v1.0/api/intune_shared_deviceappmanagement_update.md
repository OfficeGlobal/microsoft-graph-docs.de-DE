# <a name="update-deviceappmanagement"></a><span data-ttu-id="1a748-101">Aktualisieren von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="1a748-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="1a748-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1a748-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a748-103">Aktualisiert die Eigenschaften von Objekten des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="1a748-103">Update the properties of a [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a748-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1a748-104">Prerequisites</span></span>
<span data-ttu-id="1a748-105">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="1a748-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="1a748-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1a748-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="1a748-107">Beachten Sie, dass die entsprechende Berechtigung gemäß dem Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="1a748-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="1a748-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a748-108">Permission type</span></span>|<span data-ttu-id="1a748-109">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a748-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a748-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a748-110">Delegated (work or school account)</span></span>|<span data-ttu-id="1a748-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a748-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a748-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a748-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a748-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a748-113">Not supported.</span></span>|
|<span data-ttu-id="1a748-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a748-114">Application</span></span>|<span data-ttu-id="1a748-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a748-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a748-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a748-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="1a748-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a748-117">Request headers</span></span>
|<span data-ttu-id="1a748-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1a748-118">Header</span></span>|<span data-ttu-id="1a748-119">Wert</span><span class="sxs-lookup"><span data-stu-id="1a748-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a748-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1a748-120">Authorization</span></span>|<span data-ttu-id="1a748-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1a748-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a748-122">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="1a748-122">Accept</span></span>|<span data-ttu-id="1a748-123">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="1a748-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a748-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a748-124">Request body</span></span>
<span data-ttu-id="1a748-125">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="1a748-125">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="1a748-126">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1a748-126">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span></span>

|<span data-ttu-id="1a748-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a748-127">Property</span></span>|<span data-ttu-id="1a748-128">Typ</span><span class="sxs-lookup"><span data-stu-id="1a748-128">Type</span></span>|<span data-ttu-id="1a748-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a748-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a748-130">id</span><span class="sxs-lookup"><span data-stu-id="1a748-130">id</span></span>|<span data-ttu-id="1a748-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a748-131">String</span></span>|<span data-ttu-id="1a748-132">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="1a748-132">Key of the entity.</span></span>|
|<span data-ttu-id="1a748-133">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="1a748-133">**On-boarding**</span></span>|
|<span data-ttu-id="1a748-134">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="1a748-134">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="1a748-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1a748-135">Boolean</span></span>|<span data-ttu-id="1a748-136">Gibt an, ob das Konto Anwendungen mit dem Microsoft Store für Unternehmen synchronisieren darf.</span><span class="sxs-lookup"><span data-stu-id="1a748-136">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="1a748-137">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="1a748-137">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="1a748-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a748-138">String</span></span>|<span data-ttu-id="1a748-139">Die Gebietsschemainformationen, die zur Synchronisierung von Anwendungen mit dem Microsoft Store für Unternehmen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="1a748-139">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="1a748-140">Angegeben werden Kulturen, die für ein Land bzw. eine Region spezifisch sind.</span><span class="sxs-lookup"><span data-stu-id="1a748-140">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="1a748-141">Die Namen dieser Kulturen folgen dem Standard RFC 4646 (Windows Vista und höher).</span><span class="sxs-lookup"><span data-stu-id="1a748-141">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="1a748-142">Das Format lautet <languagecode2>-<country/regioncode2>. Dabei ist <languagecode2> ein klein geschriebener Code aus zwei Buchstaben nach ISO 639-1 und <country/regioncode2> ein groß geschriebener Code aus zwei Buchstaben nach ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="1a748-142">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="1a748-143">Beispiel für eine spezifische Kultur: „en-US“ für „Englisch (Vereinigte Staaten)“.</span><span class="sxs-lookup"><span data-stu-id="1a748-143">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="1a748-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="1a748-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="1a748-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a748-145">DateTimeOffset</span></span>|<span data-ttu-id="1a748-146">Zeitpunkt der letzten Anwendungssynchronisierung mit dem Microsoft Store für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="1a748-146">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="1a748-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1a748-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="1a748-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a748-148">DateTimeOffset</span></span>|<span data-ttu-id="1a748-149">Zeitpunkt, zu dem das Konto die Apps letztmals erfolgreich mit dem Microsoft Store für Unternehmen synchronisiert hat.</span><span class="sxs-lookup"><span data-stu-id="1a748-149">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="1a748-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a748-150">Response</span></span>
<span data-ttu-id="1a748-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1a748-151">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a748-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a748-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a748-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a748-153">Request</span></span>
<span data-ttu-id="1a748-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a748-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="1a748-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a748-155">Response</span></span>
<span data-ttu-id="1a748-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a748-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



