---
title: EducationClass entfernen
description: Löscht eine Klasse aus einer Schule.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 462ba0700a3070c5f01eb8ce9b507a6a3617c177
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529033"
---
# <a name="remove-educationclass"></a><span data-ttu-id="d7f07-103">EducationClass entfernen</span><span class="sxs-lookup"><span data-stu-id="d7f07-103">Remove educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7f07-104">Löscht eine Klasse aus einer Schule.</span><span class="sxs-lookup"><span data-stu-id="d7f07-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7f07-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7f07-105">Permissions</span></span>
<span data-ttu-id="d7f07-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7f07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7f07-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7f07-108">Permission type</span></span>      | <span data-ttu-id="d7f07-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7f07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7f07-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7f07-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d7f07-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7f07-111">Not supported.</span></span>  |
|<span data-ttu-id="d7f07-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7f07-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d7f07-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7f07-113">Not supported.</span></span>  |
|<span data-ttu-id="d7f07-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7f07-114">Application</span></span> | <span data-ttu-id="d7f07-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7f07-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d7f07-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7f07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d7f07-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7f07-117">Request headers</span></span>
| <span data-ttu-id="d7f07-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d7f07-118">Header</span></span>       | <span data-ttu-id="d7f07-119">Wert</span><span class="sxs-lookup"><span data-stu-id="d7f07-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d7f07-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7f07-120">Authorization</span></span>  | <span data-ttu-id="d7f07-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7f07-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7f07-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7f07-123">Request body</span></span>
<span data-ttu-id="d7f07-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d7f07-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d7f07-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7f07-125">Response</span></span>
<span data-ttu-id="d7f07-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7f07-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7f07-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7f07-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7f07-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7f07-128">Request</span></span>
<span data-ttu-id="d7f07-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7f07-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="d7f07-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7f07-130">Response</span></span>
<span data-ttu-id="d7f07-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d7f07-131">The following is an example of the response.</span></span> 

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
    "Error: /api-reference/beta/api/educationschool-delete-classes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
