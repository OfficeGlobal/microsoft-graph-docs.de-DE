---
title: Auflisten von groupLifecyclePolicies
description: Ruft eine Liste der groupLifecyclePolicy-Objekte ab, zu der eine Gruppe gehört.
author: dkershaw10
ms.openlocfilehash: f70a0d868241d17513249902e838e237771f17be
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323758"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="dae89-103">Auflisten von groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="dae89-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="dae89-104">Ruft eine Liste der [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekte ab, zu der eine Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="dae89-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="dae89-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dae89-105">Permissions</span></span>

<span data-ttu-id="dae89-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dae89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dae89-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dae89-108">Permission type</span></span>      | <span data-ttu-id="dae89-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dae89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dae89-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dae89-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dae89-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dae89-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="dae89-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dae89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dae89-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dae89-113">Not supported.</span></span>    |
|<span data-ttu-id="dae89-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dae89-114">Application</span></span> | <span data-ttu-id="dae89-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dae89-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dae89-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dae89-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dae89-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="dae89-117">Optional query parameters</span></span>
<span data-ttu-id="dae89-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dae89-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dae89-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dae89-119">Request headers</span></span>
| <span data-ttu-id="dae89-120">Name</span><span class="sxs-lookup"><span data-stu-id="dae89-120">Name</span></span> | <span data-ttu-id="dae89-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dae89-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="dae89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dae89-122">Authorization</span></span> | <span data-ttu-id="dae89-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dae89-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dae89-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dae89-125">Request body</span></span>
<span data-ttu-id="dae89-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dae89-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dae89-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="dae89-127">Response</span></span>
<span data-ttu-id="dae89-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dae89-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dae89-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dae89-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dae89-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dae89-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="dae89-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="dae89-131">Response</span></span>

<span data-ttu-id="dae89-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dae89-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
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