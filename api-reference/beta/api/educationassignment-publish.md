---
title: 'EducationAssignment: Veröffentlichen'
description: Diese Aktion, die den Status einer Zuordnung aus der ursprünglichen Entwurfsstatus in der veröffentlichten Status geändert wird. Nur in der Klasse Lehrer kann diese aufrufen. Eine Zuordnung im Status "Entwurf" ist, Studenten die Zuordnung werden nicht angezeigt, noch werden die Übermittlung Objekte vorhanden sein. Wenn Sie diese API aufrufen, Übermittlung Objekte erstellt werden, und die Zuordnung in der Student-Liste angezeigt wird.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: c7cdaebb91490270cc0a8f205b41a89b662a7a13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926701"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="91957-106">EducationAssignment: Veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="91957-106">educationAssignment: publish</span></span>

> <span data-ttu-id="91957-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91957-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91957-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91957-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91957-109">Diese Aktion, die den Status einer Zuordnung aus der ursprünglichen Entwurfsstatus in der veröffentlichten Status geändert wird.</span><span class="sxs-lookup"><span data-stu-id="91957-109">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="91957-110">Nur in der Klasse Lehrer kann diese aufrufen.</span><span class="sxs-lookup"><span data-stu-id="91957-110">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="91957-111">Eine Zuordnung im Status "Entwurf" ist, Studenten die Zuordnung werden nicht angezeigt, noch werden die Übermittlung Objekte vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="91957-111">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="91957-112">Wenn Sie diese API aufrufen, Übermittlung Objekte erstellt werden, und die Zuordnung in der Student-Liste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="91957-112">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="91957-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="91957-113">Permissions</span></span>
<span data-ttu-id="91957-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91957-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91957-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="91957-116">Permission type</span></span>      | <span data-ttu-id="91957-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="91957-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91957-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="91957-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="91957-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91957-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="91957-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="91957-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="91957-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91957-121">Not supported.</span></span>  |
|<span data-ttu-id="91957-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="91957-122">Application</span></span> | <span data-ttu-id="91957-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91957-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="91957-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="91957-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="91957-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="91957-125">Request headers</span></span>
| <span data-ttu-id="91957-126">Header</span><span class="sxs-lookup"><span data-stu-id="91957-126">Header</span></span>       | <span data-ttu-id="91957-127">Wert</span><span class="sxs-lookup"><span data-stu-id="91957-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91957-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="91957-128">Authorization</span></span>  | <span data-ttu-id="91957-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="91957-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91957-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="91957-131">Request body</span></span>
<span data-ttu-id="91957-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="91957-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91957-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="91957-133">Response</span></span>
<span data-ttu-id="91957-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="91957-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91957-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="91957-136">Example</span></span>
<span data-ttu-id="91957-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="91957-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="91957-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="91957-138">Request</span></span>
<span data-ttu-id="91957-139">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="91957-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="91957-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="91957-140">Response</span></span>
<span data-ttu-id="91957-141">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="91957-141">The following is an example of a response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
