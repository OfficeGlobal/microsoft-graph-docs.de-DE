---
title: EducationClass entfernen
description: Löscht eine Klasse aus einer Schule.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1ae6e96358f0ea6c85feb8cfec50a68ba1a7ee4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934975"
---
# <a name="remove-educationclass"></a><span data-ttu-id="493bf-103">EducationClass entfernen</span><span class="sxs-lookup"><span data-stu-id="493bf-103">Remove educationClass</span></span>

> <span data-ttu-id="493bf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="493bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="493bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="493bf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="493bf-106">Löscht eine Klasse aus einer Schule.</span><span class="sxs-lookup"><span data-stu-id="493bf-106">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="493bf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="493bf-107">Permissions</span></span>
<span data-ttu-id="493bf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="493bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="493bf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="493bf-110">Permission type</span></span>      | <span data-ttu-id="493bf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="493bf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="493bf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="493bf-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="493bf-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="493bf-113">Not supported.</span></span>  |
|<span data-ttu-id="493bf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="493bf-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="493bf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="493bf-115">Not supported.</span></span>  |
|<span data-ttu-id="493bf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="493bf-116">Application</span></span> | <span data-ttu-id="493bf-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="493bf-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="493bf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="493bf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="493bf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="493bf-119">Request headers</span></span>
| <span data-ttu-id="493bf-120">Header</span><span class="sxs-lookup"><span data-stu-id="493bf-120">Header</span></span>       | <span data-ttu-id="493bf-121">Wert</span><span class="sxs-lookup"><span data-stu-id="493bf-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="493bf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="493bf-122">Authorization</span></span>  | <span data-ttu-id="493bf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="493bf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="493bf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="493bf-125">Request body</span></span>
<span data-ttu-id="493bf-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="493bf-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="493bf-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="493bf-127">Response</span></span>
<span data-ttu-id="493bf-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="493bf-128">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="493bf-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="493bf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="493bf-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="493bf-130">Request</span></span>
<span data-ttu-id="493bf-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="493bf-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="493bf-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="493bf-132">Response</span></span>
<span data-ttu-id="493bf-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="493bf-133">The following is an example of the response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
