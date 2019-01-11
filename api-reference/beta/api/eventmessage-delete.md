---
title: eventMessage löschen
description: Mit dieser API können Sie Ressourcen des Typs „eventMessage“ löschen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 032e43b603edbcce880ec8b1309b417e72f3bf03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887787"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="19e46-103">eventMessage löschen</span><span class="sxs-lookup"><span data-stu-id="19e46-103">Delete eventMessage</span></span>

> <span data-ttu-id="19e46-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="19e46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19e46-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19e46-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19e46-106">Mit dieser API können Sie Ressourcen des Typs „eventMessage“ löschen.</span><span class="sxs-lookup"><span data-stu-id="19e46-106">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="19e46-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="19e46-107">Permissions</span></span>
<span data-ttu-id="19e46-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19e46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19e46-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19e46-110">Permission type</span></span>      | <span data-ttu-id="19e46-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19e46-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19e46-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19e46-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19e46-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19e46-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="19e46-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19e46-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19e46-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19e46-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="19e46-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19e46-116">Application</span></span> | <span data-ttu-id="19e46-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19e46-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="19e46-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19e46-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="19e46-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19e46-119">Request headers</span></span>
| <span data-ttu-id="19e46-120">Name</span><span class="sxs-lookup"><span data-stu-id="19e46-120">Name</span></span>       | <span data-ttu-id="19e46-121">Typ</span><span class="sxs-lookup"><span data-stu-id="19e46-121">Type</span></span> | <span data-ttu-id="19e46-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19e46-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19e46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19e46-123">Authorization</span></span>  | <span data-ttu-id="19e46-124">string</span><span class="sxs-lookup"><span data-stu-id="19e46-124">string</span></span>  | <span data-ttu-id="19e46-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="19e46-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19e46-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19e46-127">Request body</span></span>
<span data-ttu-id="19e46-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="19e46-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19e46-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="19e46-129">Response</span></span>

<span data-ttu-id="19e46-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19e46-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19e46-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19e46-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19e46-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19e46-133">Request</span></span>
<span data-ttu-id="19e46-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19e46-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="19e46-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="19e46-135">Response</span></span>
<span data-ttu-id="19e46-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="19e46-136">Here is an example of the response.</span></span> 
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
