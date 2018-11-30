---
title: Verträge auflisten
description: Mit dieser API können Sie eine Liste der einem Partnermandanten zugeordneten Objekte des Typs contract abrufen.
ms.openlocfilehash: 41e30880bded985695581e7d1402a24d2353e07e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059581"
---
# <a name="list-contracts"></a><span data-ttu-id="523ee-103">Verträge auflisten</span><span class="sxs-lookup"><span data-stu-id="523ee-103">List contracts</span></span>

> <span data-ttu-id="523ee-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="523ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="523ee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="523ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="523ee-106">Mit dieser API können Sie eine Liste der einem Partnermandanten zugeordneten Objekte des Typs [contract](../resources/contract.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="523ee-106">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="523ee-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="523ee-107">Permissions</span></span>

<span data-ttu-id="523ee-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="523ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="523ee-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="523ee-110">Permission type</span></span>      | <span data-ttu-id="523ee-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="523ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="523ee-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="523ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="523ee-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="523ee-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="523ee-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="523ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="523ee-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="523ee-115">Not supported.</span></span>    |
|<span data-ttu-id="523ee-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="523ee-116">Application</span></span> | <span data-ttu-id="523ee-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="523ee-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="523ee-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="523ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="523ee-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="523ee-119">Optional query parameters</span></span>

<span data-ttu-id="523ee-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="523ee-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="523ee-121">Für „customerId“, „defaultDomainName“ und „displayName“ wird Filterung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="523ee-121">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="523ee-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="523ee-122">Request headers</span></span>

| <span data-ttu-id="523ee-123">Name</span><span class="sxs-lookup"><span data-stu-id="523ee-123">Name</span></span>      |<span data-ttu-id="523ee-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="523ee-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="523ee-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="523ee-125">Authorization</span></span>  | <span data-ttu-id="523ee-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="523ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="523ee-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="523ee-128">Request body</span></span>

<span data-ttu-id="523ee-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="523ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="523ee-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="523ee-130">Response</span></span>

<span data-ttu-id="523ee-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contract](../resources/contract.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="523ee-131">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="523ee-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="523ee-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="523ee-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="523ee-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts
```

##### <a name="response"></a><span data-ttu-id="523ee-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="523ee-134">Response</span></span>

<span data-ttu-id="523ee-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="523ee-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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