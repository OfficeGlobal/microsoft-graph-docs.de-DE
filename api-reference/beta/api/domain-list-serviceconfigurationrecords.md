---
title: serviceConfigurationRecords auflisten
description: Dient zum Abrufen einer Liste von domainDnsRecord-Objekten, die erforderlich sind, um Dienste für die Domäne zu aktivieren.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: a68938b7eb5b2abed1a2d0476fdfeb5fdd783ec4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833719"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="f821c-103">serviceConfigurationRecords auflisten</span><span class="sxs-lookup"><span data-stu-id="f821c-103">List serviceConfigurationRecords</span></span>

> <span data-ttu-id="f821c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f821c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f821c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f821c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f821c-106">Dient zum Abrufen einer Liste von [domainDnsRecord](../resources/domaindnsrecord.md)-Objekten, die erforderlich sind, um Dienste für die Domäne zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f821c-106">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="f821c-p102">Verwenden Sie die zurückgegebene Liste, um der Zonendatei der Domäne Datensätze hinzufügen. Dies kann über die Domänenregistrierungsstelle oder die Konfiguration des DNS-Servers erfolgen.</span><span class="sxs-lookup"><span data-stu-id="f821c-p102">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="f821c-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f821c-109">Permissions</span></span>

<span data-ttu-id="f821c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f821c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f821c-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f821c-112">Permission type</span></span>      | <span data-ttu-id="f821c-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f821c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f821c-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f821c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f821c-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f821c-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="f821c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f821c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f821c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f821c-117">Not supported.</span></span>    |
|<span data-ttu-id="f821c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f821c-118">Application</span></span> | <span data-ttu-id="f821c-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f821c-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f821c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f821c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f821c-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f821c-121">Optional query parameters</span></span>

<span data-ttu-id="f821c-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f821c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f821c-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f821c-123">Request headers</span></span>

| <span data-ttu-id="f821c-124">Name</span><span class="sxs-lookup"><span data-stu-id="f821c-124">Name</span></span>      |<span data-ttu-id="f821c-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f821c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f821c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f821c-126">Authorization</span></span>  | <span data-ttu-id="f821c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f821c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f821c-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f821c-129">Content-Type</span></span>  | <span data-ttu-id="f821c-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f821c-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f821c-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f821c-131">Request body</span></span>

<span data-ttu-id="f821c-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f821c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f821c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f821c-133">Response</span></span>

<span data-ttu-id="f821c-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [domainDnsRecord](../resources/domaindnsrecord.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f821c-134">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f821c-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f821c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f821c-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f821c-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="f821c-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f821c-137">Response</span></span>
<span data-ttu-id="f821c-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f821c-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedServices": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
