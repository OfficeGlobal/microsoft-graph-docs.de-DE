---
title: 'EducationSubmission: zurückgeben'
description: Diese Aktion können Sie die Qualität und Feedback dieser Übermittlung, die an die Student verfügbaren zugeordnet.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b1772788230b5220b3bdc6813b122d1158e26ab2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511240"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="d2113-103">EducationSubmission: zurückgeben</span><span class="sxs-lookup"><span data-stu-id="d2113-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2113-104">Diese Aktion können Sie die Qualität und Feedback dieser Übermittlung, die an die Student verfügbaren zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="d2113-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="d2113-105">Den Status der Übermittlung von "abgesendet" in "zurückgegebene" geändert, und gibt an, dass Feedback bereitgestellt wird oder Benotung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="d2113-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="d2113-106">Diese Aktion kann nur durch die Lehrer erfolgen.</span><span class="sxs-lookup"><span data-stu-id="d2113-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2113-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d2113-107">Permissions</span></span>
<span data-ttu-id="d2113-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2113-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2113-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d2113-110">Permission type</span></span>      | <span data-ttu-id="d2113-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d2113-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2113-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d2113-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="d2113-113">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2113-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="d2113-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d2113-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d2113-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2113-115">Not supported.</span></span>  |
|<span data-ttu-id="d2113-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d2113-116">Application</span></span> | <span data-ttu-id="d2113-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2113-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d2113-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2113-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="d2113-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d2113-119">Request headers</span></span>
| <span data-ttu-id="d2113-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d2113-120">Header</span></span>       | <span data-ttu-id="d2113-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d2113-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2113-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2113-122">Authorization</span></span>  | <span data-ttu-id="d2113-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d2113-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2113-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d2113-125">Request body</span></span>
<span data-ttu-id="d2113-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d2113-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2113-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2113-127">Response</span></span>
<span data-ttu-id="d2113-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2113-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2113-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d2113-130">Example</span></span>
<span data-ttu-id="d2113-131">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="d2113-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2113-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2113-132">Request</span></span>
<span data-ttu-id="d2113-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d2113-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="d2113-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2113-134">Response</span></span>
<span data-ttu-id="d2113-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d2113-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
