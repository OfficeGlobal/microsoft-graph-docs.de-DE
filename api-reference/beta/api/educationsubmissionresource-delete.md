---
title: EducationSubmissionResource löschen
description: Löscht eine Ressource aus der Übermittlung an. Dies kann nur durch die Student erfolgen. Wenn die Ressource aus der Zuordnung kopiert wurde, wird eine neue Kopie der Ressource erstellt werden, nachdem die aktuelle Kopie gelöscht wurde.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a735cb1451e8d3eb8df13e6fa395c3e02393f451
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518982"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="0a1d6-105">EducationSubmissionResource löschen</span><span class="sxs-lookup"><span data-stu-id="0a1d6-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a1d6-106">Löscht eine Ressource aus der Übermittlung an.</span><span class="sxs-lookup"><span data-stu-id="0a1d6-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="0a1d6-107">Dies kann nur durch die Student erfolgen.</span><span class="sxs-lookup"><span data-stu-id="0a1d6-107">This can only be done by the student.</span></span> <span data-ttu-id="0a1d6-108">Wenn die Ressource aus der Zuordnung kopiert wurde, wird eine neue Kopie der Ressource erstellt werden, nachdem die aktuelle Kopie gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="0a1d6-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="0a1d6-109">Dadurch können Sie die Ressource in den ursprünglichen Zustand "Zurücksetzen".</span><span class="sxs-lookup"><span data-stu-id="0a1d6-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="0a1d6-110">Wenn die Ressource nicht in der Zuweisung kopiert wurde aber aus der Student hinzugefügt wurde, wird die Ressource einfach gelöscht.</span><span class="sxs-lookup"><span data-stu-id="0a1d6-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a1d6-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0a1d6-111">Permissions</span></span>
<span data-ttu-id="0a1d6-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a1d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a1d6-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a1d6-114">Permission type</span></span>      | <span data-ttu-id="0a1d6-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a1d6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a1d6-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a1d6-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="0a1d6-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a1d6-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="0a1d6-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a1d6-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0a1d6-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a1d6-119">Not supported.</span></span>  |
|<span data-ttu-id="0a1d6-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a1d6-120">Application</span></span> | <span data-ttu-id="0a1d6-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a1d6-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0a1d6-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a1d6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0a1d6-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a1d6-123">Request headers</span></span>
| <span data-ttu-id="0a1d6-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0a1d6-124">Header</span></span>       | <span data-ttu-id="0a1d6-125">Wert</span><span class="sxs-lookup"><span data-stu-id="0a1d6-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a1d6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a1d6-126">Authorization</span></span>  | <span data-ttu-id="0a1d6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0a1d6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a1d6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a1d6-129">Request body</span></span>
<span data-ttu-id="0a1d6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0a1d6-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0a1d6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a1d6-131">Response</span></span>
<span data-ttu-id="0a1d6-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a1d6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1d6-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a1d6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a1d6-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a1d6-135">Request</span></span>
<span data-ttu-id="0a1d6-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a1d6-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="0a1d6-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a1d6-137">Response</span></span>
<span data-ttu-id="0a1d6-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0a1d6-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
