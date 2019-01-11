---
title: Auflisten von groupLifecyclePolicies
description: Listet alle groupLifecyclePolicies auf.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: da0251e044912c4ee5b107f7ec0c7e052ddb0046
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864442"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="3eb08-103">Auflisten von groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="3eb08-103">List groupLifecyclePolicies</span></span>

> <span data-ttu-id="3eb08-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3eb08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eb08-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3eb08-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3eb08-106">Listet alle [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="3eb08-106">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3eb08-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3eb08-107">Permissions</span></span>

<span data-ttu-id="3eb08-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3eb08-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3eb08-110">Permission type</span></span>      | <span data-ttu-id="3eb08-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3eb08-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eb08-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3eb08-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3eb08-113">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb08-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="3eb08-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3eb08-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eb08-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3eb08-115">Not supported</span></span> |
|<span data-ttu-id="3eb08-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3eb08-116">Application</span></span> | <span data-ttu-id="3eb08-117">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb08-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3eb08-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3eb08-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3eb08-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3eb08-119">Optional query parameters</span></span>
<span data-ttu-id="3eb08-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3eb08-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3eb08-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3eb08-121">Request headers</span></span>
| <span data-ttu-id="3eb08-122">Name</span><span class="sxs-lookup"><span data-stu-id="3eb08-122">Name</span></span> | <span data-ttu-id="3eb08-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3eb08-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="3eb08-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eb08-124">Authorization</span></span> | <span data-ttu-id="3eb08-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3eb08-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3eb08-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3eb08-127">Request body</span></span>
<span data-ttu-id="3eb08-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3eb08-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eb08-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3eb08-129">Response</span></span>

<span data-ttu-id="3eb08-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3eb08-130">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb08-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3eb08-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3eb08-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3eb08-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="3eb08-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="3eb08-133">Response</span></span>

<span data-ttu-id="3eb08-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3eb08-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
