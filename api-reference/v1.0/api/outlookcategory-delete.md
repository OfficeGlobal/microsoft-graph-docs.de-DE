---
title: Löschen der Outlook-Kategorie
description: Löscht das angegebene outlookCategory-Objekt.
author: angelgolfer-ms
ms.openlocfilehash: ded640425c30352cc83d4adaa02c76ed2bcfa170
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301036"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="b8780-103">Löschen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="b8780-103">Delete Outlook category</span></span>


<span data-ttu-id="b8780-104">Löscht das angegebene [outlookCategory](../resources/outlookcategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b8780-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8780-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8780-105">Permissions</span></span>
<span data-ttu-id="b8780-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8780-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8780-108">Permission type</span></span>      | <span data-ttu-id="b8780-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8780-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8780-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8780-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8780-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8780-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b8780-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8780-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8780-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8780-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b8780-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8780-114">Application</span></span> | <span data-ttu-id="b8780-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8780-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8780-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8780-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8780-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b8780-117">Optional query parameters</span></span>
<span data-ttu-id="b8780-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8780-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8780-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8780-119">Request headers</span></span>
| <span data-ttu-id="b8780-120">Name</span><span class="sxs-lookup"><span data-stu-id="b8780-120">Name</span></span>      |<span data-ttu-id="b8780-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8780-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8780-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8780-122">Authorization</span></span>  | <span data-ttu-id="b8780-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8780-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8780-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8780-125">Request body</span></span>
<span data-ttu-id="b8780-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b8780-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8780-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8780-127">Response</span></span>

<span data-ttu-id="b8780-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8780-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8780-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8780-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8780-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8780-131">Request</span></span>
<span data-ttu-id="b8780-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8780-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="b8780-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8780-133">Response</span></span>
<span data-ttu-id="b8780-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8780-134">Here is an example of the response.</span></span>
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