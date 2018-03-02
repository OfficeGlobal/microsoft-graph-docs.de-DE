# <a name="update-educationuser-properties"></a><span data-ttu-id="9418b-101">EducationUser-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9418b-101">Update educationUser properties</span></span>

<span data-ttu-id="9418b-102">Aktualisieren der Eigenschaften eines **educationuser**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9418b-102">Update the properties of an **eventMessage** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9418b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9418b-103">Permissions</span></span>
<span data-ttu-id="9418b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9418b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9418b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9418b-106">Permission type</span></span>      | <span data-ttu-id="9418b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9418b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9418b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9418b-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="9418b-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9418b-109">Not supported.</span></span>  |
|<span data-ttu-id="9418b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9418b-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9418b-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9418b-111">Not supported.</span></span>  |
|<span data-ttu-id="9418b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9418b-112">Application</span></span> | <span data-ttu-id="9418b-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9418b-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9418b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9418b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9418b-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9418b-115">Request headers</span></span>
| <span data-ttu-id="9418b-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9418b-116">Header</span></span>       | <span data-ttu-id="9418b-117">Wert</span><span class="sxs-lookup"><span data-stu-id="9418b-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9418b-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="9418b-118">Authorization</span></span>  | <span data-ttu-id="9418b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9418b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9418b-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9418b-121">Content-Type</span></span>  | <span data-ttu-id="9418b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9418b-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9418b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9418b-123">Request body</span></span>
<span data-ttu-id="9418b-124">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9418b-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9418b-125">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="9418b-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9418b-126">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="9418b-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9418b-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9418b-127">Property</span></span>     | <span data-ttu-id="9418b-128">Typ</span><span class="sxs-lookup"><span data-stu-id="9418b-128">Type</span></span>   |<span data-ttu-id="9418b-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9418b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9418b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="9418b-130">displayName</span></span>| <span data-ttu-id="9418b-131">String</span><span class="sxs-lookup"><span data-stu-id="9418b-131">String</span></span>| <span data-ttu-id="9418b-132">Der Anzeigename des Benutzers</span><span class="sxs-lookup"><span data-stu-id="9418b-132">Display Name of User</span></span>|
|<span data-ttu-id="9418b-133">givenName</span><span class="sxs-lookup"><span data-stu-id="9418b-133">givenName</span></span>| <span data-ttu-id="9418b-134">String</span><span class="sxs-lookup"><span data-stu-id="9418b-134">String</span></span> | <span data-ttu-id="9418b-135">Vorname</span><span class="sxs-lookup"><span data-stu-id="9418b-135">First Name</span></span> |
|<span data-ttu-id="9418b-136">middleName</span><span class="sxs-lookup"><span data-stu-id="9418b-136">middleName</span></span>| <span data-ttu-id="9418b-137">String</span><span class="sxs-lookup"><span data-stu-id="9418b-137">String</span></span> | <span data-ttu-id="9418b-138">Zweiter Vorname des Benutzers</span><span class="sxs-lookup"><span data-stu-id="9418b-138">Middle Name of user</span></span>|
|<span data-ttu-id="9418b-139">surname</span><span class="sxs-lookup"><span data-stu-id="9418b-139">surname</span></span>| <span data-ttu-id="9418b-140">String</span><span class="sxs-lookup"><span data-stu-id="9418b-140">String</span></span> | <span data-ttu-id="9418b-141">Nachname des Benutzers</span><span class="sxs-lookup"><span data-stu-id="9418b-141">Surname of user</span></span>|
|<span data-ttu-id="9418b-142">mail</span><span class="sxs-lookup"><span data-stu-id="9418b-142">mail</span></span>| <span data-ttu-id="9418b-143">String</span><span class="sxs-lookup"><span data-stu-id="9418b-143">String</span></span>| <span data-ttu-id="9418b-144">E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="9418b-144">Email Address</span></span>|
|<span data-ttu-id="9418b-145">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="9418b-145">mobilePhone</span></span>| <span data-ttu-id="9418b-146">String</span><span class="sxs-lookup"><span data-stu-id="9418b-146">String</span></span> | <span data-ttu-id="9418b-147">Mobiltelefonnummer des Benutzers</span><span class="sxs-lookup"><span data-stu-id="9418b-147">Mobile number of user</span></span> |
|<span data-ttu-id="9418b-148">externalSource</span><span class="sxs-lookup"><span data-stu-id="9418b-148">externalSource</span></span>|<span data-ttu-id="9418b-149">string</span><span class="sxs-lookup"><span data-stu-id="9418b-149">string</span></span>| <span data-ttu-id="9418b-150">Mögliche Werte sind: `sis`, `manual` und `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="9418b-150">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="9418b-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="9418b-151">externalSource</span></span>|<span data-ttu-id="9418b-152">string</span><span class="sxs-lookup"><span data-stu-id="9418b-152">string</span></span>| <span data-ttu-id="9418b-153">Quelle, aus der dieser Benutzer erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="9418b-153">Where this user was created from.</span></span>  <span data-ttu-id="9418b-154">Mögliche Werte sind: `sis`, `manual` und `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="9418b-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="9418b-155">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="9418b-155">MailingAddress</span></span>|[<span data-ttu-id="9418b-156">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9418b-156">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="9418b-157">E-Mail-Adresse des Benutzers</span><span class="sxs-lookup"><span data-stu-id="9418b-157">Mail address of user.</span></span>|
|<span data-ttu-id="9418b-158">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="9418b-158">residenceAddress</span></span>|[<span data-ttu-id="9418b-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9418b-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="9418b-160">Die Wohnadresse des Benutzers</span><span class="sxs-lookup"><span data-stu-id="9418b-160">Address where user lives.</span></span>|
|<span data-ttu-id="9418b-161">primaryRole</span><span class="sxs-lookup"><span data-stu-id="9418b-161">primaryRole</span></span>|<span data-ttu-id="9418b-162">string</span><span class="sxs-lookup"><span data-stu-id="9418b-162">string</span></span>| <span data-ttu-id="9418b-163">Standardrolle für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="9418b-163">Default Role for a user.</span></span>  <span data-ttu-id="9418b-164">Die Rolle des Benutzers kann in einer einzelnen Klasse unterschiedlich sein.</span><span class="sxs-lookup"><span data-stu-id="9418b-164">The user's role might be different in an individual class.</span></span> <span data-ttu-id="9418b-165">Mögliche Werte sind: `student`, `teacher` und `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="9418b-165">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="9418b-166">student</span><span class="sxs-lookup"><span data-stu-id="9418b-166">student</span></span>|[<span data-ttu-id="9418b-167">educationStudent</span><span class="sxs-lookup"><span data-stu-id="9418b-167">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="9418b-168">Ist die primäre Rolle Kursteilnehmer, enthält dieser Block spezifische Daten für Kursteilnehmer.</span><span class="sxs-lookup"><span data-stu-id="9418b-168">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="9418b-169">teacher</span><span class="sxs-lookup"><span data-stu-id="9418b-169">teacher</span></span>|[<span data-ttu-id="9418b-170">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="9418b-170">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="9418b-171">Ist die primäre Rolle Lehrer, enthält dieser Block lehrerspezifische Daten.</span><span class="sxs-lookup"><span data-stu-id="9418b-171">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="9418b-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="9418b-172">Response</span></span>
<span data-ttu-id="9418b-173">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9418b-173">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9418b-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9418b-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9418b-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9418b-175">Request</span></span>
<span data-ttu-id="9418b-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9418b-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/13020
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
##### <a name="response"></a><span data-ttu-id="9418b-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="9418b-177">Response</span></span>
<span data-ttu-id="9418b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9418b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "string",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->