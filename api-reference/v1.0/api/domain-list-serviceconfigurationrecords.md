---
title: serviceConfigurationRecords auflisten
description: Dient zum Abrufen einer Liste von domainDnsRecord-Objekten, die erforderlich sind, um Dienste für die Domäne zu aktivieren.
ms.openlocfilehash: 92cc0695fa4128fcd32a59aee210fc63a35ac412
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016496"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="c0f95-103">serviceConfigurationRecords auflisten</span><span class="sxs-lookup"><span data-stu-id="c0f95-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="c0f95-104">Dient zum Abrufen einer Liste von [domainDnsRecord](../resources/domaindnsrecord.md)-Objekten, die erforderlich sind, um Dienste für die Domäne zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="c0f95-104">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="c0f95-p101">Verwenden Sie die zurückgegebene Liste, um der Zonendatei der Domäne Datensätze hinzufügen. Dies kann über die Domänenregistrierungsstelle oder die Konfiguration des DNS-Servers erfolgen.</span><span class="sxs-lookup"><span data-stu-id="c0f95-p101">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0f95-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c0f95-107">Permissions</span></span>

<span data-ttu-id="c0f95-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0f95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c0f95-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0f95-110">Permission type</span></span>      | <span data-ttu-id="c0f95-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0f95-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0f95-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0f95-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0f95-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f95-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="c0f95-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0f95-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0f95-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0f95-115">Not supported.</span></span>    |
|<span data-ttu-id="c0f95-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0f95-116">Application</span></span> | <span data-ttu-id="c0f95-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0f95-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0f95-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0f95-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0f95-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c0f95-119">Optional query parameters</span></span>

<span data-ttu-id="c0f95-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c0f95-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0f95-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0f95-121">Request headers</span></span>

| <span data-ttu-id="c0f95-122">Name</span><span class="sxs-lookup"><span data-stu-id="c0f95-122">Name</span></span>      |<span data-ttu-id="c0f95-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0f95-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0f95-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0f95-124">Authorization</span></span>  | <span data-ttu-id="c0f95-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0f95-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0f95-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0f95-127">Content-Type</span></span>  | <span data-ttu-id="c0f95-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c0f95-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0f95-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0f95-129">Request body</span></span>

<span data-ttu-id="c0f95-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c0f95-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0f95-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0f95-131">Response</span></span>

<span data-ttu-id="c0f95-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [domainDnsRecord](../resources/domaindnsrecord.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0f95-132">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0f95-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0f95-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0f95-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0f95-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="c0f95-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0f95-135">Response</span></span>
<span data-ttu-id="c0f95-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0f95-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type":"microsoft.graph.domainDnsMxRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "@odata.type":"microsoft.graph.domainDnsTxtRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedService": "Email",
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