---
title: Löschen der Outlook-Kategorie
description: Löscht das angegebene outlookCategory-Objekt.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5c909176634d64245d5ff5521c0da68b02e8777b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972264"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="ecf0a-103">Löschen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="ecf0a-103">Delete Outlook category</span></span>


<span data-ttu-id="ecf0a-104">Löscht das angegebene [outlookCategory](../resources/outlookcategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ecf0a-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecf0a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ecf0a-105">Permissions</span></span>
<span data-ttu-id="ecf0a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecf0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecf0a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ecf0a-108">Permission type</span></span>      | <span data-ttu-id="ecf0a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ecf0a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecf0a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ecf0a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ecf0a-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ecf0a-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="ecf0a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ecf0a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecf0a-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ecf0a-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="ecf0a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ecf0a-114">Application</span></span> | <span data-ttu-id="ecf0a-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ecf0a-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecf0a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecf0a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ecf0a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ecf0a-117">Request headers</span></span>
| <span data-ttu-id="ecf0a-118">Name</span><span class="sxs-lookup"><span data-stu-id="ecf0a-118">Name</span></span>      |<span data-ttu-id="ecf0a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ecf0a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ecf0a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecf0a-120">Authorization</span></span>  | <span data-ttu-id="ecf0a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ecf0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecf0a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ecf0a-123">Request body</span></span>
<span data-ttu-id="ecf0a-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ecf0a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecf0a-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecf0a-125">Response</span></span>

<span data-ttu-id="ecf0a-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ecf0a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecf0a-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ecf0a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ecf0a-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecf0a-129">Request</span></span>
<span data-ttu-id="ecf0a-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ecf0a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="ecf0a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecf0a-131">Response</span></span>
<span data-ttu-id="ecf0a-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ecf0a-132">Here is an example of the response.</span></span>
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
