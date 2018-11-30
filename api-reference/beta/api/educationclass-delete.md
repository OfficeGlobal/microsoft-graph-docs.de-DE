---
title: EducationClass löschen
description: Löschen einer Klasse. Da eine Klasse auch eine universelle Gruppe ist, wird beim Löschen einer Klasse die Gruppe gelöscht.
ms.openlocfilehash: e63903f1a6db2c223071f04db26f31e3cfbc2168
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063071"
---
# <a name="delete-educationclass"></a><span data-ttu-id="d9ee0-104">EducationClass löschen</span><span class="sxs-lookup"><span data-stu-id="d9ee0-104">Delete educationClass</span></span>

> <span data-ttu-id="d9ee0-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9ee0-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9ee0-107">Löschen einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-107">Delete a class.</span></span> <span data-ttu-id="d9ee0-108">Da eine Klasse auch eine universelle Gruppe ist, wird beim Löschen einer Klasse die Gruppe gelöscht.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-108">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9ee0-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d9ee0-109">Permissions</span></span>
<span data-ttu-id="d9ee0-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9ee0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9ee0-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9ee0-112">Permission type</span></span>      | <span data-ttu-id="d9ee0-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9ee0-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="d9ee0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9ee0-115">Not supported.</span></span>  |
|<span data-ttu-id="d9ee0-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d9ee0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9ee0-117">Not supported.</span></span>  |
|<span data-ttu-id="d9ee0-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9ee0-118">Application</span></span> | <span data-ttu-id="d9ee0-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ee0-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d9ee0-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9ee0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d9ee0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9ee0-121">Request headers</span></span>
| <span data-ttu-id="d9ee0-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d9ee0-122">Header</span></span>       | <span data-ttu-id="d9ee0-123">Wert</span><span class="sxs-lookup"><span data-stu-id="d9ee0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9ee0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9ee0-124">Authorization</span></span>  | <span data-ttu-id="d9ee0-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9ee0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9ee0-127">Request body</span></span>
<span data-ttu-id="d9ee0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d9ee0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9ee0-129">Response</span></span>
<span data-ttu-id="d9ee0-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9ee0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9ee0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9ee0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9ee0-133">Request</span></span>
<span data-ttu-id="d9ee0-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="d9ee0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9ee0-135">Response</span></span>
<span data-ttu-id="d9ee0-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-136">The following is an example of the response.</span></span> 

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