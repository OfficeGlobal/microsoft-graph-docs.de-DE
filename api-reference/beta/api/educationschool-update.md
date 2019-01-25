---
title: Educationschool-Eigenschaften aktualisieren
description: Aktualisieren der Eigenschaften eines school-Objekts.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c7dd9cafe1238170599e802738d42bd287ebf47f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523645"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="170ea-103">Educationschool-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="170ea-103">Update educationschool properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="170ea-104">Aktualisieren der Eigenschaften eines school-Objekts.</span><span class="sxs-lookup"><span data-stu-id="170ea-104">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="170ea-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="170ea-105">Permissions</span></span>
<span data-ttu-id="170ea-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="170ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="170ea-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="170ea-108">Permission type</span></span>      | <span data-ttu-id="170ea-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="170ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="170ea-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="170ea-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="170ea-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="170ea-111">Not supported.</span></span>  |
|<span data-ttu-id="170ea-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="170ea-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="170ea-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="170ea-113">Not supported.</span></span>  |
|<span data-ttu-id="170ea-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="170ea-114">Application</span></span> | <span data-ttu-id="170ea-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170ea-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="170ea-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="170ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="170ea-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="170ea-117">Request headers</span></span>
| <span data-ttu-id="170ea-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="170ea-118">Header</span></span>       | <span data-ttu-id="170ea-119">Wert</span><span class="sxs-lookup"><span data-stu-id="170ea-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="170ea-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="170ea-120">Authorization</span></span>  | <span data-ttu-id="170ea-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="170ea-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="170ea-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="170ea-123">Content-Type</span></span>  | <span data-ttu-id="170ea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="170ea-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="170ea-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="170ea-125">Request body</span></span>
<span data-ttu-id="170ea-126">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="170ea-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="170ea-127">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="170ea-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="170ea-128">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="170ea-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="170ea-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="170ea-129">Property</span></span>     | <span data-ttu-id="170ea-130">Typ</span><span class="sxs-lookup"><span data-stu-id="170ea-130">Type</span></span>   |<span data-ttu-id="170ea-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="170ea-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="170ea-132">displayName</span><span class="sxs-lookup"><span data-stu-id="170ea-132">displayName</span></span>| <span data-ttu-id="170ea-133">String</span><span class="sxs-lookup"><span data-stu-id="170ea-133">String</span></span>| <span data-ttu-id="170ea-134">Anzeigename der Schule</span><span class="sxs-lookup"><span data-stu-id="170ea-134">Display name of the school</span></span>| 
|<span data-ttu-id="170ea-135">description</span><span class="sxs-lookup"><span data-stu-id="170ea-135">description</span></span>| <span data-ttu-id="170ea-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="170ea-136">String</span></span> | <span data-ttu-id="170ea-137">Beschreibung der Schule</span><span class="sxs-lookup"><span data-stu-id="170ea-137">Description of the school</span></span>| 
|<span data-ttu-id="170ea-138">principalEmail</span><span class="sxs-lookup"><span data-stu-id="170ea-138">principalEmail</span></span>| <span data-ttu-id="170ea-139">String</span><span class="sxs-lookup"><span data-stu-id="170ea-139">String</span></span>| <span data-ttu-id="170ea-140">Die E-Mail-Adresse des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="170ea-140">Email address of the principal</span></span>|
|<span data-ttu-id="170ea-141">principalName</span><span class="sxs-lookup"><span data-stu-id="170ea-141">principalName</span></span>| <span data-ttu-id="170ea-142">String</span><span class="sxs-lookup"><span data-stu-id="170ea-142">String</span></span> | <span data-ttu-id="170ea-143">Der Name des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="170ea-143">Name of the principal</span></span>|
|<span data-ttu-id="170ea-144">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="170ea-144">externalPrincipalId</span></span>| <span data-ttu-id="170ea-145">String</span><span class="sxs-lookup"><span data-stu-id="170ea-145">String</span></span> | <span data-ttu-id="170ea-146">Die ID des Prinzipals im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="170ea-146">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="170ea-147">highestGrade</span><span class="sxs-lookup"><span data-stu-id="170ea-147">highestGrade</span></span>|<span data-ttu-id="170ea-148">String</span><span class="sxs-lookup"><span data-stu-id="170ea-148">String</span></span>| <span data-ttu-id="170ea-149">Höchste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="170ea-149">Highest grade taught.</span></span> |
|<span data-ttu-id="170ea-150">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="170ea-150">lowestGrade</span></span>|<span data-ttu-id="170ea-151">String</span><span class="sxs-lookup"><span data-stu-id="170ea-151">String</span></span>| <span data-ttu-id="170ea-152">Niedrigste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="170ea-152">Lowest grade taught.</span></span> |
|<span data-ttu-id="170ea-153">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="170ea-153">schoolNumber</span></span>|<span data-ttu-id="170ea-154">String</span><span class="sxs-lookup"><span data-stu-id="170ea-154">String</span></span>| <span data-ttu-id="170ea-155">Schulnummer</span><span class="sxs-lookup"><span data-stu-id="170ea-155">School Number.</span></span>|
|<span data-ttu-id="170ea-156">externalId</span><span class="sxs-lookup"><span data-stu-id="170ea-156">externalId</span></span>|<span data-ttu-id="170ea-157">String</span><span class="sxs-lookup"><span data-stu-id="170ea-157">String</span></span>| <span data-ttu-id="170ea-158">Die ID der Schule im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="170ea-158">Id of school in syncing system.</span></span> |
|<span data-ttu-id="170ea-159">phone</span><span class="sxs-lookup"><span data-stu-id="170ea-159">phone</span></span>|<span data-ttu-id="170ea-160">String</span><span class="sxs-lookup"><span data-stu-id="170ea-160">String</span></span>| <span data-ttu-id="170ea-161">Die Telefonnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="170ea-161">Phone number of school.</span></span> |
|<span data-ttu-id="170ea-162">fax</span><span class="sxs-lookup"><span data-stu-id="170ea-162">fax</span></span>|<span data-ttu-id="170ea-163">String</span><span class="sxs-lookup"><span data-stu-id="170ea-163">String</span></span>| <span data-ttu-id="170ea-164">Die Faxnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="170ea-164">Fax number of school.</span></span> |
|<span data-ttu-id="170ea-165">address</span><span class="sxs-lookup"><span data-stu-id="170ea-165">address</span></span>|[<span data-ttu-id="170ea-166">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="170ea-166">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="170ea-167">Die Adresse der Schule</span><span class="sxs-lookup"><span data-stu-id="170ea-167">Address of the School.</span></span>|
|<span data-ttu-id="170ea-168">createdBy</span><span class="sxs-lookup"><span data-stu-id="170ea-168">createdBy</span></span>|[<span data-ttu-id="170ea-169">identitySet</span><span class="sxs-lookup"><span data-stu-id="170ea-169">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="170ea-170">Entität, die Schule erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="170ea-170">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="170ea-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="170ea-171">Response</span></span>
<span data-ttu-id="170ea-172">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [educationSchool](../resources/educationschool.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="170ea-172">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="170ea-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="170ea-173">Example</span></span>
##### <a name="request"></a><span data-ttu-id="170ea-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="170ea-174">Request</span></span>
<span data-ttu-id="170ea-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="170ea-175">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="170ea-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="170ea-176">Response</span></span>
<span data-ttu-id="170ea-177">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="170ea-177">The following is an example of the response.</span></span> 

><span data-ttu-id="170ea-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="170ea-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
