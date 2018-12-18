---
title: Auflisten von groupLifecyclePolicies
description: Listet alle groupLifecyclePolicies auf.
author: dkershaw10
ms.openlocfilehash: dade0f0a11670c5ecb5eeb6626d479b4d4c4be63
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349231"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="be287-103">Auflisten von groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="be287-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="be287-104">Listet alle [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="be287-104">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="be287-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be287-105">Permissions</span></span>

<span data-ttu-id="be287-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="be287-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be287-108">Permission type</span></span>      | <span data-ttu-id="be287-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be287-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be287-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be287-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be287-111">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be287-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="be287-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be287-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be287-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be287-113">Not supported.</span></span>    |
|<span data-ttu-id="be287-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be287-114">Application</span></span> | <span data-ttu-id="be287-115">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be287-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be287-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be287-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be287-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="be287-117">Optional query parameters</span></span>
<span data-ttu-id="be287-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be287-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be287-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be287-119">Request headers</span></span>
| <span data-ttu-id="be287-120">Name</span><span class="sxs-lookup"><span data-stu-id="be287-120">Name</span></span> | <span data-ttu-id="be287-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be287-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="be287-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be287-122">Authorization</span></span> | <span data-ttu-id="be287-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="be287-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be287-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be287-125">Request body</span></span>
<span data-ttu-id="be287-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="be287-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be287-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="be287-127">Response</span></span>

<span data-ttu-id="be287-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="be287-128">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be287-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be287-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="be287-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be287-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="be287-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="be287-131">Response</span></span>

<span data-ttu-id="be287-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be287-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 223

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->