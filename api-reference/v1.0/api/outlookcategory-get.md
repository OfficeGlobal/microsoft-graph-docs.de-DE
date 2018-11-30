---
title: Abrufen der Outlook-Kategorie
description: Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen outlookCategory-Objekts.
ms.openlocfilehash: 51bed62b1dffe648f62caecdc8d038a21c0d1c6f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27015982"
---
# <a name="get-outlook-category"></a><span data-ttu-id="4b06c-103">Abrufen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="4b06c-103">Get Outlook category</span></span>


<span data-ttu-id="4b06c-104">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen [outlookCategory](../resources/outlookcategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b06c-104">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b06c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4b06c-105">Permissions</span></span>
<span data-ttu-id="4b06c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b06c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b06c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b06c-108">Permission type</span></span>      | <span data-ttu-id="4b06c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b06c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b06c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b06c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b06c-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4b06c-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4b06c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b06c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b06c-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4b06c-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4b06c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b06c-114">Application</span></span> | <span data-ttu-id="4b06c-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4b06c-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b06c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b06c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4b06c-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4b06c-117">Optional query parameters</span></span>
<span data-ttu-id="4b06c-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4b06c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b06c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b06c-119">Request headers</span></span>
| <span data-ttu-id="4b06c-120">Name</span><span class="sxs-lookup"><span data-stu-id="4b06c-120">Name</span></span>      |<span data-ttu-id="4b06c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b06c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4b06c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b06c-122">Authorization</span></span>  | <span data-ttu-id="4b06c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b06c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b06c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b06c-125">Request body</span></span>
<span data-ttu-id="4b06c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4b06c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b06c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b06c-127">Response</span></span>

<span data-ttu-id="4b06c-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [outlookCategory](../resources/outlookcategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b06c-128">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b06c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b06c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b06c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b06c-130">Request</span></span>
<span data-ttu-id="4b06c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b06c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["de912e4d-c790-4da9-949c-ccd933aaa0f7"],
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
##### <a name="response"></a><span data-ttu-id="4b06c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b06c-132">Response</span></span>
<span data-ttu-id="4b06c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b06c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
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
  "tocPath": ""
}-->