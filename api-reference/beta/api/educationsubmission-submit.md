---
title: 'EducationSubmission: Absenden'
description: Eine Aktion, die angibt, dass ein Schüler mit der Arbeit erfolgt und kann sofort in die Zuordnung zu verweisen. Diese Aktion kann nur durch die Student übernommen werden.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: ef2ef84819a6bfbeeb83a012b4c26fe7cb56662c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808575"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="60e45-104">EducationSubmission: Absenden</span><span class="sxs-lookup"><span data-stu-id="60e45-104">educationSubmission: submit</span></span>

> <span data-ttu-id="60e45-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="60e45-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60e45-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60e45-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60e45-107">Eine Aktion, die angibt, dass ein Schüler mit der Arbeit erfolgt und kann sofort in die Zuordnung zu verweisen.</span><span class="sxs-lookup"><span data-stu-id="60e45-107">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="60e45-108">Diese Aktion kann nur durch die Student übernommen werden.</span><span class="sxs-lookup"><span data-stu-id="60e45-108">This action can only be taken by the student.</span></span> <span data-ttu-id="60e45-109">Dadurch wird der Status der Übermittlung von "in Bearbeitung", "abgesendet" geändert.</span><span class="sxs-lookup"><span data-stu-id="60e45-109">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="60e45-110">Während des Aktivierungsvorgangs Submit werden alle Ressourcen in der SubmittedResources Bucket kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="60e45-110">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="60e45-111">Der Schulungsleiter wird die Ressourcenliste der übermittelten für Benotung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="60e45-111">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="60e45-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="60e45-112">Permissions</span></span>
<span data-ttu-id="60e45-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60e45-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60e45-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60e45-115">Permission type</span></span>      | <span data-ttu-id="60e45-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60e45-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60e45-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60e45-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="60e45-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60e45-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="60e45-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60e45-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="60e45-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60e45-120">Not supported.</span></span>  |
|<span data-ttu-id="60e45-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60e45-121">Application</span></span> | <span data-ttu-id="60e45-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60e45-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="60e45-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60e45-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="60e45-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60e45-124">Request headers</span></span>
| <span data-ttu-id="60e45-125">Header</span><span class="sxs-lookup"><span data-stu-id="60e45-125">Header</span></span>       | <span data-ttu-id="60e45-126">Wert</span><span class="sxs-lookup"><span data-stu-id="60e45-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="60e45-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="60e45-127">Authorization</span></span>  | <span data-ttu-id="60e45-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60e45-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60e45-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60e45-130">Request body</span></span>
<span data-ttu-id="60e45-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="60e45-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60e45-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="60e45-132">Response</span></span>
<span data-ttu-id="60e45-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60e45-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60e45-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60e45-135">Example</span></span>
<span data-ttu-id="60e45-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="60e45-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="60e45-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60e45-137">Request</span></span>
<span data-ttu-id="60e45-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="60e45-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="60e45-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="60e45-139">Response</span></span>
<span data-ttu-id="60e45-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="60e45-140">The following is an example of the response.</span></span>

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
