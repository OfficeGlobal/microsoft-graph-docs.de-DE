---
title: Abschnitt abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs section abrufen.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ce475e0bdd8b5557eb2b6c457c6736ac635eb0be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953399"
---
# <a name="get-section"></a><span data-ttu-id="1b18e-103">Abschnitt abrufen</span><span class="sxs-lookup"><span data-stu-id="1b18e-103">Get section</span></span>

> <span data-ttu-id="1b18e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1b18e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b18e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b18e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b18e-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [section](../resources/section.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="1b18e-106">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b18e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1b18e-107">Permissions</span></span>
<span data-ttu-id="1b18e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b18e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b18e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b18e-110">Permission type</span></span>      | <span data-ttu-id="1b18e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b18e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b18e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b18e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b18e-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b18e-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b18e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b18e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b18e-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b18e-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1b18e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b18e-116">Application</span></span> | <span data-ttu-id="1b18e-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b18e-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b18e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b18e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b18e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1b18e-119">Optional query parameters</span></span>
<span data-ttu-id="1b18e-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1b18e-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1b18e-p103">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `displayName` und `self` aus. Gültige `expand`-Werte für Abschnitte sind `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="1b18e-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b18e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b18e-123">Request headers</span></span>
| <span data-ttu-id="1b18e-124">Name</span><span class="sxs-lookup"><span data-stu-id="1b18e-124">Name</span></span>       | <span data-ttu-id="1b18e-125">Typ</span><span class="sxs-lookup"><span data-stu-id="1b18e-125">Type</span></span> | <span data-ttu-id="1b18e-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b18e-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1b18e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b18e-127">Authorization</span></span>  | <span data-ttu-id="1b18e-128">string</span><span class="sxs-lookup"><span data-stu-id="1b18e-128">string</span></span>  | <span data-ttu-id="1b18e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1b18e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b18e-131">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1b18e-131">Accept</span></span> | <span data-ttu-id="1b18e-132">string</span><span class="sxs-lookup"><span data-stu-id="1b18e-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1b18e-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b18e-133">Request body</span></span>
<span data-ttu-id="1b18e-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1b18e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b18e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b18e-135">Response</span></span>

<span data-ttu-id="1b18e-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [section](../resources/section.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b18e-136">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b18e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b18e-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b18e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b18e-138">Request</span></span>
<span data-ttu-id="1b18e-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b18e-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="1b18e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b18e-140">Response</span></span>
<span data-ttu-id="1b18e-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b18e-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
