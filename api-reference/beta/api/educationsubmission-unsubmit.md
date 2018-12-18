---
title: 'EducationSubmission: unsubmit'
description: 'Eine Aktion, die angibt, dass auf der Übermittlung der Zuordnung arbeiten, nachdem sie, in aktiviert wurde ein Schüler möchte. Diese Aktion kann nur durch die Student übernommen werden. '
author: dipakboyed
ms.openlocfilehash: a61f2e9c05691266ae9248ca95700f173e0ee0b0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304228"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="517cf-104">EducationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="517cf-104">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="517cf-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="517cf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="517cf-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="517cf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="517cf-107">Eine Aktion, die angibt, dass auf der Übermittlung der Zuordnung arbeiten, nachdem sie, in aktiviert wurde ein Schüler möchte.</span><span class="sxs-lookup"><span data-stu-id="517cf-107">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="517cf-108">Diese Aktion kann nur durch die Student übernommen werden.</span><span class="sxs-lookup"><span data-stu-id="517cf-108">This action can only be taken by the student.</span></span> <span data-ttu-id="517cf-109">Dies wird den Status der Übermittlung die "Arbeit" aus "abgesendet" ändern.</span><span class="sxs-lookup"><span data-stu-id="517cf-109">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="517cf-110">Während des Aktivierungsvorgangs Submit werden alle Ressourcen in der WorkingResources Bucket aus SubmittedResources kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="517cf-110">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="517cf-111">Die Liste der aktiven Ressourcen für die Benotung wird die Lehrer betrachten.</span><span class="sxs-lookup"><span data-stu-id="517cf-111">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="517cf-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="517cf-112">Permissions</span></span>
<span data-ttu-id="517cf-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="517cf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="517cf-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="517cf-115">Permission type</span></span>      | <span data-ttu-id="517cf-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="517cf-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="517cf-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="517cf-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="517cf-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="517cf-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="517cf-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="517cf-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="517cf-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="517cf-120">Not supported.</span></span>  |
|<span data-ttu-id="517cf-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="517cf-121">Application</span></span> | <span data-ttu-id="517cf-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="517cf-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="517cf-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="517cf-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="517cf-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="517cf-124">Request headers</span></span>
| <span data-ttu-id="517cf-125">Header</span><span class="sxs-lookup"><span data-stu-id="517cf-125">Header</span></span>       | <span data-ttu-id="517cf-126">Wert</span><span class="sxs-lookup"><span data-stu-id="517cf-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="517cf-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="517cf-127">Authorization</span></span>  | <span data-ttu-id="517cf-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="517cf-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="517cf-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="517cf-130">Request body</span></span>
<span data-ttu-id="517cf-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="517cf-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="517cf-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="517cf-132">Response</span></span>
<span data-ttu-id="517cf-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="517cf-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="517cf-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="517cf-135">Example</span></span>
<span data-ttu-id="517cf-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="517cf-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="517cf-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="517cf-137">Request</span></span>
<span data-ttu-id="517cf-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="517cf-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="517cf-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="517cf-139">Response</span></span>
<span data-ttu-id="517cf-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="517cf-140">The following is an example of the response.</span></span>

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
