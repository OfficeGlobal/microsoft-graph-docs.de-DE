---
title: EducationUser-Eigenschaften aktualisieren
description: Aktualisieren der Eigenschaften eines **educationuser**-Objekts.
ms.openlocfilehash: bd8d8f95cf1c8475a5c52946d0cf0d1eaa5240ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059928"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="404b6-103">EducationUser-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="404b6-103">Update educationUser properties</span></span>

> <span data-ttu-id="404b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="404b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="404b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="404b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="404b6-106">Aktualisieren der Eigenschaften eines **educationuser**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="404b6-106">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="404b6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="404b6-107">Permissions</span></span>
<span data-ttu-id="404b6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="404b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="404b6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="404b6-110">Permission type</span></span>      | <span data-ttu-id="404b6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="404b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="404b6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="404b6-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="404b6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="404b6-113">Not supported.</span></span>  |
|<span data-ttu-id="404b6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="404b6-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="404b6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="404b6-115">Not supported.</span></span>  |
|<span data-ttu-id="404b6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="404b6-116">Application</span></span> | <span data-ttu-id="404b6-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="404b6-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="404b6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="404b6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="404b6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="404b6-119">Request headers</span></span>
| <span data-ttu-id="404b6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="404b6-120">Header</span></span>       | <span data-ttu-id="404b6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="404b6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="404b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="404b6-122">Authorization</span></span>  | <span data-ttu-id="404b6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="404b6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="404b6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="404b6-125">Content-Type</span></span>  | <span data-ttu-id="404b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="404b6-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="404b6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="404b6-127">Request body</span></span>
<span data-ttu-id="404b6-128">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="404b6-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="404b6-129">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="404b6-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="404b6-130">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="404b6-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="404b6-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="404b6-131">Property</span></span>     | <span data-ttu-id="404b6-132">Typ</span><span class="sxs-lookup"><span data-stu-id="404b6-132">Type</span></span>   |<span data-ttu-id="404b6-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="404b6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="404b6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="404b6-134">displayName</span></span>| <span data-ttu-id="404b6-135">String</span><span class="sxs-lookup"><span data-stu-id="404b6-135">String</span></span>| <span data-ttu-id="404b6-136">Der Anzeigename des Benutzers</span><span class="sxs-lookup"><span data-stu-id="404b6-136">Display Name of User</span></span>|
|<span data-ttu-id="404b6-137">givenName</span><span class="sxs-lookup"><span data-stu-id="404b6-137">givenName</span></span>| <span data-ttu-id="404b6-138">String</span><span class="sxs-lookup"><span data-stu-id="404b6-138">String</span></span> | <span data-ttu-id="404b6-139">Vorname</span><span class="sxs-lookup"><span data-stu-id="404b6-139">First Name</span></span> |
|<span data-ttu-id="404b6-140">middleName</span><span class="sxs-lookup"><span data-stu-id="404b6-140">middleName</span></span>| <span data-ttu-id="404b6-141">String</span><span class="sxs-lookup"><span data-stu-id="404b6-141">String</span></span> | <span data-ttu-id="404b6-142">Zweiter Vorname des Benutzers</span><span class="sxs-lookup"><span data-stu-id="404b6-142">Middle Name of user</span></span>|
|<span data-ttu-id="404b6-143">surname</span><span class="sxs-lookup"><span data-stu-id="404b6-143">surname</span></span>| <span data-ttu-id="404b6-144">String</span><span class="sxs-lookup"><span data-stu-id="404b6-144">String</span></span> | <span data-ttu-id="404b6-145">Nachname des Benutzers</span><span class="sxs-lookup"><span data-stu-id="404b6-145">Surname of user</span></span>|
|<span data-ttu-id="404b6-146">mail</span><span class="sxs-lookup"><span data-stu-id="404b6-146">mail</span></span>| <span data-ttu-id="404b6-147">String</span><span class="sxs-lookup"><span data-stu-id="404b6-147">String</span></span>| <span data-ttu-id="404b6-148">E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="404b6-148">email address</span></span>|
|<span data-ttu-id="404b6-149">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="404b6-149">mobilePhone</span></span>| <span data-ttu-id="404b6-150">String</span><span class="sxs-lookup"><span data-stu-id="404b6-150">String</span></span> | <span data-ttu-id="404b6-151">Mobiltelefonnummer des Benutzers</span><span class="sxs-lookup"><span data-stu-id="404b6-151">Mobile number of user</span></span> |
|<span data-ttu-id="404b6-152">externalSource</span><span class="sxs-lookup"><span data-stu-id="404b6-152">externalSource</span></span>|<span data-ttu-id="404b6-153">string</span><span class="sxs-lookup"><span data-stu-id="404b6-153">string</span></span>| <span data-ttu-id="404b6-154">Mögliche Werte sind: `sis`, `manual` und `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="404b6-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="404b6-155">externalSource</span><span class="sxs-lookup"><span data-stu-id="404b6-155">externalSource</span></span>|<span data-ttu-id="404b6-156">string</span><span class="sxs-lookup"><span data-stu-id="404b6-156">string</span></span>| <span data-ttu-id="404b6-157">Quelle, aus der dieser Benutzer erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="404b6-157">Where this user was created from.</span></span>  <span data-ttu-id="404b6-158">Mögliche Werte sind: `sis`, `manual` und `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="404b6-158">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="404b6-159">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="404b6-159">mailingAddress</span></span>|[<span data-ttu-id="404b6-160">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="404b6-160">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="404b6-161">E-Mail-Adresse des Benutzers</span><span class="sxs-lookup"><span data-stu-id="404b6-161">Mail address of user.</span></span>|
|<span data-ttu-id="404b6-162">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="404b6-162">residenceAddress</span></span>|[<span data-ttu-id="404b6-163">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="404b6-163">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="404b6-164">Die Wohnadresse des Benutzers</span><span class="sxs-lookup"><span data-stu-id="404b6-164">Address where user lives.</span></span>|
|<span data-ttu-id="404b6-165">primaryRole</span><span class="sxs-lookup"><span data-stu-id="404b6-165">primaryRole</span></span>|<span data-ttu-id="404b6-166">string</span><span class="sxs-lookup"><span data-stu-id="404b6-166">string</span></span>| <span data-ttu-id="404b6-167">Standardrolle für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="404b6-167">Default Role for a user.</span></span>  <span data-ttu-id="404b6-168">Die Rolle des Benutzers kann in einer einzelnen Klasse unterschiedlich sein.</span><span class="sxs-lookup"><span data-stu-id="404b6-168">The user's role might be different in an individual class.</span></span> <span data-ttu-id="404b6-169">Mögliche Werte sind: `student`, `teacher` und `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="404b6-169">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="404b6-170">student</span><span class="sxs-lookup"><span data-stu-id="404b6-170">student</span></span>|[<span data-ttu-id="404b6-171">educationStudent</span><span class="sxs-lookup"><span data-stu-id="404b6-171">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="404b6-172">Ist die primäre Rolle Kursteilnehmer, enthält dieser Block spezifische Daten für Kursteilnehmer.</span><span class="sxs-lookup"><span data-stu-id="404b6-172">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="404b6-173">teacher</span><span class="sxs-lookup"><span data-stu-id="404b6-173">teacher</span></span>|[<span data-ttu-id="404b6-174">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="404b6-174">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="404b6-175">Ist die primäre Rolle Lehrer, enthält dieser Block lehrerspezifische Daten.</span><span class="sxs-lookup"><span data-stu-id="404b6-175">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="404b6-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="404b6-176">Response</span></span>
<span data-ttu-id="404b6-177">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="404b6-177">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="404b6-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="404b6-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="404b6-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="404b6-179">Request</span></span>
<span data-ttu-id="404b6-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="404b6-180">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/users/13020
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
##### <a name="response"></a><span data-ttu-id="404b6-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="404b6-181">Response</span></span>
<span data-ttu-id="404b6-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="404b6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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