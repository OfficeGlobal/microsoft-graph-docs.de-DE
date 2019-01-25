---
title: 'EducationAssignment: Veröffentlichen'
description: Diese Aktion, die den Status einer Zuordnung aus der ursprünglichen Entwurfsstatus in der veröffentlichten Status geändert wird. Nur in der Klasse Lehrer kann diese aufrufen. Eine Zuordnung im Status "Entwurf" ist, Studenten die Zuordnung werden nicht angezeigt, noch werden die Übermittlung Objekte vorhanden sein. Wenn Sie diese API aufrufen, Übermittlung Objekte erstellt werden, und die Zuordnung in der Student-Liste angezeigt wird.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: bac9c38d5fbd2ce80693a468c0a2d229085f32cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508713"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="f93d2-106">EducationAssignment: Veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="f93d2-106">educationAssignment: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f93d2-107">Diese Aktion, die den Status einer Zuordnung aus der ursprünglichen Entwurfsstatus in der veröffentlichten Status geändert wird.</span><span class="sxs-lookup"><span data-stu-id="f93d2-107">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="f93d2-108">Nur in der Klasse Lehrer kann diese aufrufen.</span><span class="sxs-lookup"><span data-stu-id="f93d2-108">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="f93d2-109">Eine Zuordnung im Status "Entwurf" ist, Studenten die Zuordnung werden nicht angezeigt, noch werden die Übermittlung Objekte vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="f93d2-109">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="f93d2-110">Wenn Sie diese API aufrufen, Übermittlung Objekte erstellt werden, und die Zuordnung in der Student-Liste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f93d2-110">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="f93d2-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f93d2-111">Permissions</span></span>
<span data-ttu-id="f93d2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f93d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f93d2-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f93d2-114">Permission type</span></span>      | <span data-ttu-id="f93d2-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f93d2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f93d2-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f93d2-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="f93d2-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f93d2-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f93d2-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f93d2-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f93d2-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f93d2-119">Not supported.</span></span>  |
|<span data-ttu-id="f93d2-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f93d2-120">Application</span></span> | <span data-ttu-id="f93d2-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f93d2-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f93d2-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f93d2-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="f93d2-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f93d2-123">Request headers</span></span>
| <span data-ttu-id="f93d2-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f93d2-124">Header</span></span>       | <span data-ttu-id="f93d2-125">Wert</span><span class="sxs-lookup"><span data-stu-id="f93d2-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f93d2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f93d2-126">Authorization</span></span>  | <span data-ttu-id="f93d2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f93d2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f93d2-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f93d2-129">Request body</span></span>
<span data-ttu-id="f93d2-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f93d2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f93d2-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f93d2-131">Response</span></span>
<span data-ttu-id="f93d2-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f93d2-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f93d2-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f93d2-134">Example</span></span>
<span data-ttu-id="f93d2-135">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="f93d2-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f93d2-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f93d2-136">Request</span></span>
<span data-ttu-id="f93d2-137">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f93d2-137">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="f93d2-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f93d2-138">Response</span></span>
<span data-ttu-id="f93d2-139">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="f93d2-139">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
