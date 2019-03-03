---
title: Threat Intelligence-Indikator löschen
description: Löscht ein tiIndicator-Objekt.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: eac07b5d3e81e3e3098fb63bbf0be838c7d51b2c
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366896"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="c746a-103">Threat Intelligence-Indikator löschen</span><span class="sxs-lookup"><span data-stu-id="c746a-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c746a-104">Löscht ein [tiIndicator](../resources/tiindicator.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="c746a-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c746a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c746a-105">Permissions</span></span>

<span data-ttu-id="c746a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c746a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c746a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c746a-108">Permission type</span></span>                        | <span data-ttu-id="c746a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c746a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c746a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c746a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c746a-111">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c746a-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="c746a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c746a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c746a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c746a-113">Not supported.</span></span> |
| <span data-ttu-id="c746a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c746a-114">Application</span></span>                            | <span data-ttu-id="c746a-115">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c746a-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="c746a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c746a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c746a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c746a-117">Request headers</span></span>

| <span data-ttu-id="c746a-118">Name</span><span class="sxs-lookup"><span data-stu-id="c746a-118">Name</span></span>          | <span data-ttu-id="c746a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c746a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c746a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c746a-120">Authorization</span></span> | <span data-ttu-id="c746a-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c746a-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c746a-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c746a-122">Request body</span></span>

<span data-ttu-id="c746a-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c746a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c746a-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="c746a-124">Response</span></span>

<span data-ttu-id="c746a-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c746a-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c746a-127">Beispiele</span><span class="sxs-lookup"><span data-stu-id="c746a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c746a-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c746a-128">Request</span></span>

<span data-ttu-id="c746a-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c746a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="c746a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c746a-130">Response</span></span>

<span data-ttu-id="c746a-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c746a-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
