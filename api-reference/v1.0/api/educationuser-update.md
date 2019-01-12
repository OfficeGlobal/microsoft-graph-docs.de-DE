---
title: EducationUser-Eigenschaften aktualisieren
description: Aktualisieren der Eigenschaften eines **educationuser**-Objekts.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0c93ecd601e941cd68f0b6f8d668775e7de3feef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975960"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="e08d8-103">EducationUser-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e08d8-103">Update educationUser properties</span></span>

<span data-ttu-id="e08d8-104">Aktualisieren der Eigenschaften eines **educationuser**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e08d8-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e08d8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e08d8-105">Permissions</span></span>
<span data-ttu-id="e08d8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e08d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e08d8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e08d8-108">Permission type</span></span>      | <span data-ttu-id="e08d8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e08d8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e08d8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e08d8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e08d8-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e08d8-111">Not supported.</span></span>  |
|<span data-ttu-id="e08d8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e08d8-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e08d8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e08d8-113">Not supported.</span></span>  |
|<span data-ttu-id="e08d8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e08d8-114">Application</span></span> | <span data-ttu-id="e08d8-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e08d8-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e08d8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e08d8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e08d8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e08d8-117">Request headers</span></span>
| <span data-ttu-id="e08d8-118">Header</span><span class="sxs-lookup"><span data-stu-id="e08d8-118">Header</span></span>       | <span data-ttu-id="e08d8-119">Wert</span><span class="sxs-lookup"><span data-stu-id="e08d8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e08d8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e08d8-120">Authorization</span></span>  | <span data-ttu-id="e08d8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e08d8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e08d8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e08d8-123">Content-Type</span></span>  | <span data-ttu-id="e08d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e08d8-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e08d8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e08d8-125">Request body</span></span>
<span data-ttu-id="e08d8-126">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e08d8-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e08d8-127">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="e08d8-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e08d8-128">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="e08d8-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e08d8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e08d8-129">Property</span></span>     | <span data-ttu-id="e08d8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e08d8-130">Type</span></span>   |<span data-ttu-id="e08d8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e08d8-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e08d8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="e08d8-132">displayName</span></span>| <span data-ttu-id="e08d8-133">String</span><span class="sxs-lookup"><span data-stu-id="e08d8-133">String</span></span>| <span data-ttu-id="e08d8-134">Der Anzeigename des Benutzers</span><span class="sxs-lookup"><span data-stu-id="e08d8-134">Display Name of User</span></span>|
|<span data-ttu-id="e08d8-135">givenName</span><span class="sxs-lookup"><span data-stu-id="e08d8-135">givenName</span></span>| <span data-ttu-id="e08d8-136">String</span><span class="sxs-lookup"><span data-stu-id="e08d8-136">String</span></span> | <span data-ttu-id="e08d8-137">Vorname</span><span class="sxs-lookup"><span data-stu-id="e08d8-137">First Name</span></span> |
|<span data-ttu-id="e08d8-138">middleName</span><span class="sxs-lookup"><span data-stu-id="e08d8-138">middleName</span></span>| <span data-ttu-id="e08d8-139">String</span><span class="sxs-lookup"><span data-stu-id="e08d8-139">String</span></span> | <span data-ttu-id="e08d8-140">Zweiter Vorname des Benutzers</span><span class="sxs-lookup"><span data-stu-id="e08d8-140">Middle Name of user</span></span>|
|<span data-ttu-id="e08d8-141">surname</span><span class="sxs-lookup"><span data-stu-id="e08d8-141">surname</span></span>| <span data-ttu-id="e08d8-142">String</span><span class="sxs-lookup"><span data-stu-id="e08d8-142">String</span></span> | <span data-ttu-id="e08d8-143">Nachname des Benutzers</span><span class="sxs-lookup"><span data-stu-id="e08d8-143">Surname of user</span></span>|
|<span data-ttu-id="e08d8-144">mail</span><span class="sxs-lookup"><span data-stu-id="e08d8-144">mail</span></span>| <span data-ttu-id="e08d8-145">String</span><span class="sxs-lookup"><span data-stu-id="e08d8-145">String</span></span>| <span data-ttu-id="e08d8-146">E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="e08d8-146">email address</span></span>|
|<span data-ttu-id="e08d8-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="e08d8-147">mobilePhone</span></span>| <span data-ttu-id="e08d8-148">String</span><span class="sxs-lookup"><span data-stu-id="e08d8-148">String</span></span> | <span data-ttu-id="e08d8-149">Mobiltelefonnummer des Benutzers</span><span class="sxs-lookup"><span data-stu-id="e08d8-149">Mobile number of user</span></span> |
|<span data-ttu-id="e08d8-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="e08d8-150">externalSource</span></span>|<span data-ttu-id="e08d8-151">string</span><span class="sxs-lookup"><span data-stu-id="e08d8-151">string</span></span>| <span data-ttu-id="e08d8-152">Die möglichen Werte sind: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="e08d8-152">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="e08d8-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="e08d8-153">externalSource</span></span>|<span data-ttu-id="e08d8-154">string</span><span class="sxs-lookup"><span data-stu-id="e08d8-154">string</span></span>| <span data-ttu-id="e08d8-155">Quelle, aus der dieser Benutzer erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e08d8-155">Where this user was created from.</span></span>  <span data-ttu-id="e08d8-156">Die möglichen Werte sind: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="e08d8-156">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="e08d8-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="e08d8-157">mailingAddress</span></span>|[<span data-ttu-id="e08d8-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e08d8-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="e08d8-159">E-Mail-Adresse des Benutzers</span><span class="sxs-lookup"><span data-stu-id="e08d8-159">Mail address of user.</span></span>|
|<span data-ttu-id="e08d8-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="e08d8-160">residenceAddress</span></span>|[<span data-ttu-id="e08d8-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e08d8-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="e08d8-162">Die Wohnadresse des Benutzers</span><span class="sxs-lookup"><span data-stu-id="e08d8-162">Address where user lives.</span></span>|
|<span data-ttu-id="e08d8-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="e08d8-163">primaryRole</span></span>|<span data-ttu-id="e08d8-164">string</span><span class="sxs-lookup"><span data-stu-id="e08d8-164">string</span></span>| <span data-ttu-id="e08d8-165">Standardrolle für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="e08d8-165">Default Role for a user.</span></span>  <span data-ttu-id="e08d8-166">Die Rolle des Benutzers kann in einer einzelnen Klasse unterschiedlich sein.</span><span class="sxs-lookup"><span data-stu-id="e08d8-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="e08d8-167">Die möglichen Werte sind: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="e08d8-167">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="e08d8-168">student</span><span class="sxs-lookup"><span data-stu-id="e08d8-168">student</span></span>|[<span data-ttu-id="e08d8-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="e08d8-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="e08d8-170">Ist die primäre Rolle Kursteilnehmer, enthält dieser Block spezifische Daten für Kursteilnehmer.</span><span class="sxs-lookup"><span data-stu-id="e08d8-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="e08d8-171">teacher</span><span class="sxs-lookup"><span data-stu-id="e08d8-171">teacher</span></span>|[<span data-ttu-id="e08d8-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="e08d8-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="e08d8-173">Ist die primäre Rolle Lehrer, enthält dieser Block lehrerspezifische Daten.</span><span class="sxs-lookup"><span data-stu-id="e08d8-173">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="e08d8-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="e08d8-174">Response</span></span>
<span data-ttu-id="e08d8-175">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e08d8-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e08d8-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e08d8-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e08d8-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e08d8-177">Request</span></span>
<span data-ttu-id="e08d8-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e08d8-178">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e08d8-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="e08d8-179">Response</span></span>
<span data-ttu-id="e08d8-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e08d8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
