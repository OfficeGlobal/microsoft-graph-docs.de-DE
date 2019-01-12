---
title: Seite abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines page-Objekts.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 4d583ec28b96b9ec537aaf067371f4ae68fa3375
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979306"
---
# <a name="get-page"></a><span data-ttu-id="7b497-103">Seite abrufen</span><span class="sxs-lookup"><span data-stu-id="7b497-103">Get page</span></span>

> <span data-ttu-id="7b497-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7b497-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b497-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b497-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b497-106">Dient zum Abrufen der Eigenschaften und Beziehungen eines [page](../resources/page.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7b497-106">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="7b497-107">**Seiteninformationen abrufen**</span><span class="sxs-lookup"><span data-stu-id="7b497-107">**Getting page information**</span></span>

<span data-ttu-id="7b497-108">Greifen Sie über den Seitenbezeichner auf die Metadaten einer Seite zu:</span><span class="sxs-lookup"><span data-stu-id="7b497-108">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="7b497-109">**Seiteninhalt abrufen**</span><span class="sxs-lookup"><span data-stu-id="7b497-109">**Getting page content**</span></span>

<span data-ttu-id="7b497-110">Sie können den `content`-Endpunkt der Seite verwenden, um den HTML-Inhalt einer Seite abzurufen:</span><span class="sxs-lookup"><span data-stu-id="7b497-110">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="7b497-111">Die Abfrageoption `includeIDs=true` wird verwendet, um [Seiten zu aktualisieren](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="7b497-111">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b497-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b497-112">Permissions</span></span>
<span data-ttu-id="7b497-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b497-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b497-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b497-115">Permission type</span></span>      | <span data-ttu-id="7b497-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b497-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b497-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b497-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7b497-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b497-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b497-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b497-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b497-120">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b497-120">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7b497-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b497-121">Application</span></span> | <span data-ttu-id="7b497-122">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b497-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b497-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b497-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b497-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7b497-124">Optional query parameters</span></span>
<span data-ttu-id="7b497-125">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b497-125">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7b497-p103">Die Standardantwort erweitert `parentSection` und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus. Gültige `expand`-Werte für Seiten sind `parentNotebook` und `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="7b497-p103">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b497-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b497-128">Request headers</span></span>
| <span data-ttu-id="7b497-129">Name</span><span class="sxs-lookup"><span data-stu-id="7b497-129">Name</span></span>       | <span data-ttu-id="7b497-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7b497-130">Type</span></span> | <span data-ttu-id="7b497-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b497-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7b497-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b497-132">Authorization</span></span>  | <span data-ttu-id="7b497-133">string</span><span class="sxs-lookup"><span data-stu-id="7b497-133">string</span></span>  | <span data-ttu-id="7b497-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b497-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b497-136">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7b497-136">Accept</span></span> | <span data-ttu-id="7b497-137">string</span><span class="sxs-lookup"><span data-stu-id="7b497-137">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7b497-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b497-138">Request body</span></span>
<span data-ttu-id="7b497-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b497-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b497-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b497-140">Response</span></span>

<span data-ttu-id="7b497-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [page](../resources/page.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b497-141">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b497-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b497-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b497-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b497-143">Request</span></span>
<span data-ttu-id="7b497-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b497-144">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="7b497-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b497-145">Response</span></span>
<span data-ttu-id="7b497-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b497-146">Here is an example of the response.</span></span> <span data-ttu-id="7b497-147">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="7b497-147">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="7b497-148">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b497-148">All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
