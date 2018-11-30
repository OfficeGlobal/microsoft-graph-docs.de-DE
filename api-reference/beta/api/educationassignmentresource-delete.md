---
title: EducationAssignmentResource löschen
description: .
ms.openlocfilehash: 9a9798170e8aab9d167a305a8815c26aec8eed13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059986"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="6086a-103">EducationAssignmentResource löschen</span><span class="sxs-lookup"><span data-stu-id="6086a-103">Delete educationAssignmentResource</span></span>

> <span data-ttu-id="6086a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6086a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6086a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6086a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6086a-106">Löschen Sie eine Ressource aus einer Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="6086a-106">Delete a resource from an assignment.</span></span> <span data-ttu-id="6086a-107">Nur Lehrer in der Klasse können keine Ressource entfernen.</span><span class="sxs-lookup"><span data-stu-id="6086a-107">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="6086a-108">Nachdem eine Zuordnung zum Studenten veröffentlicht wurde, können nicht Lehrer Ressourcen entfernen, die als "DistributeToStudents" markiert sind.</span><span class="sxs-lookup"><span data-stu-id="6086a-108">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="6086a-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6086a-109">Permissions</span></span>
<span data-ttu-id="6086a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6086a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6086a-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6086a-112">Permission type</span></span>      | <span data-ttu-id="6086a-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6086a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6086a-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6086a-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="6086a-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6086a-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="6086a-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6086a-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6086a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6086a-117">Not supported.</span></span>  |
|<span data-ttu-id="6086a-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6086a-118">Application</span></span> | <span data-ttu-id="6086a-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6086a-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6086a-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6086a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="6086a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6086a-121">Request headers</span></span>
| <span data-ttu-id="6086a-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6086a-122">Header</span></span>       | <span data-ttu-id="6086a-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6086a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6086a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6086a-124">Authorization</span></span>  | <span data-ttu-id="6086a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6086a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6086a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6086a-127">Request body</span></span>
<span data-ttu-id="6086a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6086a-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6086a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6086a-129">Response</span></span>
<span data-ttu-id="6086a-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6086a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6086a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6086a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6086a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6086a-133">Request</span></span>
<span data-ttu-id="6086a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6086a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="6086a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6086a-135">Response</span></span>
<span data-ttu-id="6086a-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6086a-136">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->