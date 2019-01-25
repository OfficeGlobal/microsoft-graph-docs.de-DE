---
title: 'EducationSubmission: Rückruf'
description: 'Gibt an, dass ein Schüler möchte eine Übermittlung wieder übernehmen. Diese Aktion kann nur durch einen Schüler erfolgen. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0be94d2888223ca31e37b71e490c4a9fdc28b7d0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520417"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="439c5-104">EducationSubmission: Rückruf</span><span class="sxs-lookup"><span data-stu-id="439c5-104">educationSubmission: recall</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="439c5-105">Gibt an, dass ein Schüler möchte eine Übermittlung wieder übernehmen.</span><span class="sxs-lookup"><span data-stu-id="439c5-105">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="439c5-106">Diese Aktion kann nur durch einen Schüler erfolgen.</span><span class="sxs-lookup"><span data-stu-id="439c5-106">This action can only be done by a student.</span></span> <span data-ttu-id="439c5-107">Es wird den Status der Übermittlung wieder in "in Bearbeitung" geändert, aus "abgesendet".</span><span class="sxs-lookup"><span data-stu-id="439c5-107">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="439c5-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="439c5-108">Permissions</span></span>
<span data-ttu-id="439c5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="439c5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="439c5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="439c5-111">Permission type</span></span>      | <span data-ttu-id="439c5-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="439c5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="439c5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="439c5-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="439c5-114">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="439c5-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="439c5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="439c5-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="439c5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="439c5-116">Not supported</span></span>  |
|<span data-ttu-id="439c5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="439c5-117">Application</span></span> |<span data-ttu-id="439c5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="439c5-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="439c5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="439c5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="439c5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="439c5-120">Request headers</span></span>
| <span data-ttu-id="439c5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="439c5-121">Header</span></span>       | <span data-ttu-id="439c5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="439c5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="439c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="439c5-123">Authorization</span></span>  | <span data-ttu-id="439c5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="439c5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="439c5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="439c5-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="439c5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="439c5-127">Response</span></span>
<span data-ttu-id="439c5-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="439c5-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="439c5-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="439c5-130">Example</span></span>
<span data-ttu-id="439c5-131">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="439c5-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="439c5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="439c5-132">Request</span></span>
<span data-ttu-id="439c5-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="439c5-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="439c5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="439c5-134">Response</span></span>
<span data-ttu-id="439c5-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="439c5-135">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-recall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
