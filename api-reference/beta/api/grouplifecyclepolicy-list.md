---
title: Auflisten von groupLifecyclePolicies
description: Listet alle groupLifecyclePolicies auf.
author: dkershaw10
ms.openlocfilehash: e926d071121986e1aa06511ef8ec84e6b0cd55b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350330"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="89e0f-103">Auflisten von groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="89e0f-103">List groupLifecyclePolicies</span></span>

> <span data-ttu-id="89e0f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="89e0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89e0f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="89e0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89e0f-106">Listet alle [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="89e0f-106">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89e0f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="89e0f-107">Permissions</span></span>

<span data-ttu-id="89e0f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89e0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="89e0f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89e0f-110">Permission type</span></span>      | <span data-ttu-id="89e0f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89e0f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89e0f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89e0f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89e0f-113">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e0f-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="89e0f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89e0f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89e0f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89e0f-115">Not supported</span></span> |
|<span data-ttu-id="89e0f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89e0f-116">Application</span></span> | <span data-ttu-id="89e0f-117">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e0f-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89e0f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89e0f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89e0f-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="89e0f-119">Optional query parameters</span></span>
<span data-ttu-id="89e0f-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="89e0f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89e0f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89e0f-121">Request headers</span></span>
| <span data-ttu-id="89e0f-122">Name</span><span class="sxs-lookup"><span data-stu-id="89e0f-122">Name</span></span> | <span data-ttu-id="89e0f-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89e0f-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="89e0f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="89e0f-124">Authorization</span></span> | <span data-ttu-id="89e0f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="89e0f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89e0f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89e0f-127">Request body</span></span>
<span data-ttu-id="89e0f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="89e0f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89e0f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="89e0f-129">Response</span></span>

<span data-ttu-id="89e0f-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="89e0f-130">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89e0f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89e0f-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="89e0f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89e0f-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="89e0f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="89e0f-133">Response</span></span>

<span data-ttu-id="89e0f-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89e0f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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