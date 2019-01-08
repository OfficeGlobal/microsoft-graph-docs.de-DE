---
title: Löschen der Outlook-Kategorie
description: Löscht das angegebene outlookCategory-Objekt.
author: angelgolfer-ms
ms.openlocfilehash: 114dee21aea5143bd3ad1d6503490ed7941fe6f3
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748234"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="ac892-103">Löschen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="ac892-103">Delete Outlook category</span></span>

> <span data-ttu-id="ac892-104">**Wichtig**: unter der /beta Version von Microsoft Graph-APIs sind in der Vorschau und kann geändert werden.</span><span class="sxs-lookup"><span data-stu-id="ac892-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac892-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac892-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac892-106">Löscht das angegebene [outlookCategory](../resources/outlookcategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ac892-106">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac892-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ac892-107">Permissions</span></span>
<span data-ttu-id="ac892-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac892-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac892-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ac892-110">Permission type</span></span>      | <span data-ttu-id="ac892-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ac892-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac892-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ac892-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ac892-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac892-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="ac892-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ac892-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac892-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac892-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="ac892-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ac892-116">Application</span></span> | <span data-ttu-id="ac892-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac892-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac892-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac892-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ac892-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ac892-119">Request headers</span></span>
| <span data-ttu-id="ac892-120">Name</span><span class="sxs-lookup"><span data-stu-id="ac892-120">Name</span></span>      |<span data-ttu-id="ac892-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac892-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac892-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac892-122">Authorization</span></span>  | <span data-ttu-id="ac892-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ac892-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac892-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ac892-125">Request body</span></span>
<span data-ttu-id="ac892-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ac892-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac892-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac892-127">Response</span></span>

<span data-ttu-id="ac892-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac892-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac892-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac892-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac892-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac892-131">Request</span></span>
<span data-ttu-id="ac892-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac892-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories('4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
```
##### <a name="response"></a><span data-ttu-id="ac892-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac892-133">Response</span></span>
<span data-ttu-id="ac892-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ac892-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->