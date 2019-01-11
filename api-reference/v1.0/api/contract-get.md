---
title: Vertrag abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs contract abrufen.
localization_priority: Normal
ms.openlocfilehash: dd379286e161cc68e33af49bec20bb580512ef0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805775"
---
# <a name="get-contract"></a><span data-ttu-id="19d78-103">Vertrag abrufen</span><span class="sxs-lookup"><span data-stu-id="19d78-103">Get Contract</span></span>

<span data-ttu-id="19d78-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [contract](../resources/contract.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="19d78-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="19d78-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="19d78-105">Permissions</span></span>

<span data-ttu-id="19d78-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19d78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="19d78-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19d78-108">Permission type</span></span>      | <span data-ttu-id="19d78-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19d78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19d78-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19d78-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19d78-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19d78-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19d78-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19d78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19d78-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19d78-113">Not supported.</span></span>    |
|<span data-ttu-id="19d78-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19d78-114">Application</span></span> | <span data-ttu-id="19d78-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19d78-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19d78-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19d78-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19d78-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="19d78-117">Optional query parameters</span></span>

<span data-ttu-id="19d78-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="19d78-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19d78-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19d78-119">Request headers</span></span>

| <span data-ttu-id="19d78-120">Name</span><span class="sxs-lookup"><span data-stu-id="19d78-120">Name</span></span>      |<span data-ttu-id="19d78-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19d78-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19d78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19d78-122">Authorization</span></span>  | <span data-ttu-id="19d78-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="19d78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19d78-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19d78-125">Request body</span></span>

<span data-ttu-id="19d78-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="19d78-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19d78-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="19d78-127">Response</span></span>

<span data-ttu-id="19d78-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contract](../resources/contract.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19d78-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19d78-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19d78-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19d78-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19d78-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="19d78-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="19d78-131">Response</span></span>
<span data-ttu-id="19d78-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19d78-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
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
