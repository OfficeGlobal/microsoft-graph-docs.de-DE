---
title: Domäne aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines Domänenobjekts.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 7815d86a733d597860ed986b926972e328598f65
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843519"
---
# <a name="update-domain"></a><span data-ttu-id="6dc5d-103">Domäne aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6dc5d-103">Update domain</span></span>

> <span data-ttu-id="6dc5d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6dc5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6dc5d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6dc5d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6dc5d-106">Dient zum Aktualisieren der Eigenschaften eines Domänenobjekts.</span><span class="sxs-lookup"><span data-stu-id="6dc5d-106">Update the properties of domain object.</span></span>

> <span data-ttu-id="6dc5d-107">**Wichtig:** Nur überprüfte Domänen können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="6dc5d-107">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dc5d-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6dc5d-108">Permissions</span></span>

<span data-ttu-id="6dc5d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dc5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6dc5d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6dc5d-111">Permission type</span></span>      | <span data-ttu-id="6dc5d-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6dc5d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dc5d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6dc5d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6dc5d-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6dc5d-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6dc5d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6dc5d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dc5d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6dc5d-116">Not supported.</span></span>    |
|<span data-ttu-id="6dc5d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6dc5d-117">Application</span></span> | <span data-ttu-id="6dc5d-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc5d-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dc5d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dc5d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="6dc5d-120">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="6dc5d-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dc5d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6dc5d-121">Request headers</span></span>

| <span data-ttu-id="6dc5d-122">Name</span><span class="sxs-lookup"><span data-stu-id="6dc5d-122">Name</span></span>       | <span data-ttu-id="6dc5d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6dc5d-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6dc5d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dc5d-124">Authorization</span></span>  | <span data-ttu-id="6dc5d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6dc5d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6dc5d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6dc5d-127">Content-Type</span></span>  | <span data-ttu-id="6dc5d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc5d-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dc5d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6dc5d-129">Request body</span></span>

<span data-ttu-id="6dc5d-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Für optimale Leistung sollten Sie nur geänderte Werte einschließen.</span><span class="sxs-lookup"><span data-stu-id="6dc5d-p104">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="6dc5d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dc5d-133">Response</span></span>

<span data-ttu-id="6dc5d-134">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben, aber kein Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6dc5d-134">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dc5d-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6dc5d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6dc5d-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dc5d-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/beta/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="6dc5d-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dc5d-137">Response</span></span>

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
