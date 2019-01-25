---
title: 'EducationSubmission: Freigeben'
description: " und gibt an, dass die Benotung erfolgt. Diese Aktion kann nur durch die Lehrer erfolgen."
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fb8d9ce6646cb7055f2edb4cc56c7d9784d96915
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530174"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="dc600-104">EducationSubmission: Freigeben</span><span class="sxs-lookup"><span data-stu-id="dc600-104">educationSubmission: release</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc600-105">Diese Aktion können Sie die Qualität und Feedback dieser Übermittlung, die an die Student verfügbaren zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="dc600-105">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="dc600-106">Den Status der Übermittlung von "abgesendet" in "veröffentlicht" geändert, und gibt an, dass die Benotung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="dc600-106">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="dc600-107">Diese Aktion kann nur durch die Lehrer erfolgen.</span><span class="sxs-lookup"><span data-stu-id="dc600-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc600-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dc600-108">Permissions</span></span>
<span data-ttu-id="dc600-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc600-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc600-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dc600-111">Permission type</span></span>      | <span data-ttu-id="dc600-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dc600-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc600-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dc600-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="dc600-114">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc600-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="dc600-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dc600-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dc600-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc600-116">Not supported.</span></span>  |
|<span data-ttu-id="dc600-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dc600-117">Application</span></span> | <span data-ttu-id="dc600-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc600-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dc600-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc600-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="dc600-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dc600-120">Request headers</span></span>
| <span data-ttu-id="dc600-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dc600-121">Header</span></span>       | <span data-ttu-id="dc600-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dc600-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc600-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc600-123">Authorization</span></span>  | <span data-ttu-id="dc600-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dc600-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc600-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dc600-126">Request body</span></span>
<span data-ttu-id="dc600-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dc600-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc600-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc600-128">Response</span></span>
<span data-ttu-id="dc600-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc600-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc600-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dc600-131">Example</span></span>
<span data-ttu-id="dc600-132">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="dc600-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dc600-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc600-133">Request</span></span>
<span data-ttu-id="dc600-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dc600-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="dc600-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc600-135">Response</span></span>
<span data-ttu-id="dc600-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dc600-136">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-release.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
