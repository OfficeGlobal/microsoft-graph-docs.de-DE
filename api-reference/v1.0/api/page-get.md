---
title: Seite abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines page-Objekts.
localization_priority: Normal
ms.openlocfilehash: 7fac5d442ade9f41201881e6b5082ce9ec5fed0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807945"
---
# <a name="get-page"></a><span data-ttu-id="bbf98-103">Seite abrufen</span><span class="sxs-lookup"><span data-stu-id="bbf98-103">Get page</span></span>

<span data-ttu-id="bbf98-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines [page](../resources/page.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bbf98-104">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="bbf98-105">**Seiteninformationen abrufen**</span><span class="sxs-lookup"><span data-stu-id="bbf98-105">**Getting page information**</span></span>

<span data-ttu-id="bbf98-106">Greifen Sie über den Seitenbezeichner auf die Metadaten einer Seite zu:</span><span class="sxs-lookup"><span data-stu-id="bbf98-106">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="bbf98-107">**Seiteninhalt abrufen**</span><span class="sxs-lookup"><span data-stu-id="bbf98-107">**Getting page content**</span></span>

<span data-ttu-id="bbf98-108">Sie können den `content`-Endpunkt der Seite verwenden, um den HTML-Inhalt einer Seite abzurufen:</span><span class="sxs-lookup"><span data-stu-id="bbf98-108">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="bbf98-109">Die Abfrageoption `includeIDs=true` wird verwendet, um [Seiten zu aktualisieren](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="bbf98-109">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bbf98-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bbf98-110">Permissions</span></span>
<span data-ttu-id="bbf98-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbf98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbf98-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bbf98-113">Permission type</span></span>      | <span data-ttu-id="bbf98-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bbf98-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbf98-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bbf98-115">Delegated (work or school account)</span></span> | <span data-ttu-id="bbf98-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf98-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="bbf98-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bbf98-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbf98-118">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbf98-118">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="bbf98-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bbf98-119">Application</span></span> | <span data-ttu-id="bbf98-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf98-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbf98-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bbf98-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bbf98-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bbf98-122">Optional query parameters</span></span>
<span data-ttu-id="bbf98-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bbf98-123">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="bbf98-p102">Die Standardantwort erweitert `parentSection` und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus. Gültige `expand`-Werte für Seiten sind `parentNotebook` und `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="bbf98-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbf98-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bbf98-126">Request headers</span></span>
| <span data-ttu-id="bbf98-127">Name</span><span class="sxs-lookup"><span data-stu-id="bbf98-127">Name</span></span>       | <span data-ttu-id="bbf98-128">Typ</span><span class="sxs-lookup"><span data-stu-id="bbf98-128">Type</span></span> | <span data-ttu-id="bbf98-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbf98-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bbf98-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbf98-130">Authorization</span></span>  | <span data-ttu-id="bbf98-131">string</span><span class="sxs-lookup"><span data-stu-id="bbf98-131">string</span></span>  | <span data-ttu-id="bbf98-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bbf98-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbf98-134">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bbf98-134">Accept</span></span> | <span data-ttu-id="bbf98-135">string</span><span class="sxs-lookup"><span data-stu-id="bbf98-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="bbf98-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bbf98-136">Request body</span></span>
<span data-ttu-id="bbf98-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bbf98-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbf98-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="bbf98-138">Response</span></span>

<span data-ttu-id="bbf98-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [page](../resources/page.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bbf98-139">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bbf98-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bbf98-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbf98-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bbf98-141">Request</span></span>
<span data-ttu-id="bbf98-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bbf98-142">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="bbf98-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="bbf98-143">Response</span></span>
<span data-ttu-id="bbf98-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bbf98-144">Here is an example of the response.</span></span> <span data-ttu-id="bbf98-145">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="bbf98-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="bbf98-146">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bbf98-146">All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
