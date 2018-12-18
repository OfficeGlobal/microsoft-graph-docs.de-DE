---
title: 'EducationSubmission: zurückgeben'
description: Diese Aktion können Sie die Qualität und Feedback dieser Übermittlung, die an die Student verfügbaren zugeordnet.
author: dipakboyed
ms.openlocfilehash: d73300328168baf9481b329b36f056aa27044b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350876"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="b1fa5-103">EducationSubmission: zurückgeben</span><span class="sxs-lookup"><span data-stu-id="b1fa5-103">educationSubmission: return</span></span>

> <span data-ttu-id="b1fa5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1fa5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1fa5-106">Diese Aktion können Sie die Qualität und Feedback dieser Übermittlung, die an die Student verfügbaren zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-106">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="b1fa5-107">Den Status der Übermittlung von "abgesendet" in "zurückgegebene" geändert, und gibt an, dass Feedback bereitgestellt wird oder Benotung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-107">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="b1fa5-108">Diese Aktion kann nur durch die Lehrer erfolgen.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1fa5-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b1fa5-109">Permissions</span></span>
<span data-ttu-id="b1fa5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1fa5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1fa5-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1fa5-112">Permission type</span></span>      | <span data-ttu-id="b1fa5-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1fa5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1fa5-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1fa5-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="b1fa5-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1fa5-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="b1fa5-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1fa5-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b1fa5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1fa5-117">Not supported.</span></span>  |
|<span data-ttu-id="b1fa5-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1fa5-118">Application</span></span> | <span data-ttu-id="b1fa5-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1fa5-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b1fa5-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1fa5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="b1fa5-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1fa5-121">Request headers</span></span>
| <span data-ttu-id="b1fa5-122">Header</span><span class="sxs-lookup"><span data-stu-id="b1fa5-122">Header</span></span>       | <span data-ttu-id="b1fa5-123">Wert</span><span class="sxs-lookup"><span data-stu-id="b1fa5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1fa5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1fa5-124">Authorization</span></span>  | <span data-ttu-id="b1fa5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1fa5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1fa5-127">Request body</span></span>
<span data-ttu-id="b1fa5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1fa5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1fa5-129">Response</span></span>
<span data-ttu-id="b1fa5-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1fa5-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1fa5-132">Example</span></span>
<span data-ttu-id="b1fa5-133">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b1fa5-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1fa5-134">Request</span></span>
<span data-ttu-id="b1fa5-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="b1fa5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1fa5-136">Response</span></span>
<span data-ttu-id="b1fa5-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b1fa5-137">The following is an example of the response.</span></span>

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