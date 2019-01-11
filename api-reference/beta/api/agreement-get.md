---
title: Abrufen der Vereinbarung
description: Rufen Sie die Eigenschaften und die Beziehungen eines Vereinbarung-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: 0ca4e941705fe716c3aa11a73c934c40deb279d4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818655"
---
# <a name="get-agreement"></a><span data-ttu-id="d170b-103">Abrufen der Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="d170b-103">Get agreement</span></span>

> <span data-ttu-id="d170b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d170b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d170b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d170b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d170b-106">Rufen Sie die Eigenschaften und die Beziehungen eines [Vereinbarung](../resources/agreement.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="d170b-106">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d170b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d170b-107">Permissions</span></span>
<span data-ttu-id="d170b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d170b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d170b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d170b-110">Permission type</span></span>                        | <span data-ttu-id="d170b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d170b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d170b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d170b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d170b-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="d170b-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="d170b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d170b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d170b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d170b-115">Not supported.</span></span> |
|<span data-ttu-id="d170b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d170b-116">Application</span></span>                            | <span data-ttu-id="d170b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d170b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d170b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d170b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="d170b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d170b-119">Request headers</span></span>
| <span data-ttu-id="d170b-120">Name</span><span class="sxs-lookup"><span data-stu-id="d170b-120">Name</span></span>         | <span data-ttu-id="d170b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d170b-121">Type</span></span>        | <span data-ttu-id="d170b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d170b-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d170b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d170b-123">Authorization</span></span> | <span data-ttu-id="d170b-124">string</span><span class="sxs-lookup"><span data-stu-id="d170b-124">string</span></span> | <span data-ttu-id="d170b-125">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="d170b-125">Bearer \{token\}.</span></span> <span data-ttu-id="d170b-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d170b-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d170b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d170b-127">Request body</span></span>
<span data-ttu-id="d170b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d170b-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d170b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d170b-129">Response</span></span>
<span data-ttu-id="d170b-130">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortobjekt Code und [Vereinbarung](../resources/agreement.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d170b-130">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d170b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d170b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d170b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d170b-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="d170b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d170b-133">Response</span></span>
><span data-ttu-id="d170b-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d170b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
