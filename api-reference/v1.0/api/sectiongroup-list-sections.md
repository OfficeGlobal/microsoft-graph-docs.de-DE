---
title: Abschnitte auflisten
description: Abrufen einer Liste von OnenoteSection-Objekten aus der angegebenen Abschnittsgruppe.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8c29ec47ef322c205a8c62a4074c5fec84de6c14
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948709"
---
# <a name="list-sections"></a><span data-ttu-id="d85d1-103">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="d85d1-103">List sections</span></span>

<span data-ttu-id="d85d1-104">Abrufen einer Liste von [OnenoteSection](../resources/section.md) -Objekten aus der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="d85d1-104">Retrieve a list of [onenoteSection](../resources/section.md) objects from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="d85d1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d85d1-105">Permissions</span></span>
<span data-ttu-id="d85d1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d85d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d85d1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d85d1-108">Permission type</span></span>      | <span data-ttu-id="d85d1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d85d1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d85d1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d85d1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d85d1-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d85d1-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d85d1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d85d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d85d1-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d85d1-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d85d1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d85d1-114">Application</span></span> | <span data-ttu-id="d85d1-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d85d1-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d85d1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d85d1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d85d1-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d85d1-117">Optional query parameters</span></span>
<span data-ttu-id="d85d1-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d85d1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d85d1-119">Die Standardsortierreihenfolge ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="d85d1-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="d85d1-p102">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `displayName` und `self` aus. Gültige `expand`-Werte für Abschnitte sind `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="d85d1-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d85d1-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d85d1-122">Request headers</span></span>
| <span data-ttu-id="d85d1-123">Name</span><span class="sxs-lookup"><span data-stu-id="d85d1-123">Name</span></span>       | <span data-ttu-id="d85d1-124">Typ</span><span class="sxs-lookup"><span data-stu-id="d85d1-124">Type</span></span> | <span data-ttu-id="d85d1-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d85d1-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d85d1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d85d1-126">Authorization</span></span>  | <span data-ttu-id="d85d1-127">string</span><span class="sxs-lookup"><span data-stu-id="d85d1-127">string</span></span>  | <span data-ttu-id="d85d1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d85d1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d85d1-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d85d1-130">Accept</span></span> | <span data-ttu-id="d85d1-131">string</span><span class="sxs-lookup"><span data-stu-id="d85d1-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d85d1-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d85d1-132">Request body</span></span>
<span data-ttu-id="d85d1-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d85d1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d85d1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d85d1-134">Response</span></span>

<span data-ttu-id="d85d1-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [OnenoteSection](../resources/section.md) .</span><span class="sxs-lookup"><span data-stu-id="d85d1-135">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d85d1-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d85d1-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d85d1-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d85d1-137">Request</span></span>
<span data-ttu-id="d85d1-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d85d1-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="d85d1-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d85d1-139">Response</span></span>
<span data-ttu-id="d85d1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d85d1-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
