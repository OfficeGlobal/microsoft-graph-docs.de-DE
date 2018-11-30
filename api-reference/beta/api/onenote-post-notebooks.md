---
title: Notizbuch erstellen
description: Mit dieser API können Sie eine neue OneNote-Ressource des Typs notebook erstellen.
ms.openlocfilehash: b1f32bc8aadb5e5ec42e751453535b3ef116e907
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066171"
---
# <a name="create-notebook"></a><span data-ttu-id="c45b7-103">Notizbuch erstellen</span><span class="sxs-lookup"><span data-stu-id="c45b7-103">Create notebook</span></span>

> <span data-ttu-id="c45b7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c45b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c45b7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c45b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c45b7-106">Mit dieser API können Sie eine neue OneNote-Ressource des Typs [notebook](../resources/notebook.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c45b7-106">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c45b7-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c45b7-107">Permissions</span></span>
<span data-ttu-id="c45b7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c45b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c45b7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c45b7-110">Permission type</span></span>      | <span data-ttu-id="c45b7-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c45b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c45b7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c45b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c45b7-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c45b7-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c45b7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c45b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c45b7-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c45b7-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c45b7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c45b7-116">Application</span></span> | <span data-ttu-id="c45b7-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c45b7-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c45b7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c45b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="c45b7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c45b7-119">Request headers</span></span>
| <span data-ttu-id="c45b7-120">Name</span><span class="sxs-lookup"><span data-stu-id="c45b7-120">Name</span></span>       | <span data-ttu-id="c45b7-121">Typ</span><span class="sxs-lookup"><span data-stu-id="c45b7-121">Type</span></span> | <span data-ttu-id="c45b7-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c45b7-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c45b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c45b7-123">Authorization</span></span>  | <span data-ttu-id="c45b7-124">string</span><span class="sxs-lookup"><span data-stu-id="c45b7-124">string</span></span>  | <span data-ttu-id="c45b7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c45b7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c45b7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c45b7-127">Content-Type</span></span> | <span data-ttu-id="c45b7-128">string</span><span class="sxs-lookup"><span data-stu-id="c45b7-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c45b7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c45b7-129">Request body</span></span>
<span data-ttu-id="c45b7-130">Geben Sie im Anforderungstext einen Namen für das Notizbuch an.</span><span class="sxs-lookup"><span data-stu-id="c45b7-130">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="c45b7-p104">Notizbuchnamen müssen eindeutig sein. Der Name darf nicht mehr als 128 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="c45b7-p104">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="c45b7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c45b7-133">Response</span></span>

<span data-ttu-id="c45b7-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das neue [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c45b7-134">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c45b7-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c45b7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c45b7-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c45b7-136">Request</span></span>
<span data-ttu-id="c45b7-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c45b7-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c45b7-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c45b7-138">Response</span></span>
<span data-ttu-id="c45b7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c45b7-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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