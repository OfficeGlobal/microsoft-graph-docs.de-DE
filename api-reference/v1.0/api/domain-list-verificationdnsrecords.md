---
title: verificationDnsRecords auflisten
description: Dient zum Abrufen einer Liste von domainDnsRecord-Objekten.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 48549b2020bb4e73169712f9d8ba6b8034187082
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850589"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="7ad3f-103">verificationDnsRecords auflisten</span><span class="sxs-lookup"><span data-stu-id="7ad3f-103">List verificationDnsRecords</span></span>

<span data-ttu-id="7ad3f-104">Dient zum Abrufen einer Liste von [domainDnsRecord](../resources/domaindnsrecord.md)-Objekten.</span><span class="sxs-lookup"><span data-stu-id="7ad3f-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="7ad3f-p101">Sie können eine zugeordnete Domäne erst dann mit Ihrem Azure AD-Mandanten verwenden, nachdem der Besitz überprüft wurde. Um den Besitz der Domäne zu überprüfen, rufen Sie die Domänenüberprüfungseinträge ab, und fügen Sie die Details zur Zonendatei der Domäne hinzu. Dies kann über die Domänenregistrierungsstelle oder die Konfiguration des DNS-Servers erfolgen.</span><span class="sxs-lookup"><span data-stu-id="7ad3f-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="7ad3f-p102">Stammdomänen erfordern eine Überprüfung. Beispielsweise muss „contoso.com“ überprüft werden. Wenn eine Stammdomäne überprüft wird, werden Unterdomänen der Stammdomäne automatisch überprüft. Beispielsweise wird „subdomain.contoso.com“ automatisch überprüft, wenn „contoso.com“ überprüft wurde.</span><span class="sxs-lookup"><span data-stu-id="7ad3f-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ad3f-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7ad3f-112">Permissions</span></span>

<span data-ttu-id="7ad3f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ad3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ad3f-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ad3f-115">Permission type</span></span>      | <span data-ttu-id="7ad3f-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ad3f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ad3f-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ad3f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7ad3f-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ad3f-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="7ad3f-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ad3f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ad3f-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ad3f-120">Not supported.</span></span>    |
|<span data-ttu-id="7ad3f-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ad3f-121">Application</span></span> | <span data-ttu-id="7ad3f-122">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ad3f-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ad3f-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad3f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="7ad3f-124">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="7ad3f-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7ad3f-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7ad3f-125">Optional query parameters</span></span>

<span data-ttu-id="7ad3f-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ad3f-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ad3f-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ad3f-127">Request headers</span></span>

| <span data-ttu-id="7ad3f-128">Name</span><span class="sxs-lookup"><span data-stu-id="7ad3f-128">Name</span></span>      |<span data-ttu-id="7ad3f-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ad3f-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ad3f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ad3f-130">Authorization</span></span>  | <span data-ttu-id="7ad3f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ad3f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ad3f-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ad3f-133">Content-Type</span></span>  | <span data-ttu-id="7ad3f-134">application/json</span><span class="sxs-lookup"><span data-stu-id="7ad3f-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ad3f-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ad3f-135">Request body</span></span>

<span data-ttu-id="7ad3f-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7ad3f-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ad3f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad3f-137">Response</span></span>

<span data-ttu-id="7ad3f-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [domainDnsRecord](../resources/domaindnsrecord.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ad3f-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ad3f-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ad3f-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ad3f-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad3f-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="7ad3f-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad3f-141">Response</span></span>

<span data-ttu-id="7ad3f-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ad3f-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
