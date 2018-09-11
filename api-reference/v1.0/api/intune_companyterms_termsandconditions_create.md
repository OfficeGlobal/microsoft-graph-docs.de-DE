# <a name="create-termsandconditions"></a><span data-ttu-id="3bbc5-101">Erstellen von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="3bbc5-101">Create termsAndConditions</span></span>

> <span data-ttu-id="3bbc5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bbc5-103">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="3bbc5-103">Create a new [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3bbc5-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3bbc5-104">Prerequisites</span></span>
<span data-ttu-id="3bbc5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3bbc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3bbc5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3bbc5-107">Permission type</span></span>|<span data-ttu-id="3bbc5-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3bbc5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bbc5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3bbc5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3bbc5-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bbc5-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3bbc5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3bbc5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bbc5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3bbc5-112">Not supported.</span></span>|
|<span data-ttu-id="3bbc5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3bbc5-113">Application</span></span>|<span data-ttu-id="3bbc5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3bbc5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bbc5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3bbc5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="3bbc5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3bbc5-116">Request headers</span></span>
|<span data-ttu-id="3bbc5-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3bbc5-117">Header</span></span>|<span data-ttu-id="3bbc5-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3bbc5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bbc5-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3bbc5-119">Authorization</span></span>|<span data-ttu-id="3bbc5-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3bbc5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bbc5-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="3bbc5-121">Accept</span></span>|<span data-ttu-id="3bbc5-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="3bbc5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bbc5-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3bbc5-123">Request body</span></span>
<span data-ttu-id="3bbc5-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditions“ an.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-124">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="3bbc5-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditions“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-125">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="3bbc5-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3bbc5-126">Property</span></span>|<span data-ttu-id="3bbc5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3bbc5-127">Type</span></span>|<span data-ttu-id="3bbc5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bbc5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bbc5-129">ID</span><span class="sxs-lookup"><span data-stu-id="3bbc5-129">id</span></span>|<span data-ttu-id="3bbc5-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3bbc5-130">String</span></span>|<span data-ttu-id="3bbc5-131">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3bbc5-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="3bbc5-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bbc5-132">createdDateTime</span></span>|<span data-ttu-id="3bbc5-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bbc5-133">DateTimeOffset</span></span>|<span data-ttu-id="3bbc5-134">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="3bbc5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bbc5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3bbc5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bbc5-136">DateTimeOffset</span></span>|<span data-ttu-id="3bbc5-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3bbc5-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3bbc5-138">displayName</span></span>|<span data-ttu-id="3bbc5-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3bbc5-139">String</span></span>|<span data-ttu-id="3bbc5-140">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="3bbc5-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="3bbc5-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bbc5-141">description</span></span>|<span data-ttu-id="3bbc5-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3bbc5-142">String</span></span>|<span data-ttu-id="3bbc5-143">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="3bbc5-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="3bbc5-144">Titel</span><span class="sxs-lookup"><span data-stu-id="3bbc5-144">title</span></span>|<span data-ttu-id="3bbc5-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3bbc5-145">String</span></span>|<span data-ttu-id="3bbc5-146">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3bbc5-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="3bbc5-147">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3bbc5-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="3bbc5-148">bodyText</span></span>|<span data-ttu-id="3bbc5-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3bbc5-149">String</span></span>|<span data-ttu-id="3bbc5-150">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="3bbc5-151">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3bbc5-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="3bbc5-152">acceptanceStatement</span></span>|<span data-ttu-id="3bbc5-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3bbc5-153">String</span></span>|<span data-ttu-id="3bbc5-154">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="3bbc5-155">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3bbc5-156">Version</span><span class="sxs-lookup"><span data-stu-id="3bbc5-156">version</span></span>|<span data-ttu-id="3bbc5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbc5-157">Int32</span></span>|<span data-ttu-id="3bbc5-158">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="3bbc5-159">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="3bbc5-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="3bbc5-160">Response</span></span>
<span data-ttu-id="3bbc5-161">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-161">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bbc5-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3bbc5-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="3bbc5-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3bbc5-163">Request</span></span>
<span data-ttu-id="3bbc5-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 337

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="3bbc5-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="3bbc5-165">Response</span></span>
<span data-ttu-id="3bbc5-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3bbc5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```








