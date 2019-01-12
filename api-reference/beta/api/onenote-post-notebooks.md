---
title: Notizbuch erstellen
description: Mit dieser API können Sie eine neue OneNote-Ressource des Typs notebook erstellen.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d7f70f53abeb4c2fe759d43c2a9c0446bd6a1929
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944257"
---
# <a name="create-notebook"></a><span data-ttu-id="dacb1-103">Notizbuch erstellen</span><span class="sxs-lookup"><span data-stu-id="dacb1-103">Create notebook</span></span>

> <span data-ttu-id="dacb1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dacb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dacb1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dacb1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dacb1-106">Mit dieser API können Sie eine neue OneNote-Ressource des Typs [notebook](../resources/notebook.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="dacb1-106">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="dacb1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dacb1-107">Permissions</span></span>
<span data-ttu-id="dacb1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dacb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dacb1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dacb1-110">Permission type</span></span>      | <span data-ttu-id="dacb1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dacb1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dacb1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dacb1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dacb1-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dacb1-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="dacb1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dacb1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dacb1-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dacb1-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="dacb1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dacb1-116">Application</span></span> | <span data-ttu-id="dacb1-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dacb1-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dacb1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dacb1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="dacb1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dacb1-119">Request headers</span></span>
| <span data-ttu-id="dacb1-120">Name</span><span class="sxs-lookup"><span data-stu-id="dacb1-120">Name</span></span>       | <span data-ttu-id="dacb1-121">Typ</span><span class="sxs-lookup"><span data-stu-id="dacb1-121">Type</span></span> | <span data-ttu-id="dacb1-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dacb1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dacb1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dacb1-123">Authorization</span></span>  | <span data-ttu-id="dacb1-124">string</span><span class="sxs-lookup"><span data-stu-id="dacb1-124">string</span></span>  | <span data-ttu-id="dacb1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dacb1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dacb1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dacb1-127">Content-Type</span></span> | <span data-ttu-id="dacb1-128">string</span><span class="sxs-lookup"><span data-stu-id="dacb1-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="dacb1-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dacb1-129">Request body</span></span>
<span data-ttu-id="dacb1-130">Geben Sie im Anforderungstext einen Namen für das Notizbuch an.</span><span class="sxs-lookup"><span data-stu-id="dacb1-130">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="dacb1-p104">Notizbuchnamen müssen eindeutig sein. Der Name darf nicht mehr als 128 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="dacb1-p104">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="dacb1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="dacb1-133">Response</span></span>

<span data-ttu-id="dacb1-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das neue [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dacb1-134">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dacb1-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dacb1-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dacb1-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dacb1-136">Request</span></span>
<span data-ttu-id="dacb1-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dacb1-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="dacb1-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="dacb1-138">Response</span></span>
<span data-ttu-id="dacb1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dacb1-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
