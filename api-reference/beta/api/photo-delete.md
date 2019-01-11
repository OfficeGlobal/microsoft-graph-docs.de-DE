---
title: Foto löschen
description: Mit dieser API können Sie Fotos löschen.
localization_priority: Normal
ms.openlocfilehash: 117f4acbf5a45d9db64ccc5d3fc0ccc4d1c64896
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829260"
---
# <a name="delete-photo"></a><span data-ttu-id="8f5ca-103">Foto löschen</span><span class="sxs-lookup"><span data-stu-id="8f5ca-103">Delete photo</span></span>

> <span data-ttu-id="8f5ca-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8f5ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f5ca-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f5ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f5ca-106">Mit dieser API können Sie Fotos löschen.</span><span class="sxs-lookup"><span data-stu-id="8f5ca-106">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f5ca-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8f5ca-107">Permissions</span></span>
<span data-ttu-id="8f5ca-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f5ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f5ca-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8f5ca-110">Permission type</span></span>      | <span data-ttu-id="8f5ca-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8f5ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f5ca-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8f5ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f5ca-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f5ca-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f5ca-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8f5ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f5ca-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f5ca-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f5ca-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8f5ca-116">Application</span></span> | <span data-ttu-id="8f5ca-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f5ca-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f5ca-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f5ca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="8f5ca-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8f5ca-119">Request headers</span></span>
| <span data-ttu-id="8f5ca-120">Name</span><span class="sxs-lookup"><span data-stu-id="8f5ca-120">Name</span></span>       | <span data-ttu-id="8f5ca-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8f5ca-121">Type</span></span> | <span data-ttu-id="8f5ca-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f5ca-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8f5ca-123">if-match</span><span class="sxs-lookup"><span data-stu-id="8f5ca-123">if-match</span></span>  | <span data-ttu-id="8f5ca-124">string</span><span class="sxs-lookup"><span data-stu-id="8f5ca-124">string</span></span>  | <span data-ttu-id="8f5ca-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene Etag (oder CTag) nicht mit dem aktuellen Etag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="8f5ca-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="8f5ca-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f5ca-126">Authorization</span></span>  | <span data-ttu-id="8f5ca-127">string</span><span class="sxs-lookup"><span data-stu-id="8f5ca-127">string</span></span>  | <span data-ttu-id="8f5ca-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f5ca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f5ca-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8f5ca-130">Request body</span></span>
<span data-ttu-id="8f5ca-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8f5ca-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f5ca-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f5ca-132">Response</span></span>

<span data-ttu-id="8f5ca-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f5ca-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f5ca-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8f5ca-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f5ca-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f5ca-136">Request</span></span>
<span data-ttu-id="8f5ca-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8f5ca-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="8f5ca-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f5ca-138">Response</span></span>
<span data-ttu-id="8f5ca-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8f5ca-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
