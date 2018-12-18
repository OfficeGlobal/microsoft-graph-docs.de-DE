---
title: EducationSubmissionResource löschen
description: Löscht eine Ressource aus der Übermittlung an. Dies kann nur durch die Student erfolgen. Wenn die Ressource aus der Zuordnung kopiert wurde, wird eine neue Kopie der Ressource erstellt werden, nachdem die aktuelle Kopie gelöscht wurde.
author: dipakboyed
ms.openlocfilehash: d56df6cee3884556186554d9c24ae09ed802c4f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313272"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="c8429-105">EducationSubmissionResource löschen</span><span class="sxs-lookup"><span data-stu-id="c8429-105">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="c8429-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c8429-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8429-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8429-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8429-108">Löscht eine Ressource aus der Übermittlung an.</span><span class="sxs-lookup"><span data-stu-id="c8429-108">Deletes a resource from the submission.</span></span> <span data-ttu-id="c8429-109">Dies kann nur durch die Student erfolgen.</span><span class="sxs-lookup"><span data-stu-id="c8429-109">This can only be done by the student.</span></span> <span data-ttu-id="c8429-110">Wenn die Ressource aus der Zuordnung kopiert wurde, wird eine neue Kopie der Ressource erstellt werden, nachdem die aktuelle Kopie gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="c8429-110">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="c8429-111">Dadurch können Sie die Ressource in den ursprünglichen Zustand "Zurücksetzen".</span><span class="sxs-lookup"><span data-stu-id="c8429-111">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="c8429-112">Wenn die Ressource nicht in der Zuweisung kopiert wurde aber aus der Student hinzugefügt wurde, wird die Ressource einfach gelöscht.</span><span class="sxs-lookup"><span data-stu-id="c8429-112">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8429-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8429-113">Permissions</span></span>
<span data-ttu-id="c8429-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8429-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8429-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8429-116">Permission type</span></span>      | <span data-ttu-id="c8429-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8429-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8429-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8429-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="c8429-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8429-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c8429-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8429-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c8429-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8429-121">Not supported.</span></span>  |
|<span data-ttu-id="c8429-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8429-122">Application</span></span> | <span data-ttu-id="c8429-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8429-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c8429-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8429-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c8429-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8429-125">Request headers</span></span>
| <span data-ttu-id="c8429-126">Header</span><span class="sxs-lookup"><span data-stu-id="c8429-126">Header</span></span>       | <span data-ttu-id="c8429-127">Wert</span><span class="sxs-lookup"><span data-stu-id="c8429-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8429-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8429-128">Authorization</span></span>  | <span data-ttu-id="c8429-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8429-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8429-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8429-131">Request body</span></span>
<span data-ttu-id="c8429-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c8429-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c8429-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8429-133">Response</span></span>
<span data-ttu-id="c8429-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8429-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8429-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8429-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8429-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8429-137">Request</span></span>
<span data-ttu-id="c8429-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8429-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="c8429-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8429-139">Response</span></span>
<span data-ttu-id="c8429-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8429-140">The following is an example of the response.</span></span> 

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