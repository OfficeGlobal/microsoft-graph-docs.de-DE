---
title: Domäne aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines Domänenobjekts.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: da51badb52b5047c6d5eb1d52004104d0395fcf2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923782"
---
# <a name="update-domain"></a><span data-ttu-id="96991-103">Domäne aktualisieren</span><span class="sxs-lookup"><span data-stu-id="96991-103">Update domain</span></span>

<span data-ttu-id="96991-104">Dient zum Aktualisieren der Eigenschaften eines Domänenobjekts.</span><span class="sxs-lookup"><span data-stu-id="96991-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="96991-105">**Wichtig:** Nur überprüfte Domänen können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="96991-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="96991-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="96991-106">Permissions</span></span>

<span data-ttu-id="96991-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96991-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="96991-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96991-109">Permission type</span></span>      | <span data-ttu-id="96991-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96991-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96991-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96991-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96991-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96991-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="96991-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96991-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96991-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96991-114">Not supported.</span></span>    |
|<span data-ttu-id="96991-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96991-115">Application</span></span> | <span data-ttu-id="96991-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96991-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96991-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96991-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="96991-118">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="96991-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96991-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96991-119">Request headers</span></span>

| <span data-ttu-id="96991-120">Name</span><span class="sxs-lookup"><span data-stu-id="96991-120">Name</span></span>       | <span data-ttu-id="96991-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96991-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="96991-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96991-122">Authorization</span></span>  | <span data-ttu-id="96991-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96991-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96991-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96991-125">Content-Type</span></span>  | <span data-ttu-id="96991-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96991-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="96991-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96991-127">Request body</span></span>

<span data-ttu-id="96991-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Für optimale Leistung sollten Sie nur geänderte Werte einschließen.</span><span class="sxs-lookup"><span data-stu-id="96991-p103">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="96991-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="96991-131">Response</span></span>

<span data-ttu-id="96991-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben, aber kein Antworttext.</span><span class="sxs-lookup"><span data-stu-id="96991-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="96991-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96991-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96991-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96991-134">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="96991-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="96991-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
