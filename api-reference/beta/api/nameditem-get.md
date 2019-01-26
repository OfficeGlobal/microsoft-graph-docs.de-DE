---
title: NamedItem abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des nameditem-Objekts.
localization_priority: Normal
ms.openlocfilehash: bb190c8329389aed3196807d5b15f6a48a18240d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570995"
---
# <a name="get-nameditem"></a><span data-ttu-id="a3ba7-103">NamedItem abrufen</span><span class="sxs-lookup"><span data-stu-id="a3ba7-103">Get NamedItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3ba7-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des nameditem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a3ba7-104">Retrieve the properties and relationships of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3ba7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a3ba7-105">Permissions</span></span>
<span data-ttu-id="a3ba7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3ba7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3ba7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3ba7-108">Permission type</span></span>      | <span data-ttu-id="a3ba7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3ba7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3ba7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3ba7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3ba7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3ba7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a3ba7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3ba7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3ba7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3ba7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a3ba7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3ba7-114">Application</span></span> | <span data-ttu-id="a3ba7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3ba7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3ba7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3ba7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a3ba7-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a3ba7-117">Optional query parameters</span></span>
<span data-ttu-id="a3ba7-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a3ba7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3ba7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3ba7-119">Request headers</span></span>
| <span data-ttu-id="a3ba7-120">Name</span><span class="sxs-lookup"><span data-stu-id="a3ba7-120">Name</span></span>      |<span data-ttu-id="a3ba7-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3ba7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3ba7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3ba7-122">Authorization</span></span>  | <span data-ttu-id="a3ba7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a3ba7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3ba7-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a3ba7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a3ba7-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a3ba7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3ba7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3ba7-128">Request body</span></span>
<span data-ttu-id="a3ba7-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a3ba7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3ba7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3ba7-130">Response</span></span>

<span data-ttu-id="a3ba7-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [NamedItem](../resources/workbooknameditem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3ba7-131">If successful, this method returns a `200 OK` response code and [NamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a3ba7-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3ba7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3ba7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3ba7-133">Request</span></span>
<span data-ttu-id="a3ba7-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3ba7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_nameditem"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)
```
##### <a name="response"></a><span data-ttu-id="a3ba7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3ba7-135">Response</span></span>
<span data-ttu-id="a3ba7-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3ba7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get NamedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
