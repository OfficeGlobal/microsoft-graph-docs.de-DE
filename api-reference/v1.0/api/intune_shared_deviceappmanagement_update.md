# <a name="update-deviceappmanagement"></a><span data-ttu-id="7e708-101">Aktualisieren von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="7e708-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="7e708-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7e708-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e708-103">Aktualisiert die Eigenschaften von Objekten des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7e708-103">Update the properties of a [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e708-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7e708-104">Prerequisites</span></span>
<span data-ttu-id="7e708-105">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="7e708-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="7e708-106">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e708-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="7e708-107">Beachten Sie, dass die entsprechende Berechtigung gemäß dem Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="7e708-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="7e708-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7e708-108">Permission type</span></span>|<span data-ttu-id="7e708-109">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7e708-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e708-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7e708-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7e708-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e708-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e708-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7e708-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e708-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e708-113">Not supported.</span></span>|
|<span data-ttu-id="7e708-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7e708-114">Application</span></span>|<span data-ttu-id="7e708-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e708-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e708-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e708-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="7e708-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e708-117">Request headers</span></span>
|<span data-ttu-id="7e708-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7e708-118">Header</span></span>|<span data-ttu-id="7e708-119">Wert</span><span class="sxs-lookup"><span data-stu-id="7e708-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e708-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7e708-120">Authorization</span></span>|<span data-ttu-id="7e708-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7e708-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e708-122">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="7e708-122">Accept</span></span>|<span data-ttu-id="7e708-123">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="7e708-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e708-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e708-124">Request body</span></span>
<span data-ttu-id="7e708-125">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="7e708-125">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="7e708-126">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7e708-126">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span></span>

|<span data-ttu-id="7e708-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e708-127">Property</span></span>|<span data-ttu-id="7e708-128">Typ</span><span class="sxs-lookup"><span data-stu-id="7e708-128">Type</span></span>|<span data-ttu-id="7e708-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e708-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e708-130">id</span><span class="sxs-lookup"><span data-stu-id="7e708-130">id</span></span>|<span data-ttu-id="7e708-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e708-131">String</span></span>|<span data-ttu-id="7e708-132">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7e708-132">Key of the entity.</span></span>|
|<span data-ttu-id="7e708-133">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="7e708-133">**On-boarding**</span></span>|
|<span data-ttu-id="7e708-134">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="7e708-134">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="7e708-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7e708-135">Boolean</span></span>|<span data-ttu-id="7e708-136">Gibt an, ob das Konto Anwendungen mit dem Microsoft Store für Unternehmen synchronisieren darf.</span><span class="sxs-lookup"><span data-stu-id="7e708-136">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="7e708-137">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="7e708-137">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="7e708-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e708-138">String</span></span>|<span data-ttu-id="7e708-139">Die Gebietsschemainformationen, die zur Synchronisierung von Anwendungen mit dem Microsoft Store für Unternehmen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="7e708-139">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="7e708-140">Angegeben werden Kulturen, die für ein Land bzw. eine Region spezifisch sind.</span><span class="sxs-lookup"><span data-stu-id="7e708-140">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="7e708-141">Die Namen dieser Kulturen folgen dem Standard RFC 4646 (Windows Vista und höher).</span><span class="sxs-lookup"><span data-stu-id="7e708-141">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="7e708-142">Das Format lautet <languagecode2>-<country/regioncode2>. Dabei ist <languagecode2> ein klein geschriebener Code aus zwei Buchstaben nach ISO 639-1 und <country/regioncode2> ein groß geschriebener Code aus zwei Buchstaben nach ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="7e708-142">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="7e708-143">Beispiel für eine spezifische Kultur: „en-US“ für „Englisch (Vereinigte Staaten)“.</span><span class="sxs-lookup"><span data-stu-id="7e708-143">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="7e708-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="7e708-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="7e708-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e708-145">DateTimeOffset</span></span>|<span data-ttu-id="7e708-146">Zeitpunkt der letzten Anwendungssynchronisierung mit dem Microsoft Store für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="7e708-146">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="7e708-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7e708-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="7e708-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e708-148">DateTimeOffset</span></span>|<span data-ttu-id="7e708-149">Zeitpunkt, zu dem das Konto die Apps letztmals erfolgreich mit dem Microsoft Store für Unternehmen synchronisiert hat</span><span class="sxs-lookup"><span data-stu-id="7e708-149">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="7e708-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e708-150">Response</span></span>
<span data-ttu-id="7e708-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7e708-151">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="7e708-152">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="7e708-152">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="7e708-153">Beispielantwort</span><span class="sxs-lookup"><span data-stu-id="7e708-153">Example response</span></span>

<span data-ttu-id="7e708-154">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="7e708-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7e708-155">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e708-155">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



