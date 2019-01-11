---
title: Abrufen von privilegedApproval
description: Rufen Sie die Eigenschaften und Beziehungen des Privilegedapproval-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: eef213416232db67bb0c1134e35d4af94734b468
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847621"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="e2895-103">Abrufen von privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="e2895-103">Get privilegedApproval</span></span>

> <span data-ttu-id="e2895-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2895-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2895-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2895-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2895-106">Rufen Sie die Eigenschaften und Beziehungen des Privilegedapproval-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="e2895-106">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2895-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e2895-107">Permissions</span></span>
<span data-ttu-id="e2895-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2895-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e2895-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2895-110">Permission type</span></span>      | <span data-ttu-id="e2895-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2895-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2895-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2895-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2895-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2895-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="e2895-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2895-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2895-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2895-115">Not supported.</span></span>    |
|<span data-ttu-id="e2895-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2895-116">Application</span></span> | <span data-ttu-id="e2895-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2895-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2895-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2895-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2895-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e2895-119">Optional query parameters</span></span>
<span data-ttu-id="e2895-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e2895-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2895-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2895-121">Request headers</span></span>
| <span data-ttu-id="e2895-122">Name</span><span class="sxs-lookup"><span data-stu-id="e2895-122">Name</span></span>      |<span data-ttu-id="e2895-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2895-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2895-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2895-124">Authorization</span></span>  | <span data-ttu-id="e2895-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e2895-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2895-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2895-127">Request body</span></span>
<span data-ttu-id="e2895-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e2895-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2895-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2895-129">Response</span></span>

<span data-ttu-id="e2895-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [PrivilegedApproval](../resources/privilegedapproval.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e2895-130">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="e2895-131">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="e2895-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e2895-132">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="e2895-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="e2895-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2895-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2895-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2895-134">Request</span></span>
<span data-ttu-id="e2895-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2895-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="e2895-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2895-136">Response</span></span>
<span data-ttu-id="e2895-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2895-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
