---
title: Löschen der Anwendung
description: Löscht eine Anwendung.
author: lleonard-msft
ms.openlocfilehash: e19ca94be2d8599f250908ab2aaa33d64b513b8d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343498"
---
# <a name="delete-application"></a><span data-ttu-id="4c014-103">Löschen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c014-103">Delete application</span></span>

> <span data-ttu-id="4c014-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4c014-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c014-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4c014-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c014-106">Löscht eine Anwendung.</span><span class="sxs-lookup"><span data-stu-id="4c014-106">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c014-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4c014-107">Permissions</span></span>
<span data-ttu-id="4c014-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c014-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c014-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c014-110">Permission type</span></span>      | <span data-ttu-id="4c014-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c014-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c014-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c014-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c014-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c014-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c014-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c014-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c014-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c014-115">Not supported.</span></span>    |
|<span data-ttu-id="4c014-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c014-116">Application</span></span> | <span data-ttu-id="4c014-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c014-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c014-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c014-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c014-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4c014-119">Request headers</span></span>
| <span data-ttu-id="4c014-120">Name</span><span class="sxs-lookup"><span data-stu-id="4c014-120">Name</span></span>       | <span data-ttu-id="4c014-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4c014-121">Type</span></span> | <span data-ttu-id="4c014-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c014-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c014-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4c014-123">Authorization</span></span>  | <span data-ttu-id="4c014-124">string</span><span class="sxs-lookup"><span data-stu-id="4c014-124">string</span></span>  | <span data-ttu-id="4c014-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4c014-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c014-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4c014-127">Request body</span></span>
<span data-ttu-id="4c014-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4c014-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c014-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c014-129">Response</span></span>

<span data-ttu-id="4c014-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c014-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c014-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c014-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c014-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c014-133">Request</span></span>
<span data-ttu-id="4c014-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4c014-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="4c014-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c014-135">Response</span></span>
<span data-ttu-id="4c014-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4c014-136">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->