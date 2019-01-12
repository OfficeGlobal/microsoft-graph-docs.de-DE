---
title: EducationClass löschen
description: Löschen einer Klasse. Da eine Klasse auch eine universelle Gruppe ist, wird beim Löschen einer Klasse die Gruppe gelöscht.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9b25e95dfa109ef48d67374ba7569a32af22ba50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935066"
---
# <a name="delete-educationclass"></a><span data-ttu-id="15f69-104">EducationClass löschen</span><span class="sxs-lookup"><span data-stu-id="15f69-104">Delete educationClass</span></span>

> <span data-ttu-id="15f69-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15f69-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15f69-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15f69-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15f69-107">Löschen einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="15f69-107">Delete a class.</span></span> <span data-ttu-id="15f69-108">Da eine Klasse auch eine universelle Gruppe ist, wird beim Löschen einer Klasse die Gruppe gelöscht.</span><span class="sxs-lookup"><span data-stu-id="15f69-108">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="15f69-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="15f69-109">Permissions</span></span>
<span data-ttu-id="15f69-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15f69-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15f69-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15f69-112">Permission type</span></span>      | <span data-ttu-id="15f69-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15f69-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15f69-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15f69-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="15f69-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15f69-115">Not supported.</span></span>  |
|<span data-ttu-id="15f69-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15f69-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="15f69-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15f69-117">Not supported.</span></span>  |
|<span data-ttu-id="15f69-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15f69-118">Application</span></span> | <span data-ttu-id="15f69-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f69-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="15f69-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15f69-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="15f69-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15f69-121">Request headers</span></span>
| <span data-ttu-id="15f69-122">Header</span><span class="sxs-lookup"><span data-stu-id="15f69-122">Header</span></span>       | <span data-ttu-id="15f69-123">Wert</span><span class="sxs-lookup"><span data-stu-id="15f69-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="15f69-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="15f69-124">Authorization</span></span>  | <span data-ttu-id="15f69-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15f69-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15f69-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15f69-127">Request body</span></span>
<span data-ttu-id="15f69-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="15f69-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="15f69-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="15f69-129">Response</span></span>
<span data-ttu-id="15f69-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15f69-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15f69-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15f69-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15f69-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15f69-133">Request</span></span>
<span data-ttu-id="15f69-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15f69-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="15f69-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="15f69-135">Response</span></span>
<span data-ttu-id="15f69-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="15f69-136">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
