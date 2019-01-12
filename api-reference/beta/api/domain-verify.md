---
title: 'domain: verify'
description: Überprüft den Besitz der Domäne.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e61456ccf7e47283464bddb4103a02dbfdb9bdb3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950627"
---
# <a name="domain-verify"></a><span data-ttu-id="c478a-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="c478a-103">domain: verify</span></span>

> <span data-ttu-id="c478a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c478a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c478a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c478a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c478a-106">Überprüft den Besitz der Domäne.</span><span class="sxs-lookup"><span data-stu-id="c478a-106">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="c478a-p102">**Wichtig:** Gilt nur für nicht überprüfte Domänen. Bei einer nicht überprüften Domäne hat die Eigenschaft „isVerified“ des [domain](../resources/domain.md)-Objekts den Wert „false“.</span><span class="sxs-lookup"><span data-stu-id="c478a-p102">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="c478a-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c478a-109">Permissions</span></span>

<span data-ttu-id="c478a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c478a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c478a-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c478a-112">Permission type</span></span>      | <span data-ttu-id="c478a-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c478a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c478a-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c478a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c478a-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c478a-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="c478a-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c478a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c478a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c478a-117">Not supported.</span></span>    |
|<span data-ttu-id="c478a-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c478a-118">Application</span></span> | <span data-ttu-id="c478a-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c478a-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c478a-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c478a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="c478a-121">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="c478a-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c478a-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c478a-122">Request headers</span></span>

| <span data-ttu-id="c478a-123">Name</span><span class="sxs-lookup"><span data-stu-id="c478a-123">Name</span></span>       | <span data-ttu-id="c478a-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c478a-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c478a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c478a-125">Authorization</span></span>  | <span data-ttu-id="c478a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c478a-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c478a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c478a-128">Content-Type</span></span>  | <span data-ttu-id="c478a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c478a-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c478a-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c478a-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c478a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c478a-131">Response</span></span>

<span data-ttu-id="c478a-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c478a-132">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c478a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c478a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c478a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c478a-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="c478a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c478a-135">Response</span></span>
<span data-ttu-id="c478a-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c478a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "name": "contoso.com"
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
