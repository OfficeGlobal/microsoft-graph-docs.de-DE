---
title: Seite abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines page-Objekts.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 1cafa1b430f20fc74d045c498d7bba81eb160463
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572633"
---
# <a name="get-page"></a><span data-ttu-id="4e39b-103">Seite abrufen</span><span class="sxs-lookup"><span data-stu-id="4e39b-103">Get page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e39b-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines [page](../resources/onenotepage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e39b-104">Retrieve the properties and relationships of a [page](../resources/onenotepage.md) object.</span></span>

<span data-ttu-id="4e39b-105">**Seiteninformationen abrufen**</span><span class="sxs-lookup"><span data-stu-id="4e39b-105">**Getting page information**</span></span>

<span data-ttu-id="4e39b-106">Greifen Sie über den Seitenbezeichner auf die Metadaten einer Seite zu:</span><span class="sxs-lookup"><span data-stu-id="4e39b-106">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="4e39b-107">**Seiteninhalt abrufen**</span><span class="sxs-lookup"><span data-stu-id="4e39b-107">**Getting page content**</span></span>

<span data-ttu-id="4e39b-108">Sie können den `content`-Endpunkt der Seite verwenden, um den HTML-Inhalt einer Seite abzurufen:</span><span class="sxs-lookup"><span data-stu-id="4e39b-108">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="4e39b-109">Die Abfrageoption `includeIDs=true` wird verwendet, um [Seiten zu aktualisieren](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="4e39b-109">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e39b-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4e39b-110">Permissions</span></span>
<span data-ttu-id="4e39b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e39b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e39b-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e39b-113">Permission type</span></span>      | <span data-ttu-id="4e39b-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e39b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e39b-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e39b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4e39b-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e39b-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e39b-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e39b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e39b-118">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e39b-118">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4e39b-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e39b-119">Application</span></span> | <span data-ttu-id="4e39b-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e39b-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e39b-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e39b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4e39b-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4e39b-122">Optional query parameters</span></span>
<span data-ttu-id="4e39b-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4e39b-123">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4e39b-p102">Die Standardantwort erweitert `parentSection` und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus. Gültige `expand`-Werte für Seiten sind `parentNotebook` und `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="4e39b-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e39b-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e39b-126">Request headers</span></span>
| <span data-ttu-id="4e39b-127">Name</span><span class="sxs-lookup"><span data-stu-id="4e39b-127">Name</span></span>       | <span data-ttu-id="4e39b-128">Typ</span><span class="sxs-lookup"><span data-stu-id="4e39b-128">Type</span></span> | <span data-ttu-id="4e39b-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e39b-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4e39b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e39b-130">Authorization</span></span>  | <span data-ttu-id="4e39b-131">string</span><span class="sxs-lookup"><span data-stu-id="4e39b-131">string</span></span>  | <span data-ttu-id="4e39b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4e39b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e39b-134">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4e39b-134">Accept</span></span> | <span data-ttu-id="4e39b-135">string</span><span class="sxs-lookup"><span data-stu-id="4e39b-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4e39b-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e39b-136">Request body</span></span>
<span data-ttu-id="4e39b-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4e39b-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e39b-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e39b-138">Response</span></span>

<span data-ttu-id="4e39b-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [page](../resources/onenotepage.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e39b-139">If successful, this method returns a `200 OK` response code and the [page](../resources/onenotepage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e39b-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e39b-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e39b-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e39b-141">Request</span></span>
<span data-ttu-id="4e39b-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e39b-142">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="4e39b-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e39b-143">Response</span></span>
<span data-ttu-id="4e39b-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4e39b-144">Here is an example of the response.</span></span> <span data-ttu-id="4e39b-145">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="4e39b-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="4e39b-146">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e39b-146">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/page-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
