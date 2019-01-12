---
title: Notizbücher auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs notebook abrufen.
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: b66b059d92b1177a6c2b5df9a9d978eb87dec53e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975484"
---
# <a name="list-notebooks"></a><span data-ttu-id="ade42-103">Notizbücher auflisten</span><span class="sxs-lookup"><span data-stu-id="ade42-103">List notebooks</span></span>

<span data-ttu-id="ade42-104">Mit dieser API können Sie eine Liste von Objekten des Typs [notebook](../resources/notebook.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="ade42-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ade42-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ade42-105">Permissions</span></span>
<span data-ttu-id="ade42-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ade42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ade42-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ade42-108">Permission type</span></span>      | <span data-ttu-id="ade42-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ade42-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ade42-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ade42-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ade42-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ade42-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ade42-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ade42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ade42-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ade42-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ade42-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ade42-114">Application</span></span> | <span data-ttu-id="ade42-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ade42-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ade42-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ade42-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ade42-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ade42-117">Optional query parameters</span></span>
<span data-ttu-id="ade42-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ade42-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ade42-119">Die Standardsortierreihenfolge ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="ade42-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="ade42-120">Gültige `expand`-Werte für Notizbücher sind `sections` und `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="ade42-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ade42-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ade42-121">Request headers</span></span>
| <span data-ttu-id="ade42-122">Name</span><span class="sxs-lookup"><span data-stu-id="ade42-122">Name</span></span>       | <span data-ttu-id="ade42-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ade42-123">Type</span></span> | <span data-ttu-id="ade42-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ade42-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ade42-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ade42-125">Authorization</span></span>  | <span data-ttu-id="ade42-126">string</span><span class="sxs-lookup"><span data-stu-id="ade42-126">string</span></span>  | <span data-ttu-id="ade42-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ade42-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ade42-129">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ade42-129">Accept</span></span> | <span data-ttu-id="ade42-130">string</span><span class="sxs-lookup"><span data-stu-id="ade42-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ade42-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ade42-131">Request body</span></span>
<span data-ttu-id="ade42-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ade42-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ade42-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ade42-133">Response</span></span>

<span data-ttu-id="ade42-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [notebook](../resources/notebook.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ade42-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ade42-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ade42-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ade42-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ade42-136">Request</span></span>
<span data-ttu-id="ade42-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ade42-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="ade42-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ade42-138">Response</span></span>
<span data-ttu-id="ade42-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ade42-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
