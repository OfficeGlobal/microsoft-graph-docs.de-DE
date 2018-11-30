---
title: 'EducationSubmission: unsubmit'
description: . Während des Aktivierungsvorgangs Submit werden alle Ressourcen in der WorkingResources Bucket aus SubmittedResources kopiert werden. Die Liste der aktiven Ressourcen für die Benotung wird die Lehrer betrachten.
ms.openlocfilehash: 610b5a69a06c29d2e2b9b1fa6eb501a56d59b076
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059003"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="67be6-105">EducationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="67be6-105">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="67be6-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="67be6-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67be6-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67be6-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67be6-108">Eine Aktion, die angibt, dass auf der Übermittlung der Zuordnung arbeiten, nachdem sie, in aktiviert wurde ein Schüler möchte.</span><span class="sxs-lookup"><span data-stu-id="67be6-108">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="67be6-109">Diese Aktion kann nur durch die Student übernommen werden.</span><span class="sxs-lookup"><span data-stu-id="67be6-109">This action can only be taken by the student.</span></span> <span data-ttu-id="67be6-110">Dies wird den Status der Übermittlung die "Arbeit" aus "abgesendet" ändern.</span><span class="sxs-lookup"><span data-stu-id="67be6-110">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="67be6-111">Während des Aktivierungsvorgangs Submit werden alle Ressourcen in der WorkingResources Bucket aus SubmittedResources kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="67be6-111">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="67be6-112">Die Liste der aktiven Ressourcen für die Benotung wird die Lehrer betrachten.</span><span class="sxs-lookup"><span data-stu-id="67be6-112">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="67be6-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67be6-113">Permissions</span></span>
<span data-ttu-id="67be6-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67be6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67be6-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67be6-116">Permission type</span></span>      | <span data-ttu-id="67be6-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="67be6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67be6-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67be6-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="67be6-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67be6-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="67be6-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67be6-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="67be6-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67be6-121">Not supported.</span></span>  |
|<span data-ttu-id="67be6-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67be6-122">Application</span></span> | <span data-ttu-id="67be6-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67be6-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="67be6-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67be6-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="67be6-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67be6-125">Request headers</span></span>
| <span data-ttu-id="67be6-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="67be6-126">Header</span></span>       | <span data-ttu-id="67be6-127">Wert</span><span class="sxs-lookup"><span data-stu-id="67be6-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67be6-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="67be6-128">Authorization</span></span>  | <span data-ttu-id="67be6-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67be6-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67be6-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67be6-131">Request body</span></span>
<span data-ttu-id="67be6-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="67be6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67be6-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="67be6-133">Response</span></span>
<span data-ttu-id="67be6-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67be6-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67be6-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67be6-136">Example</span></span>
<span data-ttu-id="67be6-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="67be6-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="67be6-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67be6-138">Request</span></span>
<span data-ttu-id="67be6-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67be6-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="67be6-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="67be6-140">Response</span></span>
<span data-ttu-id="67be6-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="67be6-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
