---
title: Abrufen von groupLifecyclePolicy
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines groupLifecyclePolicies-Objekts abrufen.
ms.openlocfilehash: 10f8f3f5237ed3c7510019f2e8340b4ffa29cc94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059987"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="14515-103">Abrufen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="14515-103">Get groupLifecyclePolicy</span></span>

> <span data-ttu-id="14515-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="14515-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14515-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="14515-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14515-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="14515-106">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14515-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="14515-107">Permissions</span></span>

<span data-ttu-id="14515-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14515-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="14515-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="14515-110">Permission type</span></span>      | <span data-ttu-id="14515-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="14515-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14515-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="14515-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14515-113">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14515-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="14515-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="14515-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14515-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14515-115">Not supported</span></span> |
|<span data-ttu-id="14515-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="14515-116">Application</span></span> | <span data-ttu-id="14515-117">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14515-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14515-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="14515-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14515-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="14515-119">Optional query parameters</span></span>
<span data-ttu-id="14515-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="14515-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14515-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="14515-121">Request headers</span></span>
| <span data-ttu-id="14515-122">Name</span><span class="sxs-lookup"><span data-stu-id="14515-122">Name</span></span> | <span data-ttu-id="14515-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14515-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="14515-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14515-124">Authorization</span></span> | <span data-ttu-id="14515-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="14515-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14515-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="14515-127">Request body</span></span>
<span data-ttu-id="14515-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="14515-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="14515-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="14515-129">Response</span></span>
<span data-ttu-id="14515-130">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und ein [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="14515-130">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14515-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="14515-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="14515-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="14515-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="14515-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="14515-133">Response</span></span>

<span data-ttu-id="14515-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14515-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->