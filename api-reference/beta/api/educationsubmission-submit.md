---
title: 'EducationSubmission: Absenden'
description: . Während des Aktivierungsvorgangs Submit werden alle Ressourcen in der SubmittedResources Bucket kopiert werden. Der Schulungsleiter wird die Ressourcenliste der übermittelten für Benotung angezeigt.
ms.openlocfilehash: 566948278ffacb1169842c49aa11c78cba0a5f3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059900"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="f906e-105">EducationSubmission: Absenden</span><span class="sxs-lookup"><span data-stu-id="f906e-105">educationSubmission: submit</span></span>

> <span data-ttu-id="f906e-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f906e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f906e-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f906e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f906e-108">Eine Aktion, die angibt, dass ein Schüler mit der Arbeit erfolgt und kann sofort in die Zuordnung zu verweisen.</span><span class="sxs-lookup"><span data-stu-id="f906e-108">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="f906e-109">Diese Aktion kann nur durch die Student übernommen werden.</span><span class="sxs-lookup"><span data-stu-id="f906e-109">This action can only be taken by the student.</span></span> <span data-ttu-id="f906e-110">Dadurch wird der Status der Übermittlung von "in Bearbeitung", "abgesendet" geändert.</span><span class="sxs-lookup"><span data-stu-id="f906e-110">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="f906e-111">Während des Aktivierungsvorgangs Submit werden alle Ressourcen in der SubmittedResources Bucket kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="f906e-111">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="f906e-112">Der Schulungsleiter wird die Ressourcenliste der übermittelten für Benotung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f906e-112">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="f906e-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f906e-113">Permissions</span></span>
<span data-ttu-id="f906e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f906e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f906e-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f906e-116">Permission type</span></span>      | <span data-ttu-id="f906e-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f906e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f906e-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f906e-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="f906e-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f906e-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f906e-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f906e-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f906e-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f906e-121">Not supported.</span></span>  |
|<span data-ttu-id="f906e-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f906e-122">Application</span></span> | <span data-ttu-id="f906e-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f906e-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f906e-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f906e-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="f906e-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f906e-125">Request headers</span></span>
| <span data-ttu-id="f906e-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f906e-126">Header</span></span>       | <span data-ttu-id="f906e-127">Wert</span><span class="sxs-lookup"><span data-stu-id="f906e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f906e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f906e-128">Authorization</span></span>  | <span data-ttu-id="f906e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f906e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f906e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f906e-131">Request body</span></span>
<span data-ttu-id="f906e-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f906e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f906e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f906e-133">Response</span></span>
<span data-ttu-id="f906e-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f906e-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f906e-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f906e-136">Example</span></span>
<span data-ttu-id="f906e-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="f906e-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f906e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f906e-138">Request</span></span>
<span data-ttu-id="f906e-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f906e-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="f906e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="f906e-140">Response</span></span>
<span data-ttu-id="f906e-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f906e-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->