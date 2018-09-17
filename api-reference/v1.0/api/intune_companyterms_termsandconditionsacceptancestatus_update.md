# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="87931-101">Aktualisieren von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="87931-101">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="87931-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="87931-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87931-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="87931-103">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87931-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="87931-104">Prerequisites</span></span>
<span data-ttu-id="87931-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87931-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87931-107">Permission type</span></span>|<span data-ttu-id="87931-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87931-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87931-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87931-109">Delegated (work or school account)</span></span>|<span data-ttu-id="87931-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87931-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="87931-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87931-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87931-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87931-112">Not supported.</span></span>|
|<span data-ttu-id="87931-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87931-113">Application</span></span>|<span data-ttu-id="87931-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87931-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87931-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87931-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="87931-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87931-116">Request headers</span></span>
|<span data-ttu-id="87931-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="87931-117">Header</span></span>|<span data-ttu-id="87931-118">Wert</span><span class="sxs-lookup"><span data-stu-id="87931-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87931-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="87931-119">Authorization</span></span>|<span data-ttu-id="87931-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="87931-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87931-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="87931-121">Accept</span></span>|<span data-ttu-id="87931-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="87931-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87931-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87931-123">Request body</span></span>
<span data-ttu-id="87931-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="87931-124">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="87931-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="87931-125">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="87931-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87931-126">Property</span></span>|<span data-ttu-id="87931-127">Typ</span><span class="sxs-lookup"><span data-stu-id="87931-127">Type</span></span>|<span data-ttu-id="87931-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87931-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87931-129">ID</span><span class="sxs-lookup"><span data-stu-id="87931-129">id</span></span>|<span data-ttu-id="87931-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87931-130">String</span></span>|<span data-ttu-id="87931-131">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="87931-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="87931-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="87931-132">userDisplayName</span></span>|<span data-ttu-id="87931-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87931-133">String</span></span>|<span data-ttu-id="87931-134">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="87931-134">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="87931-135">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="87931-135">acceptedVersion</span></span>|<span data-ttu-id="87931-136">Int32</span><span class="sxs-lookup"><span data-stu-id="87931-136">Int32</span></span>|<span data-ttu-id="87931-137">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="87931-137">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="87931-138">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="87931-138">acceptedDateTime</span></span>|<span data-ttu-id="87931-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87931-139">DateTimeOffset</span></span>|<span data-ttu-id="87931-140">Datum und Uhrzeit der letzten Zustimmung zu den Bedingungen durch den Benutzer</span><span class="sxs-lookup"><span data-stu-id="87931-140">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="87931-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="87931-141">Response</span></span>
<span data-ttu-id="87931-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="87931-142">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87931-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87931-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="87931-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87931-144">Request</span></span>
<span data-ttu-id="87931-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87931-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 138

{
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="87931-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="87931-146">Response</span></span>
<span data-ttu-id="87931-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87931-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```








