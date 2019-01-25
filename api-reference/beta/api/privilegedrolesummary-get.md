---
title: Abrufen von privilegedRoleSummary
description: Rufen Sie die Eigenschaften und Beziehungen des PrivilegedRoleSummary-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: 3778ddcc297607b062354dcdf44727a0f57375dc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508230"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="8054d-103">Abrufen von privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="8054d-103">Get privilegedRoleSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8054d-104">Rufen Sie die Eigenschaften und Beziehungen des [PrivilegedRoleSummary](../resources/privilegedrolesummary.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="8054d-104">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8054d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8054d-105">Permissions</span></span>
<span data-ttu-id="8054d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8054d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8054d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8054d-108">Permission type</span></span>      | <span data-ttu-id="8054d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8054d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8054d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8054d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8054d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8054d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8054d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8054d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8054d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8054d-113">Not supported.</span></span>    |
|<span data-ttu-id="8054d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8054d-114">Application</span></span> | <span data-ttu-id="8054d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8054d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8054d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8054d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8054d-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8054d-117">Optional query parameters</span></span>
<span data-ttu-id="8054d-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8054d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8054d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8054d-119">Request headers</span></span>
| <span data-ttu-id="8054d-120">Name</span><span class="sxs-lookup"><span data-stu-id="8054d-120">Name</span></span>      |<span data-ttu-id="8054d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8054d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8054d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8054d-122">Authorization</span></span>  | <span data-ttu-id="8054d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8054d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8054d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8054d-125">Request body</span></span>
<span data-ttu-id="8054d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8054d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8054d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="8054d-127">Response</span></span>

<span data-ttu-id="8054d-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [PrivilegedRoleSummary](../resources/privilegedrolesummary.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8054d-128">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="8054d-129">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="8054d-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8054d-130">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="8054d-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="8054d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8054d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8054d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8054d-132">Request</span></span>
<span data-ttu-id="8054d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8054d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="8054d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8054d-134">Response</span></span>
<span data-ttu-id="8054d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8054d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
