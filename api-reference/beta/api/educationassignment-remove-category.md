---
title: EducationCategory entfernen
description: Entfernen einer vorhandenen educationCategory aus diesem educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 9b8d3b2099173911f3ddbadf17a36ba17a4c9027
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30801003"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="fff97-103">EducationCategory entfernen</span><span class="sxs-lookup"><span data-stu-id="fff97-103">Remove educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fff97-104">Entfernen eines [educationCategory](../resources/educationcategory.md) aus einem [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fff97-104">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fff97-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fff97-105">Permissions</span></span>
<span data-ttu-id="fff97-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fff97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fff97-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fff97-108">Permission type</span></span>      | <span data-ttu-id="fff97-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fff97-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fff97-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fff97-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fff97-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fff97-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="fff97-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fff97-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fff97-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fff97-113">Not supported.</span></span>  |
|<span data-ttu-id="fff97-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fff97-114">Application</span></span> | <span data-ttu-id="fff97-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fff97-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fff97-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fff97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fff97-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fff97-117">Request headers</span></span>
| <span data-ttu-id="fff97-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fff97-118">Header</span></span>       | <span data-ttu-id="fff97-119">Wert</span><span class="sxs-lookup"><span data-stu-id="fff97-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fff97-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fff97-120">Authorization</span></span>  | <span data-ttu-id="fff97-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fff97-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fff97-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fff97-123">Content-Type</span></span>  | <span data-ttu-id="fff97-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fff97-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fff97-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fff97-125">Request body</span></span>
<span data-ttu-id="fff97-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fff97-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fff97-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fff97-127">Response</span></span>
<span data-ttu-id="fff97-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fff97-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fff97-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fff97-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fff97-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fff97-130">Request</span></span>
<span data-ttu-id="fff97-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fff97-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="fff97-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fff97-132">Response</span></span>
<span data-ttu-id="fff97-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fff97-133">The following is an example of the response.</span></span> 

><span data-ttu-id="fff97-134">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="fff97-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fff97-135">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fff97-135">All of the properties will be returned from an actual call.</span></span>


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
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-remove-category.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
