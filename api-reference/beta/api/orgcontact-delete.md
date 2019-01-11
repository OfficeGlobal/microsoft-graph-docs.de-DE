---
title: OrgContact löschen
description: Löschen Sie OrgContact.
localization_priority: Normal
ms.openlocfilehash: 3eecd42debf22f7bd2330ddae5a8321b25b7350c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892064"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="01980-103">OrgContact löschen</span><span class="sxs-lookup"><span data-stu-id="01980-103">Delete orgContact</span></span>

> <span data-ttu-id="01980-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="01980-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01980-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="01980-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01980-106">Löschen Sie OrgContact.</span><span class="sxs-lookup"><span data-stu-id="01980-106">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="01980-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="01980-107">Permissions</span></span>
<span data-ttu-id="01980-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01980-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01980-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="01980-110">Permission type</span></span>      | <span data-ttu-id="01980-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="01980-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01980-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="01980-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01980-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01980-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01980-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="01980-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01980-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01980-115">Not supported.</span></span>    |
|<span data-ttu-id="01980-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="01980-116">Application</span></span> | <span data-ttu-id="01980-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01980-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01980-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="01980-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="01980-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="01980-119">Request headers</span></span>
| <span data-ttu-id="01980-120">Name</span><span class="sxs-lookup"><span data-stu-id="01980-120">Name</span></span>       | <span data-ttu-id="01980-121">Typ</span><span class="sxs-lookup"><span data-stu-id="01980-121">Type</span></span> | <span data-ttu-id="01980-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01980-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="01980-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01980-123">Authorization</span></span>  | <span data-ttu-id="01980-124">string</span><span class="sxs-lookup"><span data-stu-id="01980-124">string</span></span>  | <span data-ttu-id="01980-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="01980-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01980-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="01980-127">Request body</span></span>
<span data-ttu-id="01980-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="01980-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01980-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="01980-129">Response</span></span>

<span data-ttu-id="01980-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01980-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01980-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="01980-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01980-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="01980-133">Request</span></span>
<span data-ttu-id="01980-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="01980-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="01980-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="01980-135">Response</span></span>
<span data-ttu-id="01980-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="01980-136">Here is an example of the response.</span></span> 
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
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
