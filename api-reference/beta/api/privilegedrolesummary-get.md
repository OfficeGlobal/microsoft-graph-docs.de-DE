---
title: Abrufen von privilegedRoleSummary
description: Rufen Sie die Eigenschaften und Beziehungen des PrivilegedRoleSummary-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: ebe3a0774869c09ba26cd01726590a6b7cddb58f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816079"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="d34d0-103">Abrufen von privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="d34d0-103">Get privilegedRoleSummary</span></span>

> <span data-ttu-id="d34d0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d34d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d34d0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d34d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d34d0-106">Rufen Sie die Eigenschaften und Beziehungen des [PrivilegedRoleSummary](../resources/privilegedrolesummary.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="d34d0-106">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d34d0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d34d0-107">Permissions</span></span>
<span data-ttu-id="d34d0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d34d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d34d0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d34d0-110">Permission type</span></span>      | <span data-ttu-id="d34d0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d34d0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d34d0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d34d0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d34d0-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d34d0-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d34d0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d34d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d34d0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d34d0-115">Not supported.</span></span>    |
|<span data-ttu-id="d34d0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d34d0-116">Application</span></span> | <span data-ttu-id="d34d0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d34d0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d34d0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d34d0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d34d0-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d34d0-119">Optional query parameters</span></span>
<span data-ttu-id="d34d0-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d34d0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d34d0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d34d0-121">Request headers</span></span>
| <span data-ttu-id="d34d0-122">Name</span><span class="sxs-lookup"><span data-stu-id="d34d0-122">Name</span></span>      |<span data-ttu-id="d34d0-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d34d0-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d34d0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d34d0-124">Authorization</span></span>  | <span data-ttu-id="d34d0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d34d0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d34d0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d34d0-127">Request body</span></span>
<span data-ttu-id="d34d0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d34d0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d34d0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d34d0-129">Response</span></span>

<span data-ttu-id="d34d0-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [PrivilegedRoleSummary](../resources/privilegedrolesummary.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d34d0-130">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="d34d0-131">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="d34d0-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d34d0-132">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="d34d0-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="d34d0-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d34d0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d34d0-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d34d0-134">Request</span></span>
<span data-ttu-id="d34d0-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d34d0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="d34d0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d34d0-136">Response</span></span>
<span data-ttu-id="d34d0-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d34d0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
