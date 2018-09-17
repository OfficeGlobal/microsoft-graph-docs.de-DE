# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="41e2f-101">Erstellen von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="41e2f-101">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="41e2f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="41e2f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41e2f-103">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="41e2f-103">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41e2f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="41e2f-104">Prerequisites</span></span>
<span data-ttu-id="41e2f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="41e2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="41e2f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41e2f-107">Permission type</span></span>|<span data-ttu-id="41e2f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41e2f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41e2f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41e2f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="41e2f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41e2f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="41e2f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41e2f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41e2f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41e2f-112">Not supported.</span></span>|
|<span data-ttu-id="41e2f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41e2f-113">Application</span></span>|<span data-ttu-id="41e2f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41e2f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41e2f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41e2f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="41e2f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="41e2f-116">Request headers</span></span>
|<span data-ttu-id="41e2f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="41e2f-117">Header</span></span>|<span data-ttu-id="41e2f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="41e2f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41e2f-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="41e2f-119">Authorization</span></span>|<span data-ttu-id="41e2f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="41e2f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41e2f-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="41e2f-121">Accept</span></span>|<span data-ttu-id="41e2f-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="41e2f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41e2f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="41e2f-123">Request body</span></span>
<span data-ttu-id="41e2f-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditionsAcceptanceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="41e2f-124">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="41e2f-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditionsAcceptanceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="41e2f-125">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="41e2f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41e2f-126">Property</span></span>|<span data-ttu-id="41e2f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="41e2f-127">Type</span></span>|<span data-ttu-id="41e2f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41e2f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41e2f-129">ID</span><span class="sxs-lookup"><span data-stu-id="41e2f-129">id</span></span>|<span data-ttu-id="41e2f-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="41e2f-130">String</span></span>|<span data-ttu-id="41e2f-131">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="41e2f-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="41e2f-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="41e2f-132">userDisplayName</span></span>|<span data-ttu-id="41e2f-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="41e2f-133">String</span></span>|<span data-ttu-id="41e2f-134">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="41e2f-134">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="41e2f-135">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="41e2f-135">acceptedVersion</span></span>|<span data-ttu-id="41e2f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="41e2f-136">Int32</span></span>|<span data-ttu-id="41e2f-137">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="41e2f-137">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="41e2f-138">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="41e2f-138">acceptedDateTime</span></span>|<span data-ttu-id="41e2f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41e2f-139">DateTimeOffset</span></span>|<span data-ttu-id="41e2f-140">Datum und Uhrzeit der letzten Zustimmung zu den Bedingungen durch den Benutzer</span><span class="sxs-lookup"><span data-stu-id="41e2f-140">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="41e2f-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="41e2f-141">Response</span></span>
<span data-ttu-id="41e2f-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="41e2f-142">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e2f-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41e2f-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="41e2f-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41e2f-144">Request</span></span>
<span data-ttu-id="41e2f-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41e2f-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="41e2f-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="41e2f-146">Response</span></span>
<span data-ttu-id="41e2f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41e2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








