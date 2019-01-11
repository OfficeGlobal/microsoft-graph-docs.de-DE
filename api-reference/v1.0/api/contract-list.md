---
title: Verträge auflisten
description: Mit dieser API können Sie eine Liste der einem Partnermandanten zugeordneten Objekte des Typs contract abrufen.
localization_priority: Normal
ms.openlocfilehash: 69fdb62c7e3a89f8e4ebff5065a20ec8334bad88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821000"
---
# <a name="list-contracts"></a><span data-ttu-id="270fa-103">Verträge auflisten</span><span class="sxs-lookup"><span data-stu-id="270fa-103">List contracts</span></span>

<span data-ttu-id="270fa-104">Mit dieser API können Sie eine Liste der einem Partnermandanten zugeordneten Objekte des Typs [contract](../resources/contract.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="270fa-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="270fa-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="270fa-105">Permissions</span></span>

<span data-ttu-id="270fa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="270fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="270fa-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="270fa-108">Permission type</span></span>      | <span data-ttu-id="270fa-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="270fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="270fa-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="270fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="270fa-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="270fa-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="270fa-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="270fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="270fa-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="270fa-113">Not supported.</span></span>    |
|<span data-ttu-id="270fa-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="270fa-114">Application</span></span> | <span data-ttu-id="270fa-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270fa-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="270fa-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="270fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="270fa-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="270fa-117">Optional query parameters</span></span>

<span data-ttu-id="270fa-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="270fa-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="270fa-119">Für „customerId“, „defaultDomainName“ und „displayName“ wird Filterung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="270fa-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="270fa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="270fa-120">Request headers</span></span>

| <span data-ttu-id="270fa-121">Name</span><span class="sxs-lookup"><span data-stu-id="270fa-121">Name</span></span>      |<span data-ttu-id="270fa-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="270fa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="270fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="270fa-123">Authorization</span></span>  | <span data-ttu-id="270fa-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="270fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="270fa-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="270fa-126">Request body</span></span>

<span data-ttu-id="270fa-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="270fa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="270fa-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="270fa-128">Response</span></span>

<span data-ttu-id="270fa-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contract](../resources/contract.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="270fa-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="270fa-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="270fa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="270fa-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="270fa-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="270fa-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="270fa-132">Response</span></span>

<span data-ttu-id="270fa-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="270fa-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
