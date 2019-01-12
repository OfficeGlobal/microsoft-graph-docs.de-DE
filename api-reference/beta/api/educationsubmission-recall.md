---
title: 'EducationSubmission: Rückruf'
description: 'Gibt an, dass ein Schüler möchte eine Übermittlung wieder übernehmen. Diese Aktion kann nur durch einen Schüler erfolgen. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9e9155244522d7f1f8c61263aff6de4c87faab4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984409"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="5b717-104">EducationSubmission: Rückruf</span><span class="sxs-lookup"><span data-stu-id="5b717-104">educationSubmission: recall</span></span>

> <span data-ttu-id="5b717-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b717-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b717-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b717-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b717-107">Gibt an, dass ein Schüler möchte eine Übermittlung wieder übernehmen.</span><span class="sxs-lookup"><span data-stu-id="5b717-107">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="5b717-108">Diese Aktion kann nur durch einen Schüler erfolgen.</span><span class="sxs-lookup"><span data-stu-id="5b717-108">This action can only be done by a student.</span></span> <span data-ttu-id="5b717-109">Es wird den Status der Übermittlung wieder in "in Bearbeitung" geändert, aus "abgesendet".</span><span class="sxs-lookup"><span data-stu-id="5b717-109">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="5b717-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b717-110">Permissions</span></span>
<span data-ttu-id="5b717-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b717-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b717-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b717-113">Permission type</span></span>      | <span data-ttu-id="5b717-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b717-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b717-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b717-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="5b717-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b717-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5b717-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b717-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5b717-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b717-118">Not supported</span></span>  |
|<span data-ttu-id="5b717-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b717-119">Application</span></span> |<span data-ttu-id="5b717-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b717-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="5b717-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b717-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="5b717-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b717-122">Request headers</span></span>
| <span data-ttu-id="5b717-123">Header</span><span class="sxs-lookup"><span data-stu-id="5b717-123">Header</span></span>       | <span data-ttu-id="5b717-124">Wert</span><span class="sxs-lookup"><span data-stu-id="5b717-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b717-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b717-125">Authorization</span></span>  | <span data-ttu-id="5b717-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b717-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b717-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b717-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5b717-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b717-129">Response</span></span>
<span data-ttu-id="5b717-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b717-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b717-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b717-132">Example</span></span>
<span data-ttu-id="5b717-133">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="5b717-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5b717-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b717-134">Request</span></span>
<span data-ttu-id="5b717-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b717-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="5b717-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b717-136">Response</span></span>
<span data-ttu-id="5b717-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b717-137">The following is an example of the response.</span></span>

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
