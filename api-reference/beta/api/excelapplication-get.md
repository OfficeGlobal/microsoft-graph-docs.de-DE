---
title: Abrufen der Anwendung
description: Rufen Sie die Eigenschaften und Beziehungen des Application-Objekts ab.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 024e2cde999e90b1f361e7f67ca28ddd71078824
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522924"
---
# <a name="get-application"></a><span data-ttu-id="96467-103">Abrufen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="96467-103">Get Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96467-104">Rufen Sie die Eigenschaften und Beziehungen des Application-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="96467-104">Retrieve the properties and relationships of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="96467-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="96467-105">Permissions</span></span>
<span data-ttu-id="96467-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96467-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96467-108">Permission type</span></span>      | <span data-ttu-id="96467-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96467-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96467-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96467-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96467-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96467-111">Not supported.</span></span>    |
|<span data-ttu-id="96467-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96467-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96467-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96467-113">Not supported.</span></span>    |
|<span data-ttu-id="96467-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96467-114">Application</span></span> | <span data-ttu-id="96467-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96467-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96467-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96467-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96467-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="96467-117">Optional query parameters</span></span>
<span data-ttu-id="96467-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="96467-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96467-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96467-119">Request headers</span></span>
| <span data-ttu-id="96467-120">Name</span><span class="sxs-lookup"><span data-stu-id="96467-120">Name</span></span>      |<span data-ttu-id="96467-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96467-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96467-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96467-122">Authorization</span></span>  | <span data-ttu-id="96467-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96467-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96467-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96467-125">Request body</span></span>
<span data-ttu-id="96467-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="96467-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96467-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="96467-127">Response</span></span>

<span data-ttu-id="96467-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und [Application](../resources/application.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="96467-128">If successful, this method returns a `200 OK` response code and [Application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96467-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96467-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96467-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96467-130">Request</span></span>
<span data-ttu-id="96467-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96467-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="96467-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="96467-132">Response</span></span>
<span data-ttu-id="96467-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96467-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/excelapplication-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
