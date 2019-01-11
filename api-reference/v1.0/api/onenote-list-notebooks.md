---
title: Notizbücher auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs notebook abrufen.
author: Jewan-microsoft
localization_priority: Priority
ms.openlocfilehash: 5a6ae25ab048e0f0e9b25144957add5bbf85d615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810150"
---
# <a name="list-notebooks"></a><span data-ttu-id="79cfe-103">Notizbücher auflisten</span><span class="sxs-lookup"><span data-stu-id="79cfe-103">List notebooks</span></span>

<span data-ttu-id="79cfe-104">Mit dieser API können Sie eine Liste von Objekten des Typs [notebook](../resources/notebook.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="79cfe-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="79cfe-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="79cfe-105">Permissions</span></span>
<span data-ttu-id="79cfe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79cfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79cfe-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79cfe-108">Permission type</span></span>      | <span data-ttu-id="79cfe-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79cfe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79cfe-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79cfe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79cfe-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79cfe-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="79cfe-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79cfe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79cfe-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79cfe-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="79cfe-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79cfe-114">Application</span></span> | <span data-ttu-id="79cfe-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79cfe-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79cfe-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79cfe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79cfe-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="79cfe-117">Optional query parameters</span></span>
<span data-ttu-id="79cfe-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="79cfe-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="79cfe-119">Die Standardsortierreihenfolge ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="79cfe-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="79cfe-120">Gültige `expand`-Werte für Notizbücher sind `sections` und `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="79cfe-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79cfe-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79cfe-121">Request headers</span></span>
| <span data-ttu-id="79cfe-122">Name</span><span class="sxs-lookup"><span data-stu-id="79cfe-122">Name</span></span>       | <span data-ttu-id="79cfe-123">Typ</span><span class="sxs-lookup"><span data-stu-id="79cfe-123">Type</span></span> | <span data-ttu-id="79cfe-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79cfe-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="79cfe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="79cfe-125">Authorization</span></span>  | <span data-ttu-id="79cfe-126">string</span><span class="sxs-lookup"><span data-stu-id="79cfe-126">string</span></span>  | <span data-ttu-id="79cfe-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79cfe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79cfe-129">Annehmen</span><span class="sxs-lookup"><span data-stu-id="79cfe-129">Accept</span></span> | <span data-ttu-id="79cfe-130">string</span><span class="sxs-lookup"><span data-stu-id="79cfe-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="79cfe-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79cfe-131">Request body</span></span>
<span data-ttu-id="79cfe-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="79cfe-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79cfe-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="79cfe-133">Response</span></span>

<span data-ttu-id="79cfe-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [notebook](../resources/notebook.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79cfe-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79cfe-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79cfe-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79cfe-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79cfe-136">Request</span></span>
<span data-ttu-id="79cfe-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79cfe-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="79cfe-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="79cfe-138">Response</span></span>
<span data-ttu-id="79cfe-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79cfe-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
    {
      "isDefault": true,
      "userRole": {
      },
      "isShared": true,
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
