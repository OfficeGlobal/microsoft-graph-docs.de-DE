---
title: Namen auflisten
description: 'Dient zum Abrufen einer Liste von benannten Elementen, die mit dem Arbeitsblatt verknüpft sind. '
ms.openlocfilehash: 202e44c2747d8f90bb79183419038d9f5c632e3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018636"
---
# <a name="list-names"></a><span data-ttu-id="71e46-103">Namen auflisten</span><span class="sxs-lookup"><span data-stu-id="71e46-103">List names</span></span>

<span data-ttu-id="71e46-104">Dient zum Abrufen einer Liste von benannten Elementen, die mit dem Arbeitsblatt verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="71e46-104">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="71e46-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="71e46-105">Permissions</span></span>
<span data-ttu-id="71e46-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71e46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71e46-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71e46-108">Permission type</span></span>      | <span data-ttu-id="71e46-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71e46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71e46-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71e46-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71e46-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71e46-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71e46-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71e46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71e46-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71e46-113">Not supported.</span></span>    |
|<span data-ttu-id="71e46-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71e46-114">Application</span></span> | <span data-ttu-id="71e46-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="71e46-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71e46-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71e46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71e46-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="71e46-117">Optional query parameters</span></span>
<span data-ttu-id="71e46-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71e46-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71e46-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71e46-119">Request headers</span></span>
| <span data-ttu-id="71e46-120">Name</span><span class="sxs-lookup"><span data-stu-id="71e46-120">Name</span></span>      |<span data-ttu-id="71e46-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71e46-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71e46-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71e46-122">Authorization</span></span>  | <span data-ttu-id="71e46-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71e46-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71e46-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="71e46-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="71e46-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="71e46-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71e46-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71e46-128">Request body</span></span>
<span data-ttu-id="71e46-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="71e46-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71e46-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="71e46-130">Response</span></span>

<span data-ttu-id="71e46-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [WorkbookNamedItem](../resources/nameditem.md) .</span><span class="sxs-lookup"><span data-stu-id="71e46-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71e46-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71e46-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71e46-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71e46-133">Request</span></span>
<span data-ttu-id="71e46-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71e46-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="71e46-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="71e46-135">Response</span></span>
<span data-ttu-id="71e46-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71e46-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->