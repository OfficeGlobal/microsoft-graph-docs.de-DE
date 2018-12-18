---
title: EducationClass entfernen
description: Löscht eine Klasse aus einer Schule.
author: mmast-msft
ms.openlocfilehash: 7c69d03670adca93194c5761aa6f943ee9201ac8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319250"
---
# <a name="remove-educationclass"></a><span data-ttu-id="e9722-103">EducationClass entfernen</span><span class="sxs-lookup"><span data-stu-id="e9722-103">Remove educationClass</span></span>

> <span data-ttu-id="e9722-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e9722-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9722-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9722-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9722-106">Löscht eine Klasse aus einer Schule.</span><span class="sxs-lookup"><span data-stu-id="e9722-106">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9722-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e9722-107">Permissions</span></span>
<span data-ttu-id="e9722-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9722-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9722-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e9722-110">Permission type</span></span>      | <span data-ttu-id="e9722-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e9722-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9722-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e9722-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e9722-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9722-113">Not supported.</span></span>  |
|<span data-ttu-id="e9722-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e9722-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e9722-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9722-115">Not supported.</span></span>  |
|<span data-ttu-id="e9722-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e9722-116">Application</span></span> | <span data-ttu-id="e9722-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9722-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e9722-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9722-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e9722-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e9722-119">Request headers</span></span>
| <span data-ttu-id="e9722-120">Header</span><span class="sxs-lookup"><span data-stu-id="e9722-120">Header</span></span>       | <span data-ttu-id="e9722-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e9722-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9722-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9722-122">Authorization</span></span>  | <span data-ttu-id="e9722-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e9722-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9722-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e9722-125">Request body</span></span>
<span data-ttu-id="e9722-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e9722-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e9722-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9722-127">Response</span></span>
<span data-ttu-id="e9722-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e9722-128">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9722-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e9722-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9722-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9722-130">Request</span></span>
<span data-ttu-id="e9722-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e9722-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="e9722-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9722-132">Response</span></span>
<span data-ttu-id="e9722-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e9722-133">The following is an example of the response.</span></span> 

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