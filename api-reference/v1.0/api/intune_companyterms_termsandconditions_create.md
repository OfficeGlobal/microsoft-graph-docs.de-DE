# <a name="create-termsandconditions"></a><span data-ttu-id="c618b-101">Erstellen von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="c618b-101">Create termsAndConditions</span></span>

> <span data-ttu-id="c618b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c618b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c618b-103">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="c618b-103">Create a new [plannerBucket](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c618b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c618b-104">Prerequisites</span></span>
<span data-ttu-id="c618b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c618b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c618b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c618b-107">Permission type</span></span>|<span data-ttu-id="c618b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c618b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c618b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c618b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c618b-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c618b-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c618b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c618b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c618b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c618b-112">Not supported.</span></span>|
|<span data-ttu-id="c618b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c618b-113">Application</span></span>|<span data-ttu-id="c618b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c618b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c618b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c618b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="c618b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c618b-116">Request headers</span></span>
|<span data-ttu-id="c618b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c618b-117">Header</span></span>|<span data-ttu-id="c618b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c618b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c618b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c618b-119">Authorization</span></span>|<span data-ttu-id="c618b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c618b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c618b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c618b-121">Accept</span></span>|<span data-ttu-id="c618b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c618b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c618b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c618b-123">Request body</span></span>
<span data-ttu-id="c618b-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditions“ an.</span><span class="sxs-lookup"><span data-stu-id="c618b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="c618b-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditions“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="c618b-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="c618b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c618b-126">Property</span></span>|<span data-ttu-id="c618b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c618b-127">Type</span></span>|<span data-ttu-id="c618b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c618b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c618b-129">id</span><span class="sxs-lookup"><span data-stu-id="c618b-129">id</span></span>|<span data-ttu-id="c618b-130">String</span><span class="sxs-lookup"><span data-stu-id="c618b-130">String</span></span>|<span data-ttu-id="c618b-131">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c618b-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="c618b-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c618b-132">createdDateTime</span></span>|<span data-ttu-id="c618b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c618b-133">DateTimeOffset</span></span>|<span data-ttu-id="c618b-134">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="c618b-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="c618b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c618b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c618b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c618b-136">DateTimeOffset</span></span>|<span data-ttu-id="c618b-137">Datum und Uhrzeit der letzten Änderung des Objekts</span><span class="sxs-lookup"><span data-stu-id="c618b-137">Indicates the date the object was last modified.</span></span>|
|<span data-ttu-id="c618b-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c618b-138">displayName</span></span>|<span data-ttu-id="c618b-139">String</span><span class="sxs-lookup"><span data-stu-id="c618b-139">String</span></span>|<span data-ttu-id="c618b-140">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="c618b-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="c618b-141">description</span><span class="sxs-lookup"><span data-stu-id="c618b-141">description</span></span>|<span data-ttu-id="c618b-142">String</span><span class="sxs-lookup"><span data-stu-id="c618b-142">String</span></span>|<span data-ttu-id="c618b-143">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="c618b-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="c618b-144">title</span><span class="sxs-lookup"><span data-stu-id="c618b-144">title</span></span>|<span data-ttu-id="c618b-145">String</span><span class="sxs-lookup"><span data-stu-id="c618b-145">String</span></span>|<span data-ttu-id="c618b-146">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c618b-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="c618b-147">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="c618b-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="c618b-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="c618b-148">BodyText</span></span>|<span data-ttu-id="c618b-149">String</span><span class="sxs-lookup"><span data-stu-id="c618b-149">String</span></span>|<span data-ttu-id="c618b-150">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="c618b-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="c618b-151">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="c618b-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="c618b-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="c618b-152">acceptanceStatement</span></span>|<span data-ttu-id="c618b-153">String</span><span class="sxs-lookup"><span data-stu-id="c618b-153">String</span></span>|<span data-ttu-id="c618b-154">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="c618b-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="c618b-155">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="c618b-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="c618b-156">version</span><span class="sxs-lookup"><span data-stu-id="c618b-156">version</span></span>|<span data-ttu-id="c618b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c618b-157">Int32</span></span>|<span data-ttu-id="c618b-158">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="c618b-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="c618b-159">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="c618b-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="c618b-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="c618b-160">Response</span></span>
<span data-ttu-id="c618b-161">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c618b-161">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c618b-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c618b-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="c618b-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c618b-163">Request</span></span>
<span data-ttu-id="c618b-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c618b-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c618b-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="c618b-165">Response</span></span>
<span data-ttu-id="c618b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c618b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



