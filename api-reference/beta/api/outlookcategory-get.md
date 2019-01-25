---
title: Abrufen der Outlook-Kategorie
description: Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen outlookCategory-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7529568b26c56258e63a8c1080c019aaf0f57e59
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520039"
---
# <a name="get-outlook-category"></a><span data-ttu-id="4258e-103">Abrufen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="4258e-103">Get Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4258e-104">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen [outlookCategory](../resources/outlookcategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4258e-104">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4258e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4258e-105">Permissions</span></span>
<span data-ttu-id="4258e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4258e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4258e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4258e-108">Permission type</span></span>      | <span data-ttu-id="4258e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4258e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4258e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4258e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4258e-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4258e-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4258e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4258e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4258e-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4258e-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4258e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4258e-114">Application</span></span> | <span data-ttu-id="4258e-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4258e-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4258e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4258e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4258e-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4258e-117">Optional query parameters</span></span>
<span data-ttu-id="4258e-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4258e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4258e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4258e-119">Request headers</span></span>
| <span data-ttu-id="4258e-120">Name</span><span class="sxs-lookup"><span data-stu-id="4258e-120">Name</span></span>      |<span data-ttu-id="4258e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4258e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4258e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4258e-122">Authorization</span></span>  | <span data-ttu-id="4258e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4258e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4258e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4258e-125">Request body</span></span>
<span data-ttu-id="4258e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4258e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4258e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4258e-127">Response</span></span>

<span data-ttu-id="4258e-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [outlookCategory](../resources/outlookcategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4258e-128">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4258e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4258e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4258e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4258e-130">Request</span></span>
<span data-ttu-id="4258e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4258e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories('de912e4d-c790-4da9-949c-ccd933aaa0f7')
```
##### <a name="response"></a><span data-ttu-id="4258e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4258e-132">Response</span></span>
<span data-ttu-id="4258e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4258e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookcategory-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
