---
title: 'EducationSubmission: Rückruf'
description: 'Gibt an, dass ein Schüler möchte eine Übermittlung wieder übernehmen. Diese Aktion kann nur durch einen Schüler erfolgen. '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: a94d1c66764128d15c1017b664f9d4a6bd3f57fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828763"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="85afa-104">EducationSubmission: Rückruf</span><span class="sxs-lookup"><span data-stu-id="85afa-104">educationSubmission: recall</span></span>

> <span data-ttu-id="85afa-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85afa-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85afa-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85afa-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85afa-107">Gibt an, dass ein Schüler möchte eine Übermittlung wieder übernehmen.</span><span class="sxs-lookup"><span data-stu-id="85afa-107">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="85afa-108">Diese Aktion kann nur durch einen Schüler erfolgen.</span><span class="sxs-lookup"><span data-stu-id="85afa-108">This action can only be done by a student.</span></span> <span data-ttu-id="85afa-109">Es wird den Status der Übermittlung wieder in "in Bearbeitung" geändert, aus "abgesendet".</span><span class="sxs-lookup"><span data-stu-id="85afa-109">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="85afa-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="85afa-110">Permissions</span></span>
<span data-ttu-id="85afa-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85afa-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85afa-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85afa-113">Permission type</span></span>      | <span data-ttu-id="85afa-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85afa-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85afa-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85afa-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="85afa-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85afa-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="85afa-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85afa-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="85afa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85afa-118">Not supported</span></span>  |
|<span data-ttu-id="85afa-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85afa-119">Application</span></span> |<span data-ttu-id="85afa-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85afa-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="85afa-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85afa-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="85afa-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85afa-122">Request headers</span></span>
| <span data-ttu-id="85afa-123">Header</span><span class="sxs-lookup"><span data-stu-id="85afa-123">Header</span></span>       | <span data-ttu-id="85afa-124">Wert</span><span class="sxs-lookup"><span data-stu-id="85afa-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85afa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="85afa-125">Authorization</span></span>  | <span data-ttu-id="85afa-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="85afa-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85afa-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85afa-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="85afa-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="85afa-129">Response</span></span>
<span data-ttu-id="85afa-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85afa-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85afa-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85afa-132">Example</span></span>
<span data-ttu-id="85afa-133">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="85afa-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85afa-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85afa-134">Request</span></span>
<span data-ttu-id="85afa-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85afa-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="85afa-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="85afa-136">Response</span></span>
<span data-ttu-id="85afa-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="85afa-137">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
