---
title: sectionGroup abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs sectionGroup abrufen.
localization_priority: Normal
ms.openlocfilehash: e89460b45c03e35e36ab320433981eb0b60b3c7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878128"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="b3d16-103">sectionGroup abrufen</span><span class="sxs-lookup"><span data-stu-id="b3d16-103">Get sectionGroup</span></span>

> <span data-ttu-id="b3d16-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3d16-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3d16-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3d16-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3d16-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [sectionGroup](../resources/sectiongroup.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="b3d16-106">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3d16-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b3d16-107">Permissions</span></span>
<span data-ttu-id="b3d16-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3d16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3d16-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3d16-110">Permission type</span></span>      | <span data-ttu-id="b3d16-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3d16-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3d16-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3d16-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b3d16-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d16-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3d16-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3d16-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3d16-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3d16-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b3d16-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3d16-116">Application</span></span> | <span data-ttu-id="b3d16-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d16-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3d16-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3d16-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3d16-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b3d16-119">Optional query parameters</span></span>
<span data-ttu-id="b3d16-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b3d16-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b3d16-p103">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `name` und `self` aus. Gültige `expand`-Werte für Abschnittsgruppen sind `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="b3d16-p103">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3d16-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3d16-123">Request headers</span></span>
| <span data-ttu-id="b3d16-124">Name</span><span class="sxs-lookup"><span data-stu-id="b3d16-124">Name</span></span>       | <span data-ttu-id="b3d16-125">Typ</span><span class="sxs-lookup"><span data-stu-id="b3d16-125">Type</span></span> | <span data-ttu-id="b3d16-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3d16-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b3d16-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3d16-127">Authorization</span></span>  | <span data-ttu-id="b3d16-128">string</span><span class="sxs-lookup"><span data-stu-id="b3d16-128">string</span></span>  | <span data-ttu-id="b3d16-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b3d16-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3d16-131">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b3d16-131">Accept</span></span> | <span data-ttu-id="b3d16-132">string</span><span class="sxs-lookup"><span data-stu-id="b3d16-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b3d16-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3d16-133">Request body</span></span>
<span data-ttu-id="b3d16-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b3d16-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3d16-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3d16-135">Response</span></span>

<span data-ttu-id="b3d16-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [sectionGroup](../resources/sectiongroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3d16-136">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3d16-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3d16-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3d16-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3d16-138">Request</span></span>
<span data-ttu-id="b3d16-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3d16-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="b3d16-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3d16-140">Response</span></span>
<span data-ttu-id="b3d16-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3d16-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
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
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
