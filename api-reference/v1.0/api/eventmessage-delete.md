---
title: eventMessage löschen
description: Mit dieser API können Sie Ressourcen des Typs „eventMessage“ löschen.
ms.openlocfilehash: 14b693d44f64e43aa7357d23fe079e381c78c87a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017348"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="18272-103">eventMessage löschen</span><span class="sxs-lookup"><span data-stu-id="18272-103">Delete eventMessage</span></span>

<span data-ttu-id="18272-104">Mit dieser API können Sie Ressourcen des Typs „eventMessage“ löschen.</span><span class="sxs-lookup"><span data-stu-id="18272-104">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="18272-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18272-105">Permissions</span></span>
<span data-ttu-id="18272-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18272-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18272-108">Permission type</span></span>      | <span data-ttu-id="18272-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18272-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18272-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18272-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18272-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18272-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="18272-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18272-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18272-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18272-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="18272-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18272-114">Application</span></span> | <span data-ttu-id="18272-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18272-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18272-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18272-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="18272-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18272-117">Request headers</span></span>
| <span data-ttu-id="18272-118">Name</span><span class="sxs-lookup"><span data-stu-id="18272-118">Name</span></span>       | <span data-ttu-id="18272-119">Typ</span><span class="sxs-lookup"><span data-stu-id="18272-119">Type</span></span> | <span data-ttu-id="18272-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18272-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18272-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="18272-121">Authorization</span></span>  | <span data-ttu-id="18272-122">string</span><span class="sxs-lookup"><span data-stu-id="18272-122">string</span></span>  | <span data-ttu-id="18272-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18272-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18272-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18272-125">Request body</span></span>
<span data-ttu-id="18272-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="18272-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18272-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="18272-127">Response</span></span>

<span data-ttu-id="18272-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18272-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18272-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18272-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18272-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18272-131">Request</span></span>
<span data-ttu-id="18272-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18272-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="18272-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="18272-133">Response</span></span>
<span data-ttu-id="18272-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18272-134">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->