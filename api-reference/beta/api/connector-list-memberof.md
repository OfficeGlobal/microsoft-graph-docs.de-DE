---
title: memberOf auflisten
description: Abrufen der Connectorgroup, für der Connector ein Mitglied ist.
localization_priority: Normal
ms.openlocfilehash: 4f9bea5e61b12b6a59413a3a159148e6b5963f16
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530167"
---
# <a name="list-memberof"></a><span data-ttu-id="f7aaf-103">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="f7aaf-103">List memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7aaf-104">Abrufen der Connectorgroup, für der Connector ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="f7aaf-104">Retrieve the connectorgroup the connector is a member of.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7aaf-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7aaf-105">Permissions</span></span>
<span data-ttu-id="f7aaf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7aaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7aaf-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7aaf-108">Permission type</span></span>      | <span data-ttu-id="f7aaf-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7aaf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7aaf-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7aaf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7aaf-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7aaf-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f7aaf-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7aaf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7aaf-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7aaf-113">Not supported.</span></span>    |
|<span data-ttu-id="f7aaf-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7aaf-114">Application</span></span> | <span data-ttu-id="f7aaf-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7aaf-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7aaf-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7aaf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7aaf-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f7aaf-117">Optional query parameters</span></span>
<span data-ttu-id="f7aaf-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7aaf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7aaf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7aaf-119">Request headers</span></span>
| <span data-ttu-id="f7aaf-120">Name</span><span class="sxs-lookup"><span data-stu-id="f7aaf-120">Name</span></span>      |<span data-ttu-id="f7aaf-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7aaf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7aaf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7aaf-122">Authorization</span></span>  | <span data-ttu-id="f7aaf-123">Bearer </span><span class="sxs-lookup"><span data-stu-id="f7aaf-123">Bearer.</span></span> <span data-ttu-id="f7aaf-124">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="f7aaf-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7aaf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7aaf-125">Request body</span></span>
<span data-ttu-id="f7aaf-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f7aaf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7aaf-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7aaf-127">Response</span></span>

<span data-ttu-id="f7aaf-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [ConnectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="f7aaf-128">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7aaf-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7aaf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7aaf-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7aaf-130">Request</span></span>
<span data-ttu-id="f7aaf-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f7aaf-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="f7aaf-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7aaf-132">Response</span></span>
<span data-ttu-id="f7aaf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7aaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connector-list-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
