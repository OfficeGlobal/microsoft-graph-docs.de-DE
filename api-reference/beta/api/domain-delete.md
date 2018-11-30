---
title: Domäne löschen
description: Dient zum Löschen einer Domäne aus einem Mandanten.
ms.openlocfilehash: 2ed3772d767099e8ccd7fd5453c7a8231c9ea96c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061552"
---
# <a name="delete-domain"></a><span data-ttu-id="3815b-103">Domäne löschen</span><span class="sxs-lookup"><span data-stu-id="3815b-103">Delete domain</span></span>

> <span data-ttu-id="3815b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3815b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3815b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3815b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3815b-106">Dient zum Löschen einer Domäne aus einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3815b-106">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="3815b-107">**Wichtig:** Gelöschte Domänen können nicht wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="3815b-107">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="3815b-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3815b-108">Permissions</span></span>

<span data-ttu-id="3815b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3815b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3815b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3815b-111">Permission type</span></span>      | <span data-ttu-id="3815b-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3815b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3815b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3815b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3815b-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3815b-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3815b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3815b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3815b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3815b-116">Not supported.</span></span>    |
|<span data-ttu-id="3815b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3815b-117">Application</span></span> | <span data-ttu-id="3815b-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3815b-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3815b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3815b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="3815b-120">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="3815b-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3815b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3815b-121">Request headers</span></span>

| <span data-ttu-id="3815b-122">Name</span><span class="sxs-lookup"><span data-stu-id="3815b-122">Name</span></span>       | <span data-ttu-id="3815b-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3815b-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3815b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3815b-124">Authorization</span></span>  | <span data-ttu-id="3815b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3815b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3815b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3815b-127">Content-Type</span></span>  | <span data-ttu-id="3815b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3815b-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3815b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3815b-129">Request body</span></span>

<span data-ttu-id="3815b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3815b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3815b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3815b-131">Response</span></span>

<span data-ttu-id="3815b-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Es wird keine Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3815b-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="3815b-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3815b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3815b-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3815b-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="3815b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3815b-136">Response</span></span>

<span data-ttu-id="3815b-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3815b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->