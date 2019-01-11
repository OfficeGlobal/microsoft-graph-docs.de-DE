---
title: Abrufen der Outlook-Kategorie
description: Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen outlookCategory-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 45327a6143104b4507a8e573b5cba01b605abd00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863007"
---
# <a name="get-outlook-category"></a><span data-ttu-id="0aa1d-103">Abrufen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="0aa1d-103">Get Outlook category</span></span>

> <span data-ttu-id="0aa1d-104">**Wichtig**: unter der /beta Version von Microsoft Graph-APIs sind in der Vorschau und kann geändert werden.</span><span class="sxs-lookup"><span data-stu-id="0aa1d-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0aa1d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0aa1d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0aa1d-106">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen [outlookCategory](../resources/outlookcategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0aa1d-106">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0aa1d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0aa1d-107">Permissions</span></span>
<span data-ttu-id="0aa1d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aa1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aa1d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0aa1d-110">Permission type</span></span>      | <span data-ttu-id="0aa1d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0aa1d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aa1d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0aa1d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0aa1d-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0aa1d-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0aa1d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0aa1d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aa1d-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0aa1d-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0aa1d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0aa1d-116">Application</span></span> | <span data-ttu-id="0aa1d-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0aa1d-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0aa1d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0aa1d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0aa1d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0aa1d-119">Optional query parameters</span></span>
<span data-ttu-id="0aa1d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0aa1d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0aa1d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0aa1d-121">Request headers</span></span>
| <span data-ttu-id="0aa1d-122">Name</span><span class="sxs-lookup"><span data-stu-id="0aa1d-122">Name</span></span>      |<span data-ttu-id="0aa1d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aa1d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0aa1d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aa1d-124">Authorization</span></span>  | <span data-ttu-id="0aa1d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0aa1d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0aa1d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0aa1d-127">Request body</span></span>
<span data-ttu-id="0aa1d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0aa1d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0aa1d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0aa1d-129">Response</span></span>

<span data-ttu-id="0aa1d-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [outlookCategory](../resources/outlookcategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0aa1d-130">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0aa1d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0aa1d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0aa1d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0aa1d-132">Request</span></span>
<span data-ttu-id="0aa1d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0aa1d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories('de912e4d-c790-4da9-949c-ccd933aaa0f7')
```
##### <a name="response"></a><span data-ttu-id="0aa1d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0aa1d-134">Response</span></span>
<span data-ttu-id="0aa1d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0aa1d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
