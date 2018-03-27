# <a name="update-deviceappmanagement"></a><span data-ttu-id="747a6-101">Aktualisieren von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="747a6-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="747a6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="747a6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="747a6-103">Aktualisiert die Eigenschaften von Objekten des Typs [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="747a6-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="747a6-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="747a6-104">Prerequisites</span></span>
<span data-ttu-id="747a6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="747a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="747a6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="747a6-107">Permission type</span></span>|<span data-ttu-id="747a6-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="747a6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="747a6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="747a6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="747a6-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="747a6-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="747a6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="747a6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="747a6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="747a6-112">Not supported.</span></span>|
|<span data-ttu-id="747a6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="747a6-113">Application</span></span>|<span data-ttu-id="747a6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="747a6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="747a6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="747a6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="747a6-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="747a6-116">Request headers</span></span>
|<span data-ttu-id="747a6-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="747a6-117">Header</span></span>|<span data-ttu-id="747a6-118">Wert</span><span class="sxs-lookup"><span data-stu-id="747a6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="747a6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="747a6-119">Authorization</span></span>|<span data-ttu-id="747a6-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="747a6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="747a6-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="747a6-121">Accept</span></span>|<span data-ttu-id="747a6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="747a6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="747a6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="747a6-123">Request body</span></span>
<span data-ttu-id="747a6-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="747a6-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="747a6-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="747a6-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="747a6-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="747a6-126">Property</span></span>|<span data-ttu-id="747a6-127">Typ</span><span class="sxs-lookup"><span data-stu-id="747a6-127">Type</span></span>|<span data-ttu-id="747a6-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="747a6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="747a6-129">id</span><span class="sxs-lookup"><span data-stu-id="747a6-129">id</span></span>|<span data-ttu-id="747a6-130">String</span><span class="sxs-lookup"><span data-stu-id="747a6-130">String</span></span>|<span data-ttu-id="747a6-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="747a6-131">Not yet documented</span></span>|
|<span data-ttu-id="747a6-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="747a6-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="747a6-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="747a6-133">DateTimeOffset</span></span>|<span data-ttu-id="747a6-134">Zeitpunkt, zu dem das Konto die Apps letztmals erfolgreich mit dem Microsoft Store für Unternehmen synchronisiert hat</span><span class="sxs-lookup"><span data-stu-id="747a6-134">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="747a6-135">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="747a6-135">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="747a6-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="747a6-136">Boolean</span></span>|<span data-ttu-id="747a6-137">Gibt an, ob das Konto Anwendungen mit dem Microsoft Store für Unternehmen synchronisieren darf.</span><span class="sxs-lookup"><span data-stu-id="747a6-137">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="747a6-138">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="747a6-138">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="747a6-139">String</span><span class="sxs-lookup"><span data-stu-id="747a6-139">String</span></span>|<span data-ttu-id="747a6-140">Die Gebietsschemainformationen, die zur Synchronisierung von Anwendungen mit dem Microsoft Store für Unternehmen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="747a6-140">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="747a6-141">Angegeben werden Kulturen, die für ein Land bzw. eine Region spezifisch sind.</span><span class="sxs-lookup"><span data-stu-id="747a6-141">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="747a6-142">Die Namen dieser Kulturen folgen dem Standard RFC 4646 (Windows Vista und höher).</span><span class="sxs-lookup"><span data-stu-id="747a6-142">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="747a6-143">Das Format lautet <languagecode2>-<country/regioncode2>. Dabei ist <languagecode2> ein klein geschriebener Code aus zwei Buchstaben nach ISO 639-1 und <country/regioncode2> ein groß geschriebener Code aus zwei Buchstaben nach ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="747a6-143">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="747a6-144">Beispiel für eine spezifische Kultur: „en-US“ für „Englisch (Vereinigte Staaten)“.</span><span class="sxs-lookup"><span data-stu-id="747a6-144">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="747a6-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="747a6-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="747a6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="747a6-146">DateTimeOffset</span></span>|<span data-ttu-id="747a6-147">Zeitpunkt der letzten Anwendungssynchronisierung mit dem Microsoft Store für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="747a6-147">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|



## <a name="response"></a><span data-ttu-id="747a6-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="747a6-148">Response</span></span>
<span data-ttu-id="747a6-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="747a6-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="747a6-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="747a6-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="747a6-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="747a6-151">Request</span></span>
<span data-ttu-id="747a6-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="747a6-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 336

{
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```

### <a name="response"></a><span data-ttu-id="747a6-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="747a6-153">Response</span></span>
<span data-ttu-id="747a6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="747a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```



