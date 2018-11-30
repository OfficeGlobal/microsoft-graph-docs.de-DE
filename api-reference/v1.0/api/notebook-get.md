---
title: Notizbuch abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs notebook abrufen.
ms.openlocfilehash: e00f9eb8f7ede1bc247d41dc466f58ededb1ecd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019196"
---
# <a name="get-notebook"></a><span data-ttu-id="96da2-103">Notizbuch abrufen</span><span class="sxs-lookup"><span data-stu-id="96da2-103">Get notebook</span></span>

<span data-ttu-id="96da2-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [notebook](../resources/notebook.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="96da2-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="96da2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="96da2-105">Permissions</span></span>
<span data-ttu-id="96da2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96da2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96da2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96da2-108">Permission type</span></span>      | <span data-ttu-id="96da2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96da2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96da2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96da2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96da2-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96da2-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="96da2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96da2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96da2-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96da2-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="96da2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96da2-114">Application</span></span> | <span data-ttu-id="96da2-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96da2-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96da2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96da2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96da2-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="96da2-117">Optional query parameters</span></span>
<span data-ttu-id="96da2-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="96da2-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="96da2-119">Gültige `expand`-Werte für Notizbücher sind `sections` und `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="96da2-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96da2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96da2-120">Request headers</span></span>
| <span data-ttu-id="96da2-121">Name</span><span class="sxs-lookup"><span data-stu-id="96da2-121">Name</span></span>       | <span data-ttu-id="96da2-122">Typ</span><span class="sxs-lookup"><span data-stu-id="96da2-122">Type</span></span> | <span data-ttu-id="96da2-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96da2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96da2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="96da2-124">Authorization</span></span>  | <span data-ttu-id="96da2-125">string</span><span class="sxs-lookup"><span data-stu-id="96da2-125">string</span></span>  | <span data-ttu-id="96da2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96da2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96da2-128">Accept</span><span class="sxs-lookup"><span data-stu-id="96da2-128">Accept</span></span> | <span data-ttu-id="96da2-129">string</span><span class="sxs-lookup"><span data-stu-id="96da2-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="96da2-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96da2-130">Request body</span></span>
<span data-ttu-id="96da2-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="96da2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96da2-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="96da2-132">Response</span></span>

<span data-ttu-id="96da2-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96da2-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96da2-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96da2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96da2-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96da2-135">Request</span></span>
<span data-ttu-id="96da2-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96da2-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="96da2-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="96da2-137">Response</span></span>
<span data-ttu-id="96da2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96da2-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
