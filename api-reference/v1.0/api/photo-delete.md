---
title: Foto löschen
description: Mit dieser API können Sie Fotos löschen.
ms.openlocfilehash: 8d00eb3685d349efaa88981c6a725faa97896bb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018904"
---
# <a name="delete-photo"></a><span data-ttu-id="284ab-103">Foto löschen</span><span class="sxs-lookup"><span data-stu-id="284ab-103">Delete photo</span></span>

<span data-ttu-id="284ab-104">Mit dieser API können Sie Fotos löschen.</span><span class="sxs-lookup"><span data-stu-id="284ab-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="284ab-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="284ab-105">Permissions</span></span>
<span data-ttu-id="284ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="284ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="284ab-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="284ab-108">Permission type</span></span>      | <span data-ttu-id="284ab-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="284ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="284ab-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="284ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="284ab-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="284ab-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="284ab-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="284ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="284ab-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="284ab-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="284ab-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="284ab-114">Application</span></span> | <span data-ttu-id="284ab-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="284ab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="284ab-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="284ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="284ab-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="284ab-117">Request headers</span></span>
| <span data-ttu-id="284ab-118">Name</span><span class="sxs-lookup"><span data-stu-id="284ab-118">Name</span></span>       | <span data-ttu-id="284ab-119">Typ</span><span class="sxs-lookup"><span data-stu-id="284ab-119">Type</span></span> | <span data-ttu-id="284ab-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="284ab-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="284ab-121">if-match</span><span class="sxs-lookup"><span data-stu-id="284ab-121">if-match</span></span>  | <span data-ttu-id="284ab-122">string</span><span class="sxs-lookup"><span data-stu-id="284ab-122">string</span></span>  | <span data-ttu-id="284ab-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene Etag (oder CTag) nicht mit dem aktuellen Etag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="284ab-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="284ab-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="284ab-124">Authorization</span></span>  | <span data-ttu-id="284ab-125">string</span><span class="sxs-lookup"><span data-stu-id="284ab-125">string</span></span>  | <span data-ttu-id="284ab-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="284ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="284ab-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="284ab-128">Request body</span></span>
<span data-ttu-id="284ab-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="284ab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="284ab-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="284ab-130">Response</span></span>

<span data-ttu-id="284ab-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="284ab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="284ab-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="284ab-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="284ab-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="284ab-134">Request</span></span>
<span data-ttu-id="284ab-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="284ab-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="284ab-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="284ab-136">Response</span></span>
<span data-ttu-id="284ab-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="284ab-137">Here is an example of the response.</span></span>
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
