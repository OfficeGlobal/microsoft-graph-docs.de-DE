---
title: EducationUser-Eigenschaften aktualisieren
description: Aktualisieren der Eigenschaften eines **educationuser**-Objekts.
localization_priority: Normal
ms.openlocfilehash: aef8640f49ad6ff4d91755fd5200000f4a0e856d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856657"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="06163-103">EducationUser-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="06163-103">Update educationUser properties</span></span>

<span data-ttu-id="06163-104">Aktualisieren der Eigenschaften eines **educationuser**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="06163-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="06163-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06163-105">Permissions</span></span>
<span data-ttu-id="06163-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06163-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06163-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06163-108">Permission type</span></span>      | <span data-ttu-id="06163-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06163-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06163-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06163-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="06163-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06163-111">Not supported.</span></span>  |
|<span data-ttu-id="06163-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06163-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="06163-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06163-113">Not supported.</span></span>  |
|<span data-ttu-id="06163-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06163-114">Application</span></span> | <span data-ttu-id="06163-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06163-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06163-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06163-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="06163-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06163-117">Request headers</span></span>
| <span data-ttu-id="06163-118">Header</span><span class="sxs-lookup"><span data-stu-id="06163-118">Header</span></span>       | <span data-ttu-id="06163-119">Wert</span><span class="sxs-lookup"><span data-stu-id="06163-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="06163-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="06163-120">Authorization</span></span>  | <span data-ttu-id="06163-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06163-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="06163-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06163-123">Content-Type</span></span>  | <span data-ttu-id="06163-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06163-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06163-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06163-125">Request body</span></span>
<span data-ttu-id="06163-126">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="06163-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="06163-127">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="06163-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="06163-128">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="06163-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="06163-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06163-129">Property</span></span>     | <span data-ttu-id="06163-130">Typ</span><span class="sxs-lookup"><span data-stu-id="06163-130">Type</span></span>   |<span data-ttu-id="06163-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06163-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06163-132">displayName</span><span class="sxs-lookup"><span data-stu-id="06163-132">displayName</span></span>| <span data-ttu-id="06163-133">String</span><span class="sxs-lookup"><span data-stu-id="06163-133">String</span></span>| <span data-ttu-id="06163-134">Der Anzeigename des Benutzers</span><span class="sxs-lookup"><span data-stu-id="06163-134">Display Name of User</span></span>|
|<span data-ttu-id="06163-135">givenName</span><span class="sxs-lookup"><span data-stu-id="06163-135">givenName</span></span>| <span data-ttu-id="06163-136">String</span><span class="sxs-lookup"><span data-stu-id="06163-136">String</span></span> | <span data-ttu-id="06163-137">Vorname</span><span class="sxs-lookup"><span data-stu-id="06163-137">First Name</span></span> |
|<span data-ttu-id="06163-138">middleName</span><span class="sxs-lookup"><span data-stu-id="06163-138">middleName</span></span>| <span data-ttu-id="06163-139">String</span><span class="sxs-lookup"><span data-stu-id="06163-139">String</span></span> | <span data-ttu-id="06163-140">Zweiter Vorname des Benutzers</span><span class="sxs-lookup"><span data-stu-id="06163-140">Middle Name of user</span></span>|
|<span data-ttu-id="06163-141">surname</span><span class="sxs-lookup"><span data-stu-id="06163-141">surname</span></span>| <span data-ttu-id="06163-142">String</span><span class="sxs-lookup"><span data-stu-id="06163-142">String</span></span> | <span data-ttu-id="06163-143">Nachname des Benutzers</span><span class="sxs-lookup"><span data-stu-id="06163-143">Surname of user</span></span>|
|<span data-ttu-id="06163-144">mail</span><span class="sxs-lookup"><span data-stu-id="06163-144">mail</span></span>| <span data-ttu-id="06163-145">String</span><span class="sxs-lookup"><span data-stu-id="06163-145">String</span></span>| <span data-ttu-id="06163-146">E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="06163-146">email address</span></span>|
|<span data-ttu-id="06163-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="06163-147">mobilePhone</span></span>| <span data-ttu-id="06163-148">String</span><span class="sxs-lookup"><span data-stu-id="06163-148">String</span></span> | <span data-ttu-id="06163-149">Mobiltelefonnummer des Benutzers</span><span class="sxs-lookup"><span data-stu-id="06163-149">Mobile number of user</span></span> |
|<span data-ttu-id="06163-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="06163-150">externalSource</span></span>|<span data-ttu-id="06163-151">string</span><span class="sxs-lookup"><span data-stu-id="06163-151">string</span></span>| <span data-ttu-id="06163-152">Die möglichen Werte sind: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="06163-152">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="06163-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="06163-153">externalSource</span></span>|<span data-ttu-id="06163-154">string</span><span class="sxs-lookup"><span data-stu-id="06163-154">string</span></span>| <span data-ttu-id="06163-155">Quelle, aus der dieser Benutzer erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="06163-155">Where this user was created from.</span></span>  <span data-ttu-id="06163-156">Die möglichen Werte sind: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="06163-156">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="06163-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="06163-157">mailingAddress</span></span>|[<span data-ttu-id="06163-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="06163-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="06163-159">E-Mail-Adresse des Benutzers</span><span class="sxs-lookup"><span data-stu-id="06163-159">Mail address of user.</span></span>|
|<span data-ttu-id="06163-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="06163-160">residenceAddress</span></span>|[<span data-ttu-id="06163-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="06163-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="06163-162">Die Wohnadresse des Benutzers</span><span class="sxs-lookup"><span data-stu-id="06163-162">Address where user lives.</span></span>|
|<span data-ttu-id="06163-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="06163-163">primaryRole</span></span>|<span data-ttu-id="06163-164">string</span><span class="sxs-lookup"><span data-stu-id="06163-164">string</span></span>| <span data-ttu-id="06163-165">Standardrolle für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="06163-165">Default Role for a user.</span></span>  <span data-ttu-id="06163-166">Die Rolle des Benutzers kann in einer einzelnen Klasse unterschiedlich sein.</span><span class="sxs-lookup"><span data-stu-id="06163-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="06163-167">Die möglichen Werte sind: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="06163-167">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="06163-168">student</span><span class="sxs-lookup"><span data-stu-id="06163-168">student</span></span>|[<span data-ttu-id="06163-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="06163-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="06163-170">Ist die primäre Rolle Kursteilnehmer, enthält dieser Block spezifische Daten für Kursteilnehmer.</span><span class="sxs-lookup"><span data-stu-id="06163-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="06163-171">teacher</span><span class="sxs-lookup"><span data-stu-id="06163-171">teacher</span></span>|[<span data-ttu-id="06163-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="06163-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="06163-173">Ist die primäre Rolle Lehrer, enthält dieser Block lehrerspezifische Daten.</span><span class="sxs-lookup"><span data-stu-id="06163-173">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="06163-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="06163-174">Response</span></span>
<span data-ttu-id="06163-175">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06163-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06163-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06163-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06163-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06163-177">Request</span></span>
<span data-ttu-id="06163-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06163-178">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/{user-id}
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
##### <a name="response"></a><span data-ttu-id="06163-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="06163-179">Response</span></span>
<span data-ttu-id="06163-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06163-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "primaryRole": "student",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
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
