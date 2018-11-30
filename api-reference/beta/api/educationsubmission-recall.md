---
title: 'EducationSubmission: Rückruf'
description: .
ms.openlocfilehash: 8df134a6d8325e5b497baada89bc0fa16d0ee9e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058993"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="30944-103">EducationSubmission: Rückruf</span><span class="sxs-lookup"><span data-stu-id="30944-103">educationSubmission: recall</span></span>

> <span data-ttu-id="30944-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="30944-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30944-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="30944-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30944-106">Gibt an, dass ein Schüler möchte eine Übermittlung wieder übernehmen.</span><span class="sxs-lookup"><span data-stu-id="30944-106">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="30944-107">Diese Aktion kann nur durch einen Schüler erfolgen.</span><span class="sxs-lookup"><span data-stu-id="30944-107">This action can only be done by a student.</span></span> <span data-ttu-id="30944-108">Es wird den Status der Übermittlung wieder in "in Bearbeitung" geändert, aus "abgesendet".</span><span class="sxs-lookup"><span data-stu-id="30944-108">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="30944-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="30944-109">Permissions</span></span>
<span data-ttu-id="30944-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30944-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30944-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30944-112">Permission type</span></span>      | <span data-ttu-id="30944-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30944-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30944-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30944-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="30944-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30944-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="30944-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30944-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="30944-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30944-117">Not supported</span></span>  |
|<span data-ttu-id="30944-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30944-118">Application</span></span> |<span data-ttu-id="30944-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30944-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="30944-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30944-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="30944-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30944-121">Request headers</span></span>
| <span data-ttu-id="30944-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="30944-122">Header</span></span>       | <span data-ttu-id="30944-123">Wert</span><span class="sxs-lookup"><span data-stu-id="30944-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="30944-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="30944-124">Authorization</span></span>  | <span data-ttu-id="30944-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="30944-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30944-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="30944-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="30944-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="30944-128">Response</span></span>
<span data-ttu-id="30944-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30944-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30944-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30944-131">Example</span></span>
<span data-ttu-id="30944-132">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="30944-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="30944-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30944-133">Request</span></span>
<span data-ttu-id="30944-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="30944-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="30944-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="30944-135">Response</span></span>
<span data-ttu-id="30944-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="30944-136">The following is an example of the response.</span></span>

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