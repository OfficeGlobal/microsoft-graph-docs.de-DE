---
title: workbookPivotTable abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 65f6600fba2b1072c8501f6e2417b33a728b3410
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522119"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="64b21-103">workbookPivotTable abrufen</span><span class="sxs-lookup"><span data-stu-id="64b21-103">Get workbookPivotTable</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64b21-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.</span><span class="sxs-lookup"><span data-stu-id="64b21-104">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64b21-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="64b21-105">Permissions</span></span>
<span data-ttu-id="64b21-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="64b21-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64b21-108">Permission type</span></span>      | <span data-ttu-id="64b21-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64b21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64b21-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64b21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64b21-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64b21-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="64b21-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64b21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64b21-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64b21-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="64b21-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64b21-114">Application</span></span> | <span data-ttu-id="64b21-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64b21-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64b21-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64b21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="64b21-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="64b21-117">Optional query parameters</span></span>
<span data-ttu-id="64b21-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64b21-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64b21-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64b21-119">Request headers</span></span>
| <span data-ttu-id="64b21-120">Name</span><span class="sxs-lookup"><span data-stu-id="64b21-120">Name</span></span>      |<span data-ttu-id="64b21-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64b21-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64b21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64b21-122">Authorization</span></span>  | <span data-ttu-id="64b21-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="64b21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64b21-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="64b21-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="64b21-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="64b21-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b21-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64b21-128">Request body</span></span>
<span data-ttu-id="64b21-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="64b21-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64b21-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="64b21-130">Response</span></span>

<span data-ttu-id="64b21-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das  [workbookPivotTable](../resources/workbookpivottable.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64b21-131">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64b21-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64b21-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64b21-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64b21-133">Request</span></span>
<span data-ttu-id="64b21-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64b21-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="64b21-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="64b21-135">Response</span></span>
<span data-ttu-id="64b21-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64b21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookpivottable-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
