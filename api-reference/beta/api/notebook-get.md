---
title: Notizbuch abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs notebook abrufen.
ms.openlocfilehash: 9dd264dd2498e0c775629b9e178b7660426a8d69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065026"
---
# <a name="get-notebook"></a><span data-ttu-id="a3c18-103">Notizbuch abrufen</span><span class="sxs-lookup"><span data-stu-id="a3c18-103">Get notebook</span></span>

> <span data-ttu-id="a3c18-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a3c18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3c18-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a3c18-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3c18-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [notebook](../resources/notebook.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="a3c18-106">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3c18-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a3c18-107">Permissions</span></span>
<span data-ttu-id="a3c18-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3c18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3c18-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3c18-110">Permission type</span></span>      | <span data-ttu-id="a3c18-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3c18-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3c18-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3c18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a3c18-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c18-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3c18-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3c18-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3c18-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3c18-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a3c18-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3c18-116">Application</span></span> | <span data-ttu-id="a3c18-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c18-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3c18-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3c18-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a3c18-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a3c18-119">Optional query parameters</span></span>
<span data-ttu-id="a3c18-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a3c18-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a3c18-121">Gültige `expand`-Werte für Notizbücher sind `sections` und `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="a3c18-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3c18-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3c18-122">Request headers</span></span>
| <span data-ttu-id="a3c18-123">Name</span><span class="sxs-lookup"><span data-stu-id="a3c18-123">Name</span></span>       | <span data-ttu-id="a3c18-124">Typ</span><span class="sxs-lookup"><span data-stu-id="a3c18-124">Type</span></span> | <span data-ttu-id="a3c18-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3c18-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a3c18-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3c18-126">Authorization</span></span>  | <span data-ttu-id="a3c18-127">string</span><span class="sxs-lookup"><span data-stu-id="a3c18-127">string</span></span>  | <span data-ttu-id="a3c18-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a3c18-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3c18-130">Accept</span><span class="sxs-lookup"><span data-stu-id="a3c18-130">Accept</span></span> | <span data-ttu-id="a3c18-131">string</span><span class="sxs-lookup"><span data-stu-id="a3c18-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a3c18-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3c18-132">Request body</span></span>
<span data-ttu-id="a3c18-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a3c18-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3c18-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3c18-134">Response</span></span>

<span data-ttu-id="a3c18-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3c18-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a3c18-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3c18-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3c18-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3c18-137">Request</span></span>
<span data-ttu-id="a3c18-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3c18-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="a3c18-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3c18-139">Response</span></span>
<span data-ttu-id="a3c18-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3c18-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
