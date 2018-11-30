---
title: EducationSubmissionResource löschen
description: " die Ressource in den ursprünglichen Zustand. Wenn die Ressource nicht in der Zuweisung kopiert wurde aber aus der Student hinzugefügt wurde, wird die Ressource einfach gelöscht."
ms.openlocfilehash: 9eb5b08e2e5481e707cc6c1e0b0f8339e3d22ad4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063097"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="18324-104">EducationSubmissionResource löschen</span><span class="sxs-lookup"><span data-stu-id="18324-104">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="18324-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="18324-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18324-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18324-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18324-107">Löscht eine Ressource aus der Übermittlung an.</span><span class="sxs-lookup"><span data-stu-id="18324-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="18324-108">Dies kann nur durch die Student erfolgen.</span><span class="sxs-lookup"><span data-stu-id="18324-108">This can only be done by the student.</span></span> <span data-ttu-id="18324-109">Wenn die Ressource aus der Zuordnung kopiert wurde, wird eine neue Kopie der Ressource erstellt werden, nachdem die aktuelle Kopie gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="18324-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="18324-110">Dadurch können Sie die Ressource in den ursprünglichen Zustand "Zurücksetzen".</span><span class="sxs-lookup"><span data-stu-id="18324-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="18324-111">Wenn die Ressource nicht in der Zuweisung kopiert wurde aber aus der Student hinzugefügt wurde, wird die Ressource einfach gelöscht.</span><span class="sxs-lookup"><span data-stu-id="18324-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="18324-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18324-112">Permissions</span></span>
<span data-ttu-id="18324-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18324-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18324-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18324-115">Permission type</span></span>      | <span data-ttu-id="18324-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18324-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18324-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18324-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="18324-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18324-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="18324-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18324-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="18324-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18324-120">Not supported.</span></span>  |
|<span data-ttu-id="18324-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18324-121">Application</span></span> | <span data-ttu-id="18324-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18324-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="18324-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18324-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="18324-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18324-124">Request headers</span></span>
| <span data-ttu-id="18324-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="18324-125">Header</span></span>       | <span data-ttu-id="18324-126">Wert</span><span class="sxs-lookup"><span data-stu-id="18324-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18324-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="18324-127">Authorization</span></span>  | <span data-ttu-id="18324-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18324-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18324-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18324-130">Request body</span></span>
<span data-ttu-id="18324-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="18324-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="18324-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="18324-132">Response</span></span>
<span data-ttu-id="18324-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18324-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18324-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18324-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18324-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18324-136">Request</span></span>
<span data-ttu-id="18324-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18324-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="18324-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="18324-138">Response</span></span>
<span data-ttu-id="18324-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18324-139">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->