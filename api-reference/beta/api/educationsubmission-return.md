---
title: 'EducationSubmission: zurückgeben'
description: Diese Aktion können Sie die Qualität und Feedback dieser Übermittlung, die an die Student verfügbaren zugeordnet.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 39e57044571b43df0515755035e23a38980376fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930649"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="eac8f-103">EducationSubmission: zurückgeben</span><span class="sxs-lookup"><span data-stu-id="eac8f-103">educationSubmission: return</span></span>

> <span data-ttu-id="eac8f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eac8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eac8f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eac8f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eac8f-106">Diese Aktion können Sie die Qualität und Feedback dieser Übermittlung, die an die Student verfügbaren zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="eac8f-106">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="eac8f-107">Den Status der Übermittlung von "abgesendet" in "zurückgegebene" geändert, und gibt an, dass Feedback bereitgestellt wird oder Benotung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="eac8f-107">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="eac8f-108">Diese Aktion kann nur durch die Lehrer erfolgen.</span><span class="sxs-lookup"><span data-stu-id="eac8f-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="eac8f-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eac8f-109">Permissions</span></span>
<span data-ttu-id="eac8f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eac8f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eac8f-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eac8f-112">Permission type</span></span>      | <span data-ttu-id="eac8f-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eac8f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eac8f-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eac8f-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="eac8f-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eac8f-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="eac8f-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eac8f-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="eac8f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eac8f-117">Not supported.</span></span>  |
|<span data-ttu-id="eac8f-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eac8f-118">Application</span></span> | <span data-ttu-id="eac8f-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eac8f-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="eac8f-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eac8f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="eac8f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eac8f-121">Request headers</span></span>
| <span data-ttu-id="eac8f-122">Header</span><span class="sxs-lookup"><span data-stu-id="eac8f-122">Header</span></span>       | <span data-ttu-id="eac8f-123">Wert</span><span class="sxs-lookup"><span data-stu-id="eac8f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eac8f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eac8f-124">Authorization</span></span>  | <span data-ttu-id="eac8f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eac8f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eac8f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eac8f-127">Request body</span></span>
<span data-ttu-id="eac8f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eac8f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eac8f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="eac8f-129">Response</span></span>
<span data-ttu-id="eac8f-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eac8f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eac8f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eac8f-132">Example</span></span>
<span data-ttu-id="eac8f-133">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="eac8f-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eac8f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eac8f-134">Request</span></span>
<span data-ttu-id="eac8f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eac8f-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="eac8f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="eac8f-136">Response</span></span>
<span data-ttu-id="eac8f-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eac8f-137">The following is an example of the response.</span></span>

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
