---
title: Vertrag abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs contract abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba6ba3dd1e0dc631f5aeb61dd6d714e9d7a81bb6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917426"
---
# <a name="get-contract"></a><span data-ttu-id="f7dc2-103">Vertrag abrufen</span><span class="sxs-lookup"><span data-stu-id="f7dc2-103">Get Contract</span></span>

<span data-ttu-id="f7dc2-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [contract](../resources/contract.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="f7dc2-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7dc2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7dc2-105">Permissions</span></span>

<span data-ttu-id="f7dc2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7dc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f7dc2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7dc2-108">Permission type</span></span>      | <span data-ttu-id="f7dc2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7dc2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7dc2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7dc2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7dc2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7dc2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f7dc2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7dc2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7dc2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7dc2-113">Not supported.</span></span>    |
|<span data-ttu-id="f7dc2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7dc2-114">Application</span></span> | <span data-ttu-id="f7dc2-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7dc2-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7dc2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7dc2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7dc2-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f7dc2-117">Optional query parameters</span></span>

<span data-ttu-id="f7dc2-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7dc2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7dc2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7dc2-119">Request headers</span></span>

| <span data-ttu-id="f7dc2-120">Name</span><span class="sxs-lookup"><span data-stu-id="f7dc2-120">Name</span></span>      |<span data-ttu-id="f7dc2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7dc2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7dc2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7dc2-122">Authorization</span></span>  | <span data-ttu-id="f7dc2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f7dc2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7dc2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7dc2-125">Request body</span></span>

<span data-ttu-id="f7dc2-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f7dc2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7dc2-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7dc2-127">Response</span></span>

<span data-ttu-id="f7dc2-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contract](../resources/contract.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7dc2-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7dc2-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7dc2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7dc2-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7dc2-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="f7dc2-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7dc2-131">Response</span></span>
<span data-ttu-id="f7dc2-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7dc2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
