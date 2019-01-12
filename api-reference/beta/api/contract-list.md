---
title: Verträge auflisten
description: Mit dieser API können Sie eine Liste der einem Partnermandanten zugeordneten Objekte des Typs contract abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6df390cbe742443bf8a996362fa2cf2909ef83f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971074"
---
# <a name="list-contracts"></a><span data-ttu-id="c0de6-103">Verträge auflisten</span><span class="sxs-lookup"><span data-stu-id="c0de6-103">List contracts</span></span>

> <span data-ttu-id="c0de6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0de6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0de6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0de6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0de6-106">Mit dieser API können Sie eine Liste der einem Partnermandanten zugeordneten Objekte des Typs [contract](../resources/contract.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="c0de6-106">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0de6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c0de6-107">Permissions</span></span>

<span data-ttu-id="c0de6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0de6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c0de6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0de6-110">Permission type</span></span>      | <span data-ttu-id="c0de6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0de6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0de6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0de6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0de6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0de6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0de6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0de6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0de6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0de6-115">Not supported.</span></span>    |
|<span data-ttu-id="c0de6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0de6-116">Application</span></span> | <span data-ttu-id="c0de6-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0de6-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0de6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0de6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0de6-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c0de6-119">Optional query parameters</span></span>

<span data-ttu-id="c0de6-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c0de6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="c0de6-121">Für „customerId“, „defaultDomainName“ und „displayName“ wird Filterung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0de6-121">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0de6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0de6-122">Request headers</span></span>

| <span data-ttu-id="c0de6-123">Name</span><span class="sxs-lookup"><span data-stu-id="c0de6-123">Name</span></span>      |<span data-ttu-id="c0de6-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0de6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0de6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0de6-125">Authorization</span></span>  | <span data-ttu-id="c0de6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0de6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0de6-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0de6-128">Request body</span></span>

<span data-ttu-id="c0de6-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c0de6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0de6-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0de6-130">Response</span></span>

<span data-ttu-id="c0de6-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contract](../resources/contract.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0de6-131">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0de6-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0de6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0de6-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0de6-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts
```

##### <a name="response"></a><span data-ttu-id="c0de6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0de6-134">Response</span></span>

<span data-ttu-id="c0de6-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0de6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
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
