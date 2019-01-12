---
title: Auflisten von groupLifecyclePolicies
description: Ruft eine Liste der groupLifecyclePolicy-Objekte ab, zu der eine Gruppe gehört.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3a569c2c82205b59eda127f06a7cbef8fde17eed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985319"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="16cee-103">Auflisten von groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="16cee-103">List groupLifecyclePolicies</span></span>

> <span data-ttu-id="16cee-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16cee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16cee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16cee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16cee-106">Ruft eine Liste der [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekte ab, zu der eine Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="16cee-106">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="16cee-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="16cee-107">Permissions</span></span>

<span data-ttu-id="16cee-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16cee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16cee-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16cee-110">Permission type</span></span>      | <span data-ttu-id="16cee-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16cee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16cee-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16cee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16cee-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="16cee-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="16cee-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16cee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16cee-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16cee-115">Not supported.</span></span>    |
|<span data-ttu-id="16cee-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16cee-116">Application</span></span> | <span data-ttu-id="16cee-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="16cee-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16cee-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16cee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16cee-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="16cee-119">Optional query parameters</span></span>
<span data-ttu-id="16cee-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="16cee-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16cee-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16cee-121">Request headers</span></span>
| <span data-ttu-id="16cee-122">Name</span><span class="sxs-lookup"><span data-stu-id="16cee-122">Name</span></span> | <span data-ttu-id="16cee-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16cee-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="16cee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="16cee-124">Authorization</span></span> | <span data-ttu-id="16cee-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16cee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16cee-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="16cee-127">Request body</span></span>
<span data-ttu-id="16cee-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="16cee-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="16cee-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="16cee-129">Response</span></span>
<span data-ttu-id="16cee-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="16cee-130">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16cee-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16cee-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="16cee-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16cee-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="16cee-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="16cee-133">Response</span></span>

<span data-ttu-id="16cee-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16cee-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 227

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
