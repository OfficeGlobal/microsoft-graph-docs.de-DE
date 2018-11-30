---
title: Liste privilegedApproval
description: Abrufen einer Liste von Privilegedapproval-Objekten.
ms.openlocfilehash: 69e558a734f86dd72b35e61d9f8ceab52b9f981e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064585"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="713c4-103">Liste privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="713c4-103">List privilegedApproval</span></span>

> <span data-ttu-id="713c4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="713c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="713c4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="713c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="713c4-106">Abrufen einer Liste von Privilegedapproval-Objekten.</span><span class="sxs-lookup"><span data-stu-id="713c4-106">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="713c4-107">Verwenden Sie zum Filtern der Ergebnisse der Abfrage, die standard-OData ``$filter`` Ausdrücke in die URIs.</span><span class="sxs-lookup"><span data-stu-id="713c4-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="713c4-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="713c4-108">Permissions</span></span>
<span data-ttu-id="713c4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="713c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="713c4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="713c4-111">Permission type</span></span>      | <span data-ttu-id="713c4-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="713c4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="713c4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="713c4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="713c4-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="713c4-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="713c4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="713c4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="713c4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="713c4-116">Not supported.</span></span>    |
|<span data-ttu-id="713c4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="713c4-117">Application</span></span> | <span data-ttu-id="713c4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="713c4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="713c4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="713c4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="713c4-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="713c4-120">Optional query parameters</span></span>
<span data-ttu-id="713c4-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="713c4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="713c4-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="713c4-122">Request headers</span></span>
| <span data-ttu-id="713c4-123">Name</span><span class="sxs-lookup"><span data-stu-id="713c4-123">Name</span></span>      |<span data-ttu-id="713c4-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="713c4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="713c4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="713c4-125">Authorization</span></span>  | <span data-ttu-id="713c4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="713c4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="713c4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="713c4-128">Request body</span></span>
<span data-ttu-id="713c4-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="713c4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="713c4-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="713c4-130">Response</span></span>

<span data-ttu-id="713c4-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [PrivilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="713c4-131">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="713c4-132">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="713c4-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="713c4-133">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="713c4-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="713c4-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="713c4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="713c4-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="713c4-135">Request</span></span>
<span data-ttu-id="713c4-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="713c4-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="713c4-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="713c4-137">Response</span></span>
<span data-ttu-id="713c4-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="713c4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
