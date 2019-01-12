---
title: Vertrag abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs contract abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 86bf035bf015aa85a47c3f5cad62ef497c12e99a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916670"
---
# <a name="get-contract"></a><span data-ttu-id="46e81-103">Vertrag abrufen</span><span class="sxs-lookup"><span data-stu-id="46e81-103">Get Contract</span></span>

> <span data-ttu-id="46e81-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="46e81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46e81-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46e81-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46e81-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [contract](../resources/contract.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="46e81-106">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46e81-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="46e81-107">Permissions</span></span>

<span data-ttu-id="46e81-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46e81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="46e81-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46e81-110">Permission type</span></span>      | <span data-ttu-id="46e81-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46e81-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46e81-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46e81-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46e81-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46e81-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="46e81-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46e81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46e81-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46e81-115">Not supported.</span></span>    |
|<span data-ttu-id="46e81-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46e81-116">Application</span></span> | <span data-ttu-id="46e81-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e81-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46e81-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46e81-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46e81-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="46e81-119">Optional query parameters</span></span>

<span data-ttu-id="46e81-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="46e81-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46e81-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46e81-121">Request headers</span></span>

| <span data-ttu-id="46e81-122">Name</span><span class="sxs-lookup"><span data-stu-id="46e81-122">Name</span></span>      |<span data-ttu-id="46e81-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46e81-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46e81-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="46e81-124">Authorization</span></span>  | <span data-ttu-id="46e81-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="46e81-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46e81-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46e81-127">Request body</span></span>

<span data-ttu-id="46e81-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="46e81-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46e81-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="46e81-129">Response</span></span>

<span data-ttu-id="46e81-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contract](../resources/contract.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46e81-130">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46e81-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46e81-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46e81-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46e81-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="46e81-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="46e81-133">Response</span></span>
<span data-ttu-id="46e81-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46e81-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
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
