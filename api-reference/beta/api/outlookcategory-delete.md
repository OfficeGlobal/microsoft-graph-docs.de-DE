---
title: Löschen der Outlook-Kategorie
description: Löscht das angegebene outlookCategory-Objekt.
ms.openlocfilehash: a240df167918892face0da8932af0f2ff3d23152
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059999"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="88461-103">Löschen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="88461-103">Delete Outlook category</span></span>

> <span data-ttu-id="88461-104">**Wichtig**: unter der /beta Version von Microsoft Graph-APIs sind in der Vorschau und kann geändert werden.</span><span class="sxs-lookup"><span data-stu-id="88461-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88461-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88461-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88461-106">Löscht das angegebene [outlookCategory](../resources/outlookcategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="88461-106">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="88461-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="88461-107">Permissions</span></span>
<span data-ttu-id="88461-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88461-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88461-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="88461-110">Permission type</span></span>      | <span data-ttu-id="88461-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88461-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88461-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88461-112">Delegated (work or school account)</span></span> | <span data-ttu-id="88461-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88461-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="88461-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88461-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88461-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88461-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="88461-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88461-116">Application</span></span> | <span data-ttu-id="88461-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88461-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="88461-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88461-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88461-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="88461-119">Optional query parameters</span></span>
<span data-ttu-id="88461-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88461-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88461-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88461-121">Request headers</span></span>
| <span data-ttu-id="88461-122">Name</span><span class="sxs-lookup"><span data-stu-id="88461-122">Name</span></span>      |<span data-ttu-id="88461-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88461-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88461-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="88461-124">Authorization</span></span>  | <span data-ttu-id="88461-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="88461-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88461-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="88461-127">Request body</span></span>
<span data-ttu-id="88461-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="88461-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88461-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="88461-129">Response</span></span>

<span data-ttu-id="88461-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="88461-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88461-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88461-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88461-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88461-133">Request</span></span>
<span data-ttu-id="88461-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="88461-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories('4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
```
##### <a name="response"></a><span data-ttu-id="88461-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="88461-135">Response</span></span>
<span data-ttu-id="88461-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88461-136">Here is an example of the response.</span></span>
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