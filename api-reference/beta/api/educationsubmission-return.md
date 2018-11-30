---
title: 'EducationSubmission: zurückgeben'
description: " und gibt an, dass Feedback bereitgestellt wird oder Benotung erfolgt. Diese Aktion kann nur durch die Lehrer erfolgen."
ms.openlocfilehash: de81f5429119556753462781f701fb7c936826b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058039"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="c088e-104">EducationSubmission: zurückgeben</span><span class="sxs-lookup"><span data-stu-id="c088e-104">educationSubmission: return</span></span>

> <span data-ttu-id="c088e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c088e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c088e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c088e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c088e-107">Diese Aktion können Sie die Qualität und Feedback dieser Übermittlung, die an die Student verfügbaren zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="c088e-107">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="c088e-108">Den Status der Übermittlung von "abgesendet" in "zurückgegebene" geändert, und gibt an, dass Feedback bereitgestellt wird oder Benotung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="c088e-108">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="c088e-109">Diese Aktion kann nur durch die Lehrer erfolgen.</span><span class="sxs-lookup"><span data-stu-id="c088e-109">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="c088e-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c088e-110">Permissions</span></span>
<span data-ttu-id="c088e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c088e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c088e-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c088e-113">Permission type</span></span>      | <span data-ttu-id="c088e-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c088e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c088e-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c088e-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="c088e-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c088e-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="c088e-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c088e-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c088e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c088e-118">Not supported.</span></span>  |
|<span data-ttu-id="c088e-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c088e-119">Application</span></span> | <span data-ttu-id="c088e-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c088e-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c088e-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c088e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="c088e-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c088e-122">Request headers</span></span>
| <span data-ttu-id="c088e-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c088e-123">Header</span></span>       | <span data-ttu-id="c088e-124">Wert</span><span class="sxs-lookup"><span data-stu-id="c088e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c088e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c088e-125">Authorization</span></span>  | <span data-ttu-id="c088e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c088e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c088e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c088e-128">Request body</span></span>
<span data-ttu-id="c088e-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c088e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c088e-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c088e-130">Response</span></span>
<span data-ttu-id="c088e-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c088e-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c088e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c088e-133">Example</span></span>
<span data-ttu-id="c088e-134">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="c088e-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c088e-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c088e-135">Request</span></span>
<span data-ttu-id="c088e-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c088e-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="c088e-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c088e-137">Response</span></span>
<span data-ttu-id="c088e-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c088e-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->