---
title: Verträge auflisten
description: Mit dieser API können Sie eine Liste der einem Partnermandanten zugeordneten Objekte des Typs contract abrufen.
ms.openlocfilehash: ed2e7ea7c422372adc8377863713982cc3c688aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018524"
---
# <a name="list-contracts"></a><span data-ttu-id="b5e64-103">Verträge auflisten</span><span class="sxs-lookup"><span data-stu-id="b5e64-103">List contracts</span></span>

<span data-ttu-id="b5e64-104">Mit dieser API können Sie eine Liste der einem Partnermandanten zugeordneten Objekte des Typs [contract](../resources/contract.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="b5e64-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e64-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b5e64-105">Permissions</span></span>

<span data-ttu-id="b5e64-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b5e64-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5e64-108">Permission type</span></span>      | <span data-ttu-id="b5e64-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5e64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5e64-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5e64-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5e64-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5e64-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b5e64-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5e64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e64-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5e64-113">Not supported.</span></span>    |
|<span data-ttu-id="b5e64-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5e64-114">Application</span></span> | <span data-ttu-id="b5e64-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e64-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5e64-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5e64-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5e64-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b5e64-117">Optional query parameters</span></span>

<span data-ttu-id="b5e64-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5e64-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="b5e64-119">Für „customerId“, „defaultDomainName“ und „displayName“ wird Filterung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5e64-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5e64-120">Request headers</span></span>

| <span data-ttu-id="b5e64-121">Name</span><span class="sxs-lookup"><span data-stu-id="b5e64-121">Name</span></span>      |<span data-ttu-id="b5e64-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5e64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5e64-123">Authorization</span></span>  | <span data-ttu-id="b5e64-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5e64-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5e64-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5e64-126">Request body</span></span>

<span data-ttu-id="b5e64-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5e64-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5e64-128">Response</span></span>

<span data-ttu-id="b5e64-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contract](../resources/contract.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5e64-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5e64-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5e64-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5e64-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5e64-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="b5e64-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5e64-132">Response</span></span>

<span data-ttu-id="b5e64-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5e64-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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