---
title: ServicePrincipal löschen
description: Löschen Sie ServicePrincipal.
localization_priority: Normal
ms.openlocfilehash: 4e2cd3adeacc1e7c1f7e3c955f247800a63673b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873836"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="2d4c1-103">ServicePrincipal löschen</span><span class="sxs-lookup"><span data-stu-id="2d4c1-103">Delete servicePrincipal</span></span>

> <span data-ttu-id="2d4c1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2d4c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d4c1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d4c1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d4c1-106">Löschen Sie ServicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="2d4c1-106">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d4c1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2d4c1-107">Permissions</span></span>
<span data-ttu-id="2d4c1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d4c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d4c1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d4c1-110">Permission type</span></span>      | <span data-ttu-id="2d4c1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d4c1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d4c1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d4c1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d4c1-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2d4c1-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2d4c1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d4c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d4c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d4c1-115">Not supported.</span></span>    |
|<span data-ttu-id="2d4c1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d4c1-116">Application</span></span> | <span data-ttu-id="2d4c1-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d4c1-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d4c1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d4c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="2d4c1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d4c1-119">Request headers</span></span>
| <span data-ttu-id="2d4c1-120">Name</span><span class="sxs-lookup"><span data-stu-id="2d4c1-120">Name</span></span>       | <span data-ttu-id="2d4c1-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2d4c1-121">Type</span></span> | <span data-ttu-id="2d4c1-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d4c1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2d4c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d4c1-123">Authorization</span></span>  | <span data-ttu-id="2d4c1-124">string</span><span class="sxs-lookup"><span data-stu-id="2d4c1-124">string</span></span>  | <span data-ttu-id="2d4c1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d4c1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d4c1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d4c1-127">Request body</span></span>
<span data-ttu-id="2d4c1-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2d4c1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d4c1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d4c1-129">Response</span></span>

<span data-ttu-id="2d4c1-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d4c1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d4c1-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d4c1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d4c1-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d4c1-133">Request</span></span>
<span data-ttu-id="2d4c1-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d4c1-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="2d4c1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d4c1-135">Response</span></span>
<span data-ttu-id="2d4c1-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d4c1-136">Here is an example of the response.</span></span> 
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
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
