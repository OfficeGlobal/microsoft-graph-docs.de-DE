---
title: Vereinbarung löschen
description: Ein Objekt zu löschen.
ms.openlocfilehash: 919fc628e5f8ff9b6c016e085671f47ed6d56a5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060954"
---
# <a name="delete-agreement"></a><span data-ttu-id="8c730-103">Vereinbarung löschen</span><span class="sxs-lookup"><span data-stu-id="8c730-103">Delete agreement</span></span>

> <span data-ttu-id="8c730-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c730-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c730-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c730-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c730-106">Ein Objekt [zu](../resources/agreement.md) löschen.</span><span class="sxs-lookup"><span data-stu-id="8c730-106">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c730-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8c730-107">Permissions</span></span>
<span data-ttu-id="8c730-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c730-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c730-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c730-110">Permission type</span></span>                        | <span data-ttu-id="8c730-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c730-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c730-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c730-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c730-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c730-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="8c730-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c730-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c730-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c730-115">Not supported.</span></span> |
|<span data-ttu-id="8c730-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c730-116">Application</span></span>                            | <span data-ttu-id="8c730-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c730-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c730-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c730-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="8c730-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c730-119">Request headers</span></span>
| <span data-ttu-id="8c730-120">Name</span><span class="sxs-lookup"><span data-stu-id="8c730-120">Name</span></span>         | <span data-ttu-id="8c730-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8c730-121">Type</span></span>        | <span data-ttu-id="8c730-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c730-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8c730-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c730-123">Authorization</span></span> | <span data-ttu-id="8c730-124">string</span><span class="sxs-lookup"><span data-stu-id="8c730-124">string</span></span> | <span data-ttu-id="8c730-125">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="8c730-125">Bearer \{token\}.</span></span> <span data-ttu-id="8c730-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8c730-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c730-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c730-127">Request body</span></span>
<span data-ttu-id="8c730-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8c730-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8c730-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c730-129">Response</span></span>
<span data-ttu-id="8c730-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c730-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c730-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c730-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c730-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c730-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="8c730-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c730-134">Response</span></span>
><span data-ttu-id="8c730-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8c730-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
