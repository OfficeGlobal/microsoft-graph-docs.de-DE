---
title: sectionGroups auflisten
description: Mit dieser API können Sie eine Liste von Abschnittsgruppen aus der angegebenen Abschnittsgruppe abrufen.
ms.openlocfilehash: 11bdb6704a19fef2e704c8b7037ff1a5e33b36ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018234"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="8634e-103">sectionGroups auflisten</span><span class="sxs-lookup"><span data-stu-id="8634e-103">List sectionGroups</span></span>

<span data-ttu-id="8634e-104">Mit dieser API können Sie eine Liste von [Abschnittsgruppen](../resources/sectiongroup.md) aus der angegebenen Abschnittsgruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="8634e-104">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="8634e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8634e-105">Permissions</span></span>
<span data-ttu-id="8634e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8634e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8634e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8634e-108">Permission type</span></span>      | <span data-ttu-id="8634e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8634e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8634e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8634e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8634e-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8634e-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8634e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8634e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8634e-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8634e-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8634e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8634e-114">Application</span></span> | <span data-ttu-id="8634e-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8634e-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8634e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8634e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
GET /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
GET /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8634e-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8634e-117">Optional query parameters</span></span>
<span data-ttu-id="8634e-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8634e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8634e-119">Die Standardsortierreihenfolge ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="8634e-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="8634e-p102">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `displayName` und `self` aus. Gültige `expand`-Werte für Abschnittsgruppen sind `sections`, `sectionGroups`, `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="8634e-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8634e-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8634e-122">Request headers</span></span>
| <span data-ttu-id="8634e-123">Name</span><span class="sxs-lookup"><span data-stu-id="8634e-123">Name</span></span>       | <span data-ttu-id="8634e-124">Typ</span><span class="sxs-lookup"><span data-stu-id="8634e-124">Type</span></span> | <span data-ttu-id="8634e-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8634e-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8634e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8634e-126">Authorization</span></span>  | <span data-ttu-id="8634e-127">string</span><span class="sxs-lookup"><span data-stu-id="8634e-127">string</span></span>  | <span data-ttu-id="8634e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8634e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8634e-130">Accept</span><span class="sxs-lookup"><span data-stu-id="8634e-130">Accept</span></span> | <span data-ttu-id="8634e-131">string</span><span class="sxs-lookup"><span data-stu-id="8634e-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8634e-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8634e-132">Request body</span></span>
<span data-ttu-id="8634e-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8634e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8634e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8634e-134">Response</span></span>

<span data-ttu-id="8634e-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [sectionGroup](../resources/sectiongroup.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8634e-135">If successful, this method returns a `200 OK` response code and a collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8634e-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8634e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8634e-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8634e-137">Request</span></span>
<span data-ttu-id="8634e-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8634e-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="8634e-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="8634e-139">Response</span></span>
<span data-ttu-id="8634e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8634e-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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