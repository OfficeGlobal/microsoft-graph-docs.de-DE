---
title: Lehrer entfernen
description: Entfernen eines Lehrers von einer Klasse.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bf6860e515d1b8e1fa52b633b88740e62c6992e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507467"
---
# <a name="remove-teacher"></a><span data-ttu-id="f2e65-103">Lehrer entfernen</span><span class="sxs-lookup"><span data-stu-id="f2e65-103">Remove teacher</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2e65-104">Entfernen eines Lehrers von einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="f2e65-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2e65-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f2e65-105">Permissions</span></span>
<span data-ttu-id="f2e65-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2e65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2e65-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2e65-108">Permission type</span></span>      | <span data-ttu-id="f2e65-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2e65-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2e65-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2e65-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f2e65-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2e65-111">Not supported.</span></span>  |
|<span data-ttu-id="f2e65-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2e65-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f2e65-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2e65-113">Not supported.</span></span>  |
|<span data-ttu-id="f2e65-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2e65-114">Application</span></span> | <span data-ttu-id="f2e65-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e65-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f2e65-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2e65-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f2e65-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2e65-117">Request headers</span></span>
| <span data-ttu-id="f2e65-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f2e65-118">Header</span></span>       | <span data-ttu-id="f2e65-119">Wert</span><span class="sxs-lookup"><span data-stu-id="f2e65-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2e65-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2e65-120">Authorization</span></span>  | <span data-ttu-id="f2e65-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2e65-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f2e65-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2e65-123">Request body</span></span>
<span data-ttu-id="f2e65-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f2e65-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f2e65-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2e65-125">Response</span></span>
<span data-ttu-id="f2e65-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein leerer Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2e65-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2e65-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2e65-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2e65-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2e65-128">Request</span></span>
<span data-ttu-id="f2e65-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2e65-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/<id>/teachers/14012
```

##### <a name="response"></a><span data-ttu-id="f2e65-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2e65-130">Response</span></span>
<span data-ttu-id="f2e65-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f2e65-131">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-delete-teachers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
