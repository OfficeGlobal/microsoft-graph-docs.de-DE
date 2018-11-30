---
title: sectionGroups auflisten
description: Mit dieser API können Sie eine Liste von Abschnittsgruppen aus dem angegebenen Notizbuch abrufen.
ms.openlocfilehash: cdb5ef5b1c98f9e1632ef1cd7c6c5d5885e8d682
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061010"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="3db71-103">sectionGroups auflisten</span><span class="sxs-lookup"><span data-stu-id="3db71-103">List sectionGroups</span></span>

> <span data-ttu-id="3db71-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3db71-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3db71-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3db71-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3db71-106">Mit dieser API können Sie eine Liste von [Abschnittsgruppen](../resources/sectiongroup.md) aus dem angegebenen Notizbuch abrufen.</span><span class="sxs-lookup"><span data-stu-id="3db71-106">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="3db71-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3db71-107">Permissions</span></span>
<span data-ttu-id="3db71-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3db71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3db71-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3db71-110">Permission type</span></span>      | <span data-ttu-id="3db71-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3db71-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3db71-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3db71-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3db71-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3db71-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3db71-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3db71-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3db71-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db71-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3db71-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3db71-116">Application</span></span> | <span data-ttu-id="3db71-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3db71-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3db71-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3db71-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3db71-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3db71-119">Optional query parameters</span></span>
<span data-ttu-id="3db71-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3db71-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="3db71-121">Die Standardsortierreihenfolge ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="3db71-121">The default sort order is `name asc`.</span></span>

<span data-ttu-id="3db71-p103">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `displayName` und `self` aus. Gültige `expand`-Werte für Abschnittsgruppen sind `sections`, `sectionGroups`, `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="3db71-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3db71-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3db71-124">Request headers</span></span>
| <span data-ttu-id="3db71-125">Name</span><span class="sxs-lookup"><span data-stu-id="3db71-125">Name</span></span>       | <span data-ttu-id="3db71-126">Typ</span><span class="sxs-lookup"><span data-stu-id="3db71-126">Type</span></span> | <span data-ttu-id="3db71-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3db71-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3db71-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="3db71-128">Authorization</span></span>  | <span data-ttu-id="3db71-129">string</span><span class="sxs-lookup"><span data-stu-id="3db71-129">string</span></span>  | <span data-ttu-id="3db71-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3db71-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3db71-132">Accept</span><span class="sxs-lookup"><span data-stu-id="3db71-132">Accept</span></span> | <span data-ttu-id="3db71-133">string</span><span class="sxs-lookup"><span data-stu-id="3db71-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3db71-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3db71-134">Request body</span></span>
<span data-ttu-id="3db71-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3db71-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3db71-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3db71-136">Response</span></span>

<span data-ttu-id="3db71-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [sectionGroup](../resources/sectiongroup.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3db71-137">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3db71-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3db71-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3db71-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3db71-139">Request</span></span>
<span data-ttu-id="3db71-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3db71-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="3db71-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="3db71-141">Response</span></span>
<span data-ttu-id="3db71-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3db71-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
    {
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "displayName": "name-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->