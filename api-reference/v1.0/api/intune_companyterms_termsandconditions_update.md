# <a name="update-termsandconditions"></a><span data-ttu-id="e8eef-101">Aktualisieren von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="e8eef-101">Update termsAndConditions</span></span>

> <span data-ttu-id="e8eef-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e8eef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8eef-103">Aktualisieren der Eigenschaften eines [termsAndConditions](../resources/intune_companyterms_termsandconditions.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8eef-103">Update the properties of a [calendar](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8eef-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e8eef-104">Prerequisites</span></span>
<span data-ttu-id="e8eef-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8eef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8eef-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8eef-107">Permission type</span></span>|<span data-ttu-id="e8eef-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8eef-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8eef-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8eef-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e8eef-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8eef-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e8eef-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8eef-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8eef-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8eef-112">Not supported.</span></span>|
|<span data-ttu-id="e8eef-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8eef-113">Application</span></span>|<span data-ttu-id="e8eef-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8eef-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8eef-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8eef-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="e8eef-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8eef-116">Request headers</span></span>
|<span data-ttu-id="e8eef-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e8eef-117">Header</span></span>|<span data-ttu-id="e8eef-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e8eef-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8eef-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8eef-119">Authorization</span></span>|<span data-ttu-id="e8eef-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e8eef-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e8eef-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e8eef-121">Accept</span></span>|<span data-ttu-id="e8eef-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e8eef-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8eef-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8eef-123">Request body</span></span>
<span data-ttu-id="e8eef-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [termsAndConditions](../resources/intune_companyterms_termsandconditions.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e8eef-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_companyterms_termsandconditions.md) object.</span></span>

<span data-ttu-id="e8eef-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e8eef-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="e8eef-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e8eef-126">Property</span></span>|<span data-ttu-id="e8eef-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e8eef-127">Type</span></span>|<span data-ttu-id="e8eef-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8eef-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8eef-129">id</span><span class="sxs-lookup"><span data-stu-id="e8eef-129">id</span></span>|<span data-ttu-id="e8eef-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8eef-130">String</span></span>|<span data-ttu-id="e8eef-131">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="e8eef-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="e8eef-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8eef-132">createdDateTime</span></span>|<span data-ttu-id="e8eef-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8eef-133">DateTimeOffset</span></span>|<span data-ttu-id="e8eef-134">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8eef-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="e8eef-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8eef-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e8eef-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8eef-136">DateTimeOffset</span></span>|<span data-ttu-id="e8eef-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8eef-137">Indicates the date the object was last modified.</span></span>|
|<span data-ttu-id="e8eef-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e8eef-138">displayName</span></span>|<span data-ttu-id="e8eef-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8eef-139">String</span></span>|<span data-ttu-id="e8eef-140">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e8eef-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="e8eef-141">description</span><span class="sxs-lookup"><span data-stu-id="e8eef-141">description</span></span>|<span data-ttu-id="e8eef-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8eef-142">String</span></span>|<span data-ttu-id="e8eef-143">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e8eef-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="e8eef-144">title</span><span class="sxs-lookup"><span data-stu-id="e8eef-144">title</span></span>|<span data-ttu-id="e8eef-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8eef-145">String</span></span>|<span data-ttu-id="e8eef-146">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e8eef-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="e8eef-147">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="e8eef-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e8eef-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="e8eef-148">BodyText</span></span>|<span data-ttu-id="e8eef-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8eef-149">String</span></span>|<span data-ttu-id="e8eef-150">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="e8eef-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="e8eef-151">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="e8eef-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e8eef-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="e8eef-152">acceptanceStatement</span></span>|<span data-ttu-id="e8eef-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8eef-153">String</span></span>|<span data-ttu-id="e8eef-154">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreiben in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="e8eef-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="e8eef-155">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="e8eef-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e8eef-156">Version</span><span class="sxs-lookup"><span data-stu-id="e8eef-156">version</span></span>|<span data-ttu-id="e8eef-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e8eef-157">Int32</span></span>|<span data-ttu-id="e8eef-158">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="e8eef-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="e8eef-159">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderten Bedingungen erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="e8eef-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="e8eef-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8eef-160">Response</span></span>
<span data-ttu-id="e8eef-161">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [termsAndConditions](../resources/intune_companyterms_termsandconditions.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8eef-161">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8eef-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8eef-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8eef-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8eef-163">Request</span></span>
<span data-ttu-id="e8eef-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8eef-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 280

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="e8eef-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8eef-165">Response</span></span>
<span data-ttu-id="e8eef-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8eef-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



