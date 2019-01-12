---
title: Educationschool-Eigenschaften aktualisieren
description: Aktualisieren der Eigenschaften eines school-Objekts.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f44d6f8de1685c0c825be8781c1450baad5231e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975799"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="5a94a-103">Educationschool-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5a94a-103">Update educationschool properties</span></span>

> <span data-ttu-id="5a94a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5a94a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a94a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5a94a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a94a-106">Aktualisieren der Eigenschaften eines school-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a94a-106">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a94a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5a94a-107">Permissions</span></span>
<span data-ttu-id="5a94a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a94a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a94a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a94a-110">Permission type</span></span>      | <span data-ttu-id="5a94a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a94a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a94a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a94a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="5a94a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a94a-113">Not supported.</span></span>  |
|<span data-ttu-id="5a94a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a94a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5a94a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a94a-115">Not supported.</span></span>  |
|<span data-ttu-id="5a94a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a94a-116">Application</span></span> | <span data-ttu-id="5a94a-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a94a-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a94a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a94a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5a94a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a94a-119">Request headers</span></span>
| <span data-ttu-id="5a94a-120">Header</span><span class="sxs-lookup"><span data-stu-id="5a94a-120">Header</span></span>       | <span data-ttu-id="5a94a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5a94a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a94a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a94a-122">Authorization</span></span>  | <span data-ttu-id="5a94a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5a94a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5a94a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a94a-125">Content-Type</span></span>  | <span data-ttu-id="5a94a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a94a-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a94a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a94a-127">Request body</span></span>
<span data-ttu-id="5a94a-128">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5a94a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5a94a-129">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="5a94a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5a94a-130">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="5a94a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5a94a-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a94a-131">Property</span></span>     | <span data-ttu-id="5a94a-132">Typ</span><span class="sxs-lookup"><span data-stu-id="5a94a-132">Type</span></span>   |<span data-ttu-id="5a94a-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a94a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a94a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5a94a-134">displayName</span></span>| <span data-ttu-id="5a94a-135">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-135">String</span></span>| <span data-ttu-id="5a94a-136">Anzeigename der Schule</span><span class="sxs-lookup"><span data-stu-id="5a94a-136">Display name of the school</span></span>| 
|<span data-ttu-id="5a94a-137">description</span><span class="sxs-lookup"><span data-stu-id="5a94a-137">description</span></span>| <span data-ttu-id="5a94a-138">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-138">String</span></span> | <span data-ttu-id="5a94a-139">Beschreibung der Schule</span><span class="sxs-lookup"><span data-stu-id="5a94a-139">Description of the school</span></span>| 
|<span data-ttu-id="5a94a-140">principalEmail</span><span class="sxs-lookup"><span data-stu-id="5a94a-140">principalEmail</span></span>| <span data-ttu-id="5a94a-141">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-141">String</span></span>| <span data-ttu-id="5a94a-142">Die E-Mail-Adresse des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="5a94a-142">Email address of the principal</span></span>|
|<span data-ttu-id="5a94a-143">principalName</span><span class="sxs-lookup"><span data-stu-id="5a94a-143">principalName</span></span>| <span data-ttu-id="5a94a-144">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-144">String</span></span> | <span data-ttu-id="5a94a-145">Der Name des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="5a94a-145">Name of the principal</span></span>|
|<span data-ttu-id="5a94a-146">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="5a94a-146">externalPrincipalId</span></span>| <span data-ttu-id="5a94a-147">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-147">String</span></span> | <span data-ttu-id="5a94a-148">Die ID des Prinzipals im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="5a94a-148">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="5a94a-149">highestGrade</span><span class="sxs-lookup"><span data-stu-id="5a94a-149">highestGrade</span></span>|<span data-ttu-id="5a94a-150">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-150">String</span></span>| <span data-ttu-id="5a94a-151">Höchste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="5a94a-151">Highest grade taught.</span></span> |
|<span data-ttu-id="5a94a-152">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="5a94a-152">lowestGrade</span></span>|<span data-ttu-id="5a94a-153">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-153">String</span></span>| <span data-ttu-id="5a94a-154">Niedrigste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="5a94a-154">Lowest grade taught.</span></span> |
|<span data-ttu-id="5a94a-155">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="5a94a-155">schoolNumber</span></span>|<span data-ttu-id="5a94a-156">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-156">String</span></span>| <span data-ttu-id="5a94a-157">Schulnummer</span><span class="sxs-lookup"><span data-stu-id="5a94a-157">School Number.</span></span>|
|<span data-ttu-id="5a94a-158">externalId</span><span class="sxs-lookup"><span data-stu-id="5a94a-158">externalId</span></span>|<span data-ttu-id="5a94a-159">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-159">String</span></span>| <span data-ttu-id="5a94a-160">Die ID der Schule im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="5a94a-160">Id of school in syncing system.</span></span> |
|<span data-ttu-id="5a94a-161">phone</span><span class="sxs-lookup"><span data-stu-id="5a94a-161">phone</span></span>|<span data-ttu-id="5a94a-162">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-162">String</span></span>| <span data-ttu-id="5a94a-163">Die Telefonnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="5a94a-163">Phone number of school.</span></span> |
|<span data-ttu-id="5a94a-164">fax</span><span class="sxs-lookup"><span data-stu-id="5a94a-164">fax</span></span>|<span data-ttu-id="5a94a-165">String</span><span class="sxs-lookup"><span data-stu-id="5a94a-165">String</span></span>| <span data-ttu-id="5a94a-166">Die Faxnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="5a94a-166">Fax number of school.</span></span> |
|<span data-ttu-id="5a94a-167">address</span><span class="sxs-lookup"><span data-stu-id="5a94a-167">address</span></span>|[<span data-ttu-id="5a94a-168">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5a94a-168">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="5a94a-169">Die Adresse der Schule</span><span class="sxs-lookup"><span data-stu-id="5a94a-169">Address of the School.</span></span>|
|<span data-ttu-id="5a94a-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="5a94a-170">createdBy</span></span>|[<span data-ttu-id="5a94a-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="5a94a-171">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="5a94a-172">Entität, die Schule erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="5a94a-172">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="5a94a-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a94a-173">Response</span></span>
<span data-ttu-id="5a94a-174">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [educationSchool](../resources/educationschool.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a94a-174">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a94a-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a94a-175">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a94a-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a94a-176">Request</span></span>
<span data-ttu-id="5a94a-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a94a-177">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/schools/10002
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a><span data-ttu-id="5a94a-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a94a-178">Response</span></span>
<span data-ttu-id="5a94a-179">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5a94a-179">The following is an example of the response.</span></span> 

><span data-ttu-id="5a94a-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5a94a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
