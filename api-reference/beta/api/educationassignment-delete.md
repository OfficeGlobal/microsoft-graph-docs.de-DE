---
title: EducationAssignment löschen
description: Löschen Sie eine vorhandene Zuordnung. Nur Lehrer innerhalb einer Klasse können Arbeitsaufträge löschen.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2356330a75558ea88b94c9266fb2d4a387e87b59
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515888"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="5a769-104">EducationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="5a769-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a769-105">Löschen Sie eine vorhandene Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="5a769-105">Delete an existing assignment.</span></span> <span data-ttu-id="5a769-106">Nur Lehrer innerhalb einer Klasse können Arbeitsaufträge löschen.</span><span class="sxs-lookup"><span data-stu-id="5a769-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a769-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5a769-107">Permissions</span></span>
<span data-ttu-id="5a769-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a769-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a769-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a769-110">Permission type</span></span>      | <span data-ttu-id="5a769-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a769-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a769-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a769-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5a769-113">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a769-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="5a769-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a769-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="5a769-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a769-115">Not Supported.</span></span> |
|<span data-ttu-id="5a769-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a769-116">Application</span></span> | <span data-ttu-id="5a769-117">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5a769-117">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="5a769-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a769-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="5a769-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a769-119">Request headers</span></span>
| <span data-ttu-id="5a769-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5a769-120">Header</span></span>       | <span data-ttu-id="5a769-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5a769-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a769-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a769-122">Authorization</span></span>  | <span data-ttu-id="5a769-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5a769-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a769-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a769-125">Request body</span></span>
<span data-ttu-id="5a769-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5a769-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5a769-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a769-127">Response</span></span>
<span data-ttu-id="5a769-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a769-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a769-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a769-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a769-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a769-131">Request</span></span>
<span data-ttu-id="5a769-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a769-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="5a769-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a769-133">Response</span></span>
<span data-ttu-id="5a769-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5a769-134">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
