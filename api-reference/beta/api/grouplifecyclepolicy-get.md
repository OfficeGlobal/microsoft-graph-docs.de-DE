---
title: Abrufen von groupLifecyclePolicy
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines groupLifecyclePolicies-Objekts abrufen.
author: dkershaw10
ms.openlocfilehash: ef239385766b33c4a03576200c6c9abf3938c25a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312523"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="ecf3d-103">Abrufen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ecf3d-103">Get groupLifecyclePolicy</span></span>

> <span data-ttu-id="ecf3d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ecf3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecf3d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ecf3d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ecf3d-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="ecf3d-106">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecf3d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ecf3d-107">Permissions</span></span>

<span data-ttu-id="ecf3d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecf3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ecf3d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ecf3d-110">Permission type</span></span>      | <span data-ttu-id="ecf3d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ecf3d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecf3d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ecf3d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ecf3d-113">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecf3d-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ecf3d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ecf3d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecf3d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ecf3d-115">Not supported</span></span> |
|<span data-ttu-id="ecf3d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ecf3d-116">Application</span></span> | <span data-ttu-id="ecf3d-117">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecf3d-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecf3d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecf3d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ecf3d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ecf3d-119">Optional query parameters</span></span>
<span data-ttu-id="ecf3d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ecf3d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecf3d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ecf3d-121">Request headers</span></span>
| <span data-ttu-id="ecf3d-122">Name</span><span class="sxs-lookup"><span data-stu-id="ecf3d-122">Name</span></span> | <span data-ttu-id="ecf3d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ecf3d-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="ecf3d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecf3d-124">Authorization</span></span> | <span data-ttu-id="ecf3d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ecf3d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecf3d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ecf3d-127">Request body</span></span>
<span data-ttu-id="ecf3d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ecf3d-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ecf3d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecf3d-129">Response</span></span>
<span data-ttu-id="ecf3d-130">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und ein [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ecf3d-130">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ecf3d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ecf3d-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ecf3d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecf3d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="ecf3d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecf3d-133">Response</span></span>

<span data-ttu-id="ecf3d-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ecf3d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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