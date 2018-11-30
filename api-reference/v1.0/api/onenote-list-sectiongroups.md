---
title: sectionGroups auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs sectionGroup abrufen.
ms.openlocfilehash: 79f62fc91b97ce06aebab35ccc9308e6cfac5a3d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017744"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="ff537-103">sectionGroups auflisten</span><span class="sxs-lookup"><span data-stu-id="ff537-103">List sectionGroups</span></span>

<span data-ttu-id="ff537-104">Mit dieser API können Sie eine Liste von Objekten des Typs [sectionGroup](../resources/sectiongroup.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="ff537-104">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff537-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ff537-105">Permissions</span></span>
<span data-ttu-id="ff537-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff537-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff537-108">Permission type</span></span>      | <span data-ttu-id="ff537-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff537-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff537-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff537-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff537-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff537-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff537-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff537-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff537-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff537-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ff537-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff537-114">Application</span></span> | <span data-ttu-id="ff537-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff537-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff537-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff537-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ff537-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ff537-117">Optional query parameters</span></span>
<span data-ttu-id="ff537-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ff537-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ff537-119">Die Standardsortierreihenfolge ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="ff537-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="ff537-p102">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `displayName` und `self` aus. Gültige `expand`-Werte für Abschnittsgruppen sind `sections`, `sectionGroups`, `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="ff537-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff537-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff537-122">Request headers</span></span>
| <span data-ttu-id="ff537-123">Name</span><span class="sxs-lookup"><span data-stu-id="ff537-123">Name</span></span>       | <span data-ttu-id="ff537-124">Typ</span><span class="sxs-lookup"><span data-stu-id="ff537-124">Type</span></span> | <span data-ttu-id="ff537-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff537-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ff537-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff537-126">Authorization</span></span>  | <span data-ttu-id="ff537-127">string</span><span class="sxs-lookup"><span data-stu-id="ff537-127">string</span></span>  | <span data-ttu-id="ff537-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ff537-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff537-130">Accept</span><span class="sxs-lookup"><span data-stu-id="ff537-130">Accept</span></span> | <span data-ttu-id="ff537-131">string</span><span class="sxs-lookup"><span data-stu-id="ff537-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ff537-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff537-132">Request body</span></span>
<span data-ttu-id="ff537-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ff537-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff537-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff537-134">Response</span></span>

<span data-ttu-id="ff537-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [sectionGroup](../resources/sectiongroup.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff537-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff537-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff537-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff537-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff537-137">Request</span></span>
<span data-ttu-id="ff537-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff537-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="ff537-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff537-139">Response</span></span>
<span data-ttu-id="ff537-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff537-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
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