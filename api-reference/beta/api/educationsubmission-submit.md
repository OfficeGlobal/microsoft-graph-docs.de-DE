---
title: 'EducationSubmission: Absenden'
description: Eine Aktion, die angibt, dass ein Schüler mit der Arbeit erfolgt und kann sofort in die Zuordnung zu verweisen. Diese Aktion kann nur durch die Student übernommen werden.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f67e5b07ed1093ee63e9b6fdf7647fa6891dacc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510771"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="571b8-104">EducationSubmission: Absenden</span><span class="sxs-lookup"><span data-stu-id="571b8-104">educationSubmission: submit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="571b8-105">Eine Aktion, die angibt, dass ein Schüler mit der Arbeit erfolgt und kann sofort in die Zuordnung zu verweisen.</span><span class="sxs-lookup"><span data-stu-id="571b8-105">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="571b8-106">Diese Aktion kann nur durch die Student übernommen werden.</span><span class="sxs-lookup"><span data-stu-id="571b8-106">This action can only be taken by the student.</span></span> <span data-ttu-id="571b8-107">Dadurch wird der Status der Übermittlung von "in Bearbeitung", "abgesendet" geändert.</span><span class="sxs-lookup"><span data-stu-id="571b8-107">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="571b8-108">Während des Aktivierungsvorgangs Submit werden alle Ressourcen in der SubmittedResources Bucket kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="571b8-108">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="571b8-109">Der Schulungsleiter wird die Ressourcenliste der übermittelten für Benotung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="571b8-109">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="571b8-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="571b8-110">Permissions</span></span>
<span data-ttu-id="571b8-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="571b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="571b8-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="571b8-113">Permission type</span></span>      | <span data-ttu-id="571b8-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="571b8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="571b8-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="571b8-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="571b8-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="571b8-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="571b8-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="571b8-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="571b8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="571b8-118">Not supported.</span></span>  |
|<span data-ttu-id="571b8-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="571b8-119">Application</span></span> | <span data-ttu-id="571b8-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="571b8-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="571b8-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="571b8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="571b8-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="571b8-122">Request headers</span></span>
| <span data-ttu-id="571b8-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="571b8-123">Header</span></span>       | <span data-ttu-id="571b8-124">Wert</span><span class="sxs-lookup"><span data-stu-id="571b8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="571b8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="571b8-125">Authorization</span></span>  | <span data-ttu-id="571b8-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="571b8-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="571b8-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="571b8-128">Request body</span></span>
<span data-ttu-id="571b8-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="571b8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="571b8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="571b8-130">Response</span></span>
<span data-ttu-id="571b8-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="571b8-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="571b8-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="571b8-133">Example</span></span>
<span data-ttu-id="571b8-134">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="571b8-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="571b8-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="571b8-135">Request</span></span>
<span data-ttu-id="571b8-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="571b8-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="571b8-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="571b8-137">Response</span></span>
<span data-ttu-id="571b8-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="571b8-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-submit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
