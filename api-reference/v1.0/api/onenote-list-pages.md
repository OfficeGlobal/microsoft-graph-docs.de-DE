---
title: Seiten auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs page abrufen.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: f06404437fbd5dc34cef6d81e5b3d692bf5ce101
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829365"
---
# <a name="list-pages"></a><span data-ttu-id="e74e8-103">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="e74e8-103">List pages</span></span>

<span data-ttu-id="e74e8-104">Mit dieser API können Sie eine Liste von Objekten des Typs [page](../resources/page.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="e74e8-104">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e74e8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e74e8-105">Permissions</span></span>
<span data-ttu-id="e74e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e74e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e74e8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e74e8-108">Permission type</span></span>      | <span data-ttu-id="e74e8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e74e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e74e8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e74e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e74e8-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e74e8-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e74e8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e74e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e74e8-113">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e74e8-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e74e8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e74e8-114">Application</span></span> | <span data-ttu-id="e74e8-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e74e8-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e74e8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e74e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e74e8-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e74e8-117">Optional query parameters</span></span>
<span data-ttu-id="e74e8-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e74e8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e74e8-p102">Die Standardabfrage für Seiten gibt die ersten 20 Seiten sortiert nach `lastModifiedTime desc` zurück. Wenn die Standardabfrage mehr als 20 Seiten zurückgibt, enthält die Antwort ein `@odata.nextLink`-Objekt, mit dem Sie seitenweise durch das Resultset blättern können. Die maximale Anzahl von Seiten, die für eine `top`-Anforderung zurückgegeben werden, beträgt 100.</span><span class="sxs-lookup"><span data-stu-id="e74e8-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="e74e8-p103">Die Standardantwort erweitert `parentSection` und wählt die Eigenschaften `id`, `displayName` und `self` des Abschnitts aus. Gültige `expand`-Werte für Seiten sind `parentNotebook` und `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="e74e8-p103">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e74e8-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e74e8-124">Request headers</span></span>
| <span data-ttu-id="e74e8-125">Name</span><span class="sxs-lookup"><span data-stu-id="e74e8-125">Name</span></span>       | <span data-ttu-id="e74e8-126">Typ</span><span class="sxs-lookup"><span data-stu-id="e74e8-126">Type</span></span> | <span data-ttu-id="e74e8-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e74e8-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e74e8-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e74e8-128">Authorization</span></span>  | <span data-ttu-id="e74e8-129">string</span><span class="sxs-lookup"><span data-stu-id="e74e8-129">string</span></span>  | <span data-ttu-id="e74e8-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e74e8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e74e8-132">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e74e8-132">Accept</span></span> | <span data-ttu-id="e74e8-133">string</span><span class="sxs-lookup"><span data-stu-id="e74e8-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e74e8-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e74e8-134">Request body</span></span>
<span data-ttu-id="e74e8-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e74e8-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e74e8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e74e8-136">Response</span></span>

<span data-ttu-id="e74e8-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [page](../resources/page.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e74e8-137">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e74e8-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e74e8-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e74e8-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e74e8-139">Request</span></span>
<span data-ttu-id="e74e8-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e74e8-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="e74e8-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e74e8-141">Response</span></span>
<span data-ttu-id="e74e8-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e74e8-142">Here is an example of the response.</span></span> <span data-ttu-id="e74e8-143">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="e74e8-143">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="e74e8-144">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e74e8-144">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 393

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
