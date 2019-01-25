---
title: Liste privilegedApproval
description: Abrufen einer Liste von Privilegedapproval-Objekten.
localization_priority: Normal
ms.openlocfilehash: ab3a3c2670cd0ddebf8415e112305679c1d3446c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521551"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="2d72d-103">Liste privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2d72d-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d72d-104">Abrufen einer Liste von Privilegedapproval-Objekten.</span><span class="sxs-lookup"><span data-stu-id="2d72d-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="2d72d-105">Verwenden Sie zum Filtern der Ergebnisse der Abfrage, die standard-OData ``$filter`` Ausdrücke in die URIs.</span><span class="sxs-lookup"><span data-stu-id="2d72d-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d72d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2d72d-106">Permissions</span></span>
<span data-ttu-id="2d72d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d72d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2d72d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d72d-109">Permission type</span></span>      | <span data-ttu-id="2d72d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d72d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d72d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d72d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d72d-112">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2d72d-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2d72d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d72d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d72d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d72d-114">Not supported.</span></span>    |
|<span data-ttu-id="2d72d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d72d-115">Application</span></span> | <span data-ttu-id="2d72d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d72d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d72d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d72d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d72d-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2d72d-118">Optional query parameters</span></span>
<span data-ttu-id="2d72d-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d72d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d72d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d72d-120">Request headers</span></span>
| <span data-ttu-id="2d72d-121">Name</span><span class="sxs-lookup"><span data-stu-id="2d72d-121">Name</span></span>      |<span data-ttu-id="2d72d-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d72d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2d72d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d72d-123">Authorization</span></span>  | <span data-ttu-id="2d72d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d72d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d72d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d72d-126">Request body</span></span>
<span data-ttu-id="2d72d-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2d72d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d72d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d72d-128">Response</span></span>

<span data-ttu-id="2d72d-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [PrivilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="2d72d-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="2d72d-130">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="2d72d-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2d72d-131">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="2d72d-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="2d72d-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d72d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d72d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d72d-133">Request</span></span>
<span data-ttu-id="2d72d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d72d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="2d72d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d72d-135">Response</span></span>
<span data-ttu-id="2d72d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d72d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
