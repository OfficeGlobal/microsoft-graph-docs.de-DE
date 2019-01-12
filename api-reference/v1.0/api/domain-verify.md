---
title: 'domain: verify'
description: Überprüft den Besitz der Domäne.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be1eb96647fe78a9a796703ea67004f8fa4571cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972495"
---
# <a name="domain-verify"></a><span data-ttu-id="48b13-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="48b13-103">domain: verify</span></span>

<span data-ttu-id="48b13-104">Überprüft den Besitz der Domäne.</span><span class="sxs-lookup"><span data-stu-id="48b13-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="48b13-p101">**Wichtig:** Gilt nur für nicht überprüfte Domänen. Bei einer nicht überprüften Domäne hat die Eigenschaft „isVerified“ des [domain](../resources/domain.md)-Objekts den Wert „false“.</span><span class="sxs-lookup"><span data-stu-id="48b13-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="48b13-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48b13-107">Permissions</span></span>

<span data-ttu-id="48b13-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48b13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="48b13-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48b13-110">Permission type</span></span>      | <span data-ttu-id="48b13-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48b13-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48b13-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48b13-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48b13-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="48b13-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="48b13-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48b13-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48b13-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48b13-115">Not supported.</span></span>    |
|<span data-ttu-id="48b13-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48b13-116">Application</span></span> | <span data-ttu-id="48b13-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48b13-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48b13-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48b13-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="48b13-119">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="48b13-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48b13-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48b13-120">Request headers</span></span>

| <span data-ttu-id="48b13-121">Name</span><span class="sxs-lookup"><span data-stu-id="48b13-121">Name</span></span>       | <span data-ttu-id="48b13-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48b13-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48b13-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48b13-123">Authorization</span></span>  | <span data-ttu-id="48b13-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48b13-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="48b13-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48b13-126">Content-Type</span></span>  | <span data-ttu-id="48b13-127">application/json</span><span class="sxs-lookup"><span data-stu-id="48b13-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="48b13-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48b13-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="48b13-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="48b13-129">Response</span></span>

<span data-ttu-id="48b13-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48b13-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48b13-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48b13-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48b13-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48b13-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/{domain-name}/verify
```

##### <a name="response"></a><span data-ttu-id="48b13-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="48b13-133">Response</span></span>
<span data-ttu-id="48b13-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48b13-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "id": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
