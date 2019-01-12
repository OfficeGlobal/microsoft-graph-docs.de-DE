---
title: Abrufen von groupLifecyclePolicy
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines groupLifecyclePolicies-Objekts abrufen.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0b4d29ca8a08c2ec805549e6f10da4ac268771a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917930"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="f713c-103">Abrufen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f713c-103">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="f713c-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="f713c-104">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f713c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f713c-105">Permissions</span></span>

<span data-ttu-id="f713c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f713c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f713c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f713c-108">Permission type</span></span>      | <span data-ttu-id="f713c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f713c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f713c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f713c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f713c-111">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f713c-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="f713c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f713c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f713c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f713c-113">Not supported.</span></span>    |
|<span data-ttu-id="f713c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f713c-114">Application</span></span> | <span data-ttu-id="f713c-115">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f713c-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f713c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f713c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f713c-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f713c-117">Optional query parameters</span></span>
<span data-ttu-id="f713c-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f713c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f713c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f713c-119">Request headers</span></span>
| <span data-ttu-id="f713c-120">Name</span><span class="sxs-lookup"><span data-stu-id="f713c-120">Name</span></span> | <span data-ttu-id="f713c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f713c-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="f713c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f713c-122">Authorization</span></span> | <span data-ttu-id="f713c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f713c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f713c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f713c-125">Request body</span></span>
<span data-ttu-id="f713c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f713c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f713c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f713c-127">Response</span></span>
<span data-ttu-id="f713c-128">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und ein [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f713c-128">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f713c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f713c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f713c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f713c-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="f713c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f713c-131">Response</span></span>

<span data-ttu-id="f713c-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f713c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
