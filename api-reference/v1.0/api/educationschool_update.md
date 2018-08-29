# <a name="update-educationschool-properties"></a><span data-ttu-id="5357b-101">Educationschool-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5357b-101">Update educationschool properties</span></span>

<span data-ttu-id="5357b-102">Aktualisieren der Eigenschaften eines school-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5357b-102">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5357b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5357b-103">Permissions</span></span>
<span data-ttu-id="5357b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5357b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5357b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5357b-106">Permission type</span></span>      | <span data-ttu-id="5357b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5357b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5357b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5357b-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="5357b-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5357b-109">Not supported.</span></span>  |
|<span data-ttu-id="5357b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5357b-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5357b-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5357b-111">Not supported.</span></span>  |
|<span data-ttu-id="5357b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5357b-112">Application</span></span> | <span data-ttu-id="5357b-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5357b-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5357b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5357b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5357b-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5357b-115">Request headers</span></span>
| <span data-ttu-id="5357b-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5357b-116">Header</span></span>       | <span data-ttu-id="5357b-117">Wert</span><span class="sxs-lookup"><span data-stu-id="5357b-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5357b-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5357b-118">Authorization</span></span>  | <span data-ttu-id="5357b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5357b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5357b-121">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="5357b-121">Content-Type</span></span>  | <span data-ttu-id="5357b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5357b-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5357b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5357b-123">Request body</span></span>
<span data-ttu-id="5357b-124">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5357b-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5357b-125">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="5357b-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5357b-126">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="5357b-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5357b-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5357b-127">Property</span></span>     | <span data-ttu-id="5357b-128">Typ</span><span class="sxs-lookup"><span data-stu-id="5357b-128">Type</span></span>   |<span data-ttu-id="5357b-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5357b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5357b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="5357b-130">displayName</span></span>| <span data-ttu-id="5357b-131">String</span><span class="sxs-lookup"><span data-stu-id="5357b-131">String</span></span>| <span data-ttu-id="5357b-132">Anzeigename der Schule</span><span class="sxs-lookup"><span data-stu-id="5357b-132">Display name of the school</span></span>| 
|<span data-ttu-id="5357b-133">description</span><span class="sxs-lookup"><span data-stu-id="5357b-133">description</span></span>| <span data-ttu-id="5357b-134">String</span><span class="sxs-lookup"><span data-stu-id="5357b-134">String</span></span> | <span data-ttu-id="5357b-135">Beschreibung der Schule</span><span class="sxs-lookup"><span data-stu-id="5357b-135">Description of the school</span></span>| 
|<span data-ttu-id="5357b-136">principalEmail</span><span class="sxs-lookup"><span data-stu-id="5357b-136">principalEmail</span></span>| <span data-ttu-id="5357b-137">String</span><span class="sxs-lookup"><span data-stu-id="5357b-137">String</span></span>| <span data-ttu-id="5357b-138">Die E-Mail-Adresse des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="5357b-138">Email address of the principal</span></span>|
|<span data-ttu-id="5357b-139">principalName</span><span class="sxs-lookup"><span data-stu-id="5357b-139">principalName</span></span>| <span data-ttu-id="5357b-140">String</span><span class="sxs-lookup"><span data-stu-id="5357b-140">String</span></span> | <span data-ttu-id="5357b-141">Der Name des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="5357b-141">Name of the principal</span></span>|
|<span data-ttu-id="5357b-142">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="5357b-142">externalPrincipalId</span></span>| <span data-ttu-id="5357b-143">String</span><span class="sxs-lookup"><span data-stu-id="5357b-143">String</span></span> | <span data-ttu-id="5357b-144">Die ID des Prinzipals im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="5357b-144">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="5357b-145">highestGrade</span><span class="sxs-lookup"><span data-stu-id="5357b-145">highestGrade</span></span>|<span data-ttu-id="5357b-146">String</span><span class="sxs-lookup"><span data-stu-id="5357b-146">String</span></span>| <span data-ttu-id="5357b-147">Höchste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="5357b-147">Highest grade taught.</span></span> |
|<span data-ttu-id="5357b-148">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="5357b-148">lowestGrade</span></span>|<span data-ttu-id="5357b-149">String</span><span class="sxs-lookup"><span data-stu-id="5357b-149">String</span></span>| <span data-ttu-id="5357b-150">Niedrigste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="5357b-150">Lowest grade taught.</span></span> |
|<span data-ttu-id="5357b-151">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="5357b-151">schoolNumber</span></span>|<span data-ttu-id="5357b-152">String</span><span class="sxs-lookup"><span data-stu-id="5357b-152">String</span></span>| <span data-ttu-id="5357b-153">Schulnummer</span><span class="sxs-lookup"><span data-stu-id="5357b-153">School Number.</span></span>|
|<span data-ttu-id="5357b-154">externalId</span><span class="sxs-lookup"><span data-stu-id="5357b-154">externalId</span></span>|<span data-ttu-id="5357b-155">String</span><span class="sxs-lookup"><span data-stu-id="5357b-155">String</span></span>| <span data-ttu-id="5357b-156">Die ID der Schule im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="5357b-156">Id of school in syncing system.</span></span> |
|<span data-ttu-id="5357b-157">phone</span><span class="sxs-lookup"><span data-stu-id="5357b-157">phone</span></span>|<span data-ttu-id="5357b-158">String</span><span class="sxs-lookup"><span data-stu-id="5357b-158">String</span></span>| <span data-ttu-id="5357b-159">Die Telefonnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="5357b-159">Phone number of school.</span></span> |
|<span data-ttu-id="5357b-160">fax</span><span class="sxs-lookup"><span data-stu-id="5357b-160">fax</span></span>|<span data-ttu-id="5357b-161">String</span><span class="sxs-lookup"><span data-stu-id="5357b-161">String</span></span>| <span data-ttu-id="5357b-162">Die Faxnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="5357b-162">Fax number of school.</span></span> |
|<span data-ttu-id="5357b-163">address</span><span class="sxs-lookup"><span data-stu-id="5357b-163">address</span></span>|[<span data-ttu-id="5357b-164">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5357b-164">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="5357b-165">Die Adresse der Schule</span><span class="sxs-lookup"><span data-stu-id="5357b-165">Address of the School.</span></span>|
|<span data-ttu-id="5357b-166">createdBy</span><span class="sxs-lookup"><span data-stu-id="5357b-166">createdBy</span></span>|[<span data-ttu-id="5357b-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="5357b-167">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="5357b-168">Entität, die Schule erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="5357b-168">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="5357b-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="5357b-169">Response</span></span>
<span data-ttu-id="5357b-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [educationSchool](../resources/educationschool.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5357b-170">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5357b-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5357b-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5357b-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5357b-172">Request</span></span>
<span data-ttu-id="5357b-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5357b-173">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a><span data-ttu-id="5357b-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="5357b-174">Response</span></span>
<span data-ttu-id="5357b-175">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5357b-175">The following is an example of the response.</span></span> 

><span data-ttu-id="5357b-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5357b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
