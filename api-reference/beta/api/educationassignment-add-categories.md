---
title: EducationCategories hinzufügen
description: Hinzufügen eines vorhandenen educationCategory zu diesem educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d5fbf5d6db4ade6e44f65c256879c535d2e2a0e2
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800999"
---
# <a name="add-educationcategories"></a><span data-ttu-id="7cbd9-103">EducationCategories hinzufügen</span><span class="sxs-lookup"><span data-stu-id="7cbd9-103">Add educationCategories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cbd9-104">Fügen Sie diesem [educationAssignment](../resources/educationassignment.md)mindestens ein vorhandenes [EducationCategory](../resources/educationcategory.md) -Objekt hinzu.</span><span class="sxs-lookup"><span data-stu-id="7cbd9-104">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7cbd9-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7cbd9-105">Permissions</span></span>
<span data-ttu-id="7cbd9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cbd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cbd9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7cbd9-108">Permission type</span></span>      | <span data-ttu-id="7cbd9-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7cbd9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cbd9-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7cbd9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7cbd9-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7cbd9-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7cbd9-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7cbd9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7cbd9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7cbd9-113">Not supported.</span></span>  |
|<span data-ttu-id="7cbd9-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7cbd9-114">Application</span></span> | <span data-ttu-id="7cbd9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7cbd9-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="7cbd9-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cbd9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7cbd9-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7cbd9-117">Request headers</span></span>
| <span data-ttu-id="7cbd9-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7cbd9-118">Header</span></span>       | <span data-ttu-id="7cbd9-119">Wert</span><span class="sxs-lookup"><span data-stu-id="7cbd9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7cbd9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cbd9-120">Authorization</span></span>  | <span data-ttu-id="7cbd9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7cbd9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7cbd9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7cbd9-123">Content-Type</span></span>  | <span data-ttu-id="7cbd9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7cbd9-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7cbd9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7cbd9-125">Request body</span></span>
<span data-ttu-id="7cbd9-126">Geben Sie im Anforderungstext die odata.id der vorhandenen [educationCategory](../resources/educationcategory.md) -Objekte an, die dieser Zuordnung hinzugefügt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7cbd9-126">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="7cbd9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cbd9-127">Response</span></span>
<span data-ttu-id="7cbd9-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7cbd9-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7cbd9-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7cbd9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cbd9-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cbd9-130">Request</span></span>
<span data-ttu-id="7cbd9-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7cbd9-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/$ref
Content-type: application/json
Content-length: 212

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/classes/11021/assignmentCategories/ec98f158-341d-4fea-9f8c-14a250d489ac"
}

```
<span data-ttu-id="7cbd9-132">Geben Sie im Anforderungstext die odata.id des vorhandenen [educationCategory](../resources/educationcategory.md) -Objekts an, das dieser Zuordnung hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="7cbd9-132">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="7cbd9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cbd9-133">Response</span></span>
<span data-ttu-id="7cbd9-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7cbd9-134">The following is an example of the response.</span></span> 

><span data-ttu-id="7cbd9-135">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="7cbd9-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7cbd9-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7cbd9-136">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add educationCategory to educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-add-category.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
