---
title: eventMessage löschen
description: Mit dieser API können Sie Ressourcen des Typs „eventMessage“ löschen.
author: angelgolfer-ms
ms.openlocfilehash: 13ca9c908dc1b00a355c33f69951e04b80f26e0a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337716"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="e5967-103">eventMessage löschen</span><span class="sxs-lookup"><span data-stu-id="e5967-103">Delete eventMessage</span></span>

<span data-ttu-id="e5967-104">Mit dieser API können Sie Ressourcen des Typs „eventMessage“ löschen.</span><span class="sxs-lookup"><span data-stu-id="e5967-104">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5967-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e5967-105">Permissions</span></span>
<span data-ttu-id="e5967-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5967-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5967-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e5967-108">Permission type</span></span>      | <span data-ttu-id="e5967-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e5967-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5967-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e5967-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5967-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5967-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e5967-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e5967-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5967-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5967-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e5967-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e5967-114">Application</span></span> | <span data-ttu-id="e5967-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5967-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5967-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5967-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e5967-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e5967-117">Request headers</span></span>
| <span data-ttu-id="e5967-118">Name</span><span class="sxs-lookup"><span data-stu-id="e5967-118">Name</span></span>       | <span data-ttu-id="e5967-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e5967-119">Type</span></span> | <span data-ttu-id="e5967-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5967-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5967-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e5967-121">Authorization</span></span>  | <span data-ttu-id="e5967-122">string</span><span class="sxs-lookup"><span data-stu-id="e5967-122">string</span></span>  | <span data-ttu-id="e5967-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e5967-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5967-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e5967-125">Request body</span></span>
<span data-ttu-id="e5967-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e5967-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5967-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5967-127">Response</span></span>

<span data-ttu-id="e5967-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5967-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5967-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5967-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5967-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5967-131">Request</span></span>
<span data-ttu-id="e5967-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e5967-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="e5967-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5967-133">Response</span></span>
<span data-ttu-id="e5967-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e5967-134">Here is an example of the response.</span></span> 
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