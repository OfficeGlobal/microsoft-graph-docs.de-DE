---
title: Abschnitt abrufen
description: Rufen Sie die Eigenschaften und die Beziehungen eines OnenoteSection-Objekts ab.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: d491e0936096296c731e2ebbbc1d6d44dccdef38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941555"
---
# <a name="get-section"></a><span data-ttu-id="80fa6-103">Abschnitt abrufen</span><span class="sxs-lookup"><span data-stu-id="80fa6-103">Get section</span></span>

<span data-ttu-id="80fa6-104">Rufen Sie die Eigenschaften und die Beziehungen eines [OnenoteSection](../resources/section.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="80fa6-104">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="80fa6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="80fa6-105">Permissions</span></span>
<span data-ttu-id="80fa6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80fa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80fa6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80fa6-108">Permission type</span></span>      | <span data-ttu-id="80fa6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80fa6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80fa6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80fa6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80fa6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80fa6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="80fa6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80fa6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80fa6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80fa6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="80fa6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80fa6-114">Application</span></span> | <span data-ttu-id="80fa6-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80fa6-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80fa6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80fa6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="80fa6-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="80fa6-117">Optional query parameters</span></span>
<span data-ttu-id="80fa6-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="80fa6-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="80fa6-p102">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `displayName` und `self` aus. Gültige `expand`-Werte für Abschnitte sind `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="80fa6-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80fa6-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80fa6-121">Request headers</span></span>
| <span data-ttu-id="80fa6-122">Name</span><span class="sxs-lookup"><span data-stu-id="80fa6-122">Name</span></span>       | <span data-ttu-id="80fa6-123">Typ</span><span class="sxs-lookup"><span data-stu-id="80fa6-123">Type</span></span> | <span data-ttu-id="80fa6-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80fa6-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="80fa6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="80fa6-125">Authorization</span></span>  | <span data-ttu-id="80fa6-126">string</span><span class="sxs-lookup"><span data-stu-id="80fa6-126">string</span></span>  | <span data-ttu-id="80fa6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80fa6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80fa6-129">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80fa6-129">Accept</span></span> | <span data-ttu-id="80fa6-130">string</span><span class="sxs-lookup"><span data-stu-id="80fa6-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="80fa6-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80fa6-131">Request body</span></span>
<span data-ttu-id="80fa6-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="80fa6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80fa6-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="80fa6-133">Response</span></span>

<span data-ttu-id="80fa6-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [OnenoteSection](../resources/section.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="80fa6-134">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="80fa6-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80fa6-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80fa6-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80fa6-136">Request</span></span>
<span data-ttu-id="80fa6-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80fa6-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="80fa6-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="80fa6-138">Response</span></span>
<span data-ttu-id="80fa6-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80fa6-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
