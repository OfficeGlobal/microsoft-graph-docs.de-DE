---
title: Seiten auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs page aus dem angegebenen Abschnitt abrufen.
localization_priority: Normal
ms.openlocfilehash: 9e0dea1f9a786734222dbc4c93b059e22d4322bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813020"
---
# <a name="list-pages"></a><span data-ttu-id="e833e-103">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="e833e-103">List pages</span></span>

> <span data-ttu-id="e833e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e833e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e833e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e833e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e833e-106">Mit dieser API können Sie eine Liste von Objekten des Typs [page](../resources/page.md) aus dem angegebenen Abschnitt abrufen.</span><span class="sxs-lookup"><span data-stu-id="e833e-106">Retrieve a list of [page](../resources/page.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="e833e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e833e-107">Permissions</span></span>
<span data-ttu-id="e833e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e833e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e833e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e833e-110">Permission type</span></span>      | <span data-ttu-id="e833e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e833e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e833e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e833e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e833e-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e833e-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e833e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e833e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e833e-115">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e833e-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e833e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e833e-116">Application</span></span> | <span data-ttu-id="e833e-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e833e-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e833e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e833e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e833e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e833e-119">Optional query parameters</span></span>
<span data-ttu-id="e833e-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e833e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e833e-p103">Die Standardabfrage für Seiten gibt die ersten 20 Seiten sortiert nach `lastModifiedTime desc` zurück. Wenn die Standardabfrage mehr als 20 Seiten zurückgibt, enthält die Antwort ein `@odata.nextLink`-Objekt, mit dem Sie seitenweise durch das Resultset blättern können. Die maximale Anzahl von Seiten, die für eine `top`-Anforderung zurückgegeben werden, beträgt 100.</span><span class="sxs-lookup"><span data-stu-id="e833e-p103">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="e833e-p104">Die Standardantwort erweitert `parentSection` und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus. Gültige `expand`-Werte für Seiten sind `parentNotebook` und `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="e833e-p104">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e833e-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e833e-126">Request headers</span></span>
| <span data-ttu-id="e833e-127">Name</span><span class="sxs-lookup"><span data-stu-id="e833e-127">Name</span></span>       | <span data-ttu-id="e833e-128">Typ</span><span class="sxs-lookup"><span data-stu-id="e833e-128">Type</span></span> | <span data-ttu-id="e833e-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e833e-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e833e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e833e-130">Authorization</span></span>  | <span data-ttu-id="e833e-131">string</span><span class="sxs-lookup"><span data-stu-id="e833e-131">string</span></span>  | <span data-ttu-id="e833e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e833e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e833e-134">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e833e-134">Accept</span></span> | <span data-ttu-id="e833e-135">string</span><span class="sxs-lookup"><span data-stu-id="e833e-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e833e-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e833e-136">Request body</span></span>
<span data-ttu-id="e833e-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e833e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e833e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="e833e-138">Response</span></span>

<span data-ttu-id="e833e-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [page](../resources/page.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e833e-139">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e833e-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e833e-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e833e-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e833e-141">Request</span></span>
<span data-ttu-id="e833e-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e833e-142">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="e833e-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="e833e-143">Response</span></span>
<span data-ttu-id="e833e-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e833e-144">Here is an example of the response.</span></span> <span data-ttu-id="e833e-145">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="e833e-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="e833e-146">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e833e-146">All of the properties will be returned from an actual call.</span></span>
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
