---
title: EducationCategory löschen
description: Löscht eine vorhandene Kategorie.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3c68f4a9950437ddcebc0cd40237bef07c597648
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800998"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="8b88a-103">EducationCategory löschen</span><span class="sxs-lookup"><span data-stu-id="8b88a-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b88a-104">Löscht eine vorhandene Kategorie.</span><span class="sxs-lookup"><span data-stu-id="8b88a-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b88a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b88a-105">Permissions</span></span>
<span data-ttu-id="8b88a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b88a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b88a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b88a-108">Permission type</span></span>      | <span data-ttu-id="8b88a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b88a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b88a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b88a-110">Delegated (work or school account)</span></span>| <span data-ttu-id="8b88a-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b88a-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="8b88a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b88a-112">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="8b88a-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8b88a-113">Not Supported.</span></span> |
|<span data-ttu-id="8b88a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b88a-114">Application</span></span> | <span data-ttu-id="8b88a-115">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8b88a-115">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="8b88a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b88a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignmentCategories/<id>
```
## <a name="request-headers"></a><span data-ttu-id="8b88a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b88a-117">Request headers</span></span>
| <span data-ttu-id="8b88a-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8b88a-118">Header</span></span>       | <span data-ttu-id="8b88a-119">Wert</span><span class="sxs-lookup"><span data-stu-id="8b88a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b88a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b88a-120">Authorization</span></span>  | <span data-ttu-id="8b88a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b88a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b88a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b88a-123">Request body</span></span>
<span data-ttu-id="8b88a-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8b88a-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8b88a-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b88a-125">Response</span></span>
<span data-ttu-id="8b88a-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b88a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b88a-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b88a-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b88a-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b88a-129">Request</span></span>
<span data-ttu-id="8b88a-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b88a-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
### <a name="response"></a><span data-ttu-id="8b88a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b88a-131">Response</span></span>
<span data-ttu-id="8b88a-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b88a-132">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationcategory-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
