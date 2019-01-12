---
title: Notizbuch abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs notebook abrufen.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: befabbe46950b6b68819be992f0257cc121a2075
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927639"
---
# <a name="get-notebook"></a><span data-ttu-id="b99eb-103">Notizbuch abrufen</span><span class="sxs-lookup"><span data-stu-id="b99eb-103">Get notebook</span></span>

> <span data-ttu-id="b99eb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b99eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b99eb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b99eb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b99eb-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [notebook](../resources/notebook.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="b99eb-106">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b99eb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b99eb-107">Permissions</span></span>
<span data-ttu-id="b99eb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b99eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b99eb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b99eb-110">Permission type</span></span>      | <span data-ttu-id="b99eb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b99eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b99eb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b99eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b99eb-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b99eb-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b99eb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b99eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b99eb-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b99eb-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b99eb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b99eb-116">Application</span></span> | <span data-ttu-id="b99eb-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b99eb-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b99eb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b99eb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b99eb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b99eb-119">Optional query parameters</span></span>
<span data-ttu-id="b99eb-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b99eb-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b99eb-121">Gültige `expand`-Werte für Notizbücher sind `sections` und `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="b99eb-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b99eb-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b99eb-122">Request headers</span></span>
| <span data-ttu-id="b99eb-123">Name</span><span class="sxs-lookup"><span data-stu-id="b99eb-123">Name</span></span>       | <span data-ttu-id="b99eb-124">Typ</span><span class="sxs-lookup"><span data-stu-id="b99eb-124">Type</span></span> | <span data-ttu-id="b99eb-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b99eb-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b99eb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b99eb-126">Authorization</span></span>  | <span data-ttu-id="b99eb-127">string</span><span class="sxs-lookup"><span data-stu-id="b99eb-127">string</span></span>  | <span data-ttu-id="b99eb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b99eb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b99eb-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b99eb-130">Accept</span></span> | <span data-ttu-id="b99eb-131">string</span><span class="sxs-lookup"><span data-stu-id="b99eb-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b99eb-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b99eb-132">Request body</span></span>
<span data-ttu-id="b99eb-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b99eb-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b99eb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b99eb-134">Response</span></span>

<span data-ttu-id="b99eb-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b99eb-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b99eb-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b99eb-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b99eb-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b99eb-137">Request</span></span>
<span data-ttu-id="b99eb-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b99eb-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="b99eb-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b99eb-139">Response</span></span>
<span data-ttu-id="b99eb-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b99eb-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
