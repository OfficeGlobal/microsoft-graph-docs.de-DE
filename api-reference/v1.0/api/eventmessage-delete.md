---
title: eventMessage löschen
description: Mit dieser API können Sie Ressourcen des Typs „eventMessage“ löschen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: fb6f00b642a919e63250074dc6f447be7997a722
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831276"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="62791-103">eventMessage löschen</span><span class="sxs-lookup"><span data-stu-id="62791-103">Delete eventMessage</span></span>

<span data-ttu-id="62791-104">Mit dieser API können Sie Ressourcen des Typs „eventMessage“ löschen.</span><span class="sxs-lookup"><span data-stu-id="62791-104">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="62791-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="62791-105">Permissions</span></span>
<span data-ttu-id="62791-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62791-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62791-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62791-108">Permission type</span></span>      | <span data-ttu-id="62791-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62791-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62791-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62791-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62791-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62791-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="62791-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62791-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62791-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62791-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="62791-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62791-114">Application</span></span> | <span data-ttu-id="62791-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62791-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="62791-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62791-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="62791-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="62791-117">Request headers</span></span>
| <span data-ttu-id="62791-118">Name</span><span class="sxs-lookup"><span data-stu-id="62791-118">Name</span></span>       | <span data-ttu-id="62791-119">Typ</span><span class="sxs-lookup"><span data-stu-id="62791-119">Type</span></span> | <span data-ttu-id="62791-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62791-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="62791-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62791-121">Authorization</span></span>  | <span data-ttu-id="62791-122">string</span><span class="sxs-lookup"><span data-stu-id="62791-122">string</span></span>  | <span data-ttu-id="62791-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="62791-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62791-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62791-125">Request body</span></span>
<span data-ttu-id="62791-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="62791-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62791-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="62791-127">Response</span></span>

<span data-ttu-id="62791-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62791-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62791-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62791-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62791-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="62791-131">Request</span></span>
<span data-ttu-id="62791-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="62791-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="62791-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="62791-133">Response</span></span>
<span data-ttu-id="62791-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="62791-134">Here is an example of the response.</span></span> 
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
