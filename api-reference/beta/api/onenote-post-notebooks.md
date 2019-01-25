---
title: Notizbuch erstellen
description: Mit dieser API können Sie eine neue OneNote-Ressource des Typs notebook erstellen.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: deeb775f19ba2378cd15ffcbd72ef2caafd23b83
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514824"
---
# <a name="create-notebook"></a><span data-ttu-id="3c052-103">Notizbuch erstellen</span><span class="sxs-lookup"><span data-stu-id="3c052-103">Create notebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c052-104">Mit dieser API können Sie eine neue OneNote-Ressource des Typs [notebook](../resources/notebook.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3c052-104">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3c052-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3c052-105">Permissions</span></span>
<span data-ttu-id="3c052-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c052-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c052-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3c052-108">Permission type</span></span>      | <span data-ttu-id="3c052-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3c052-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c052-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3c052-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c052-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c052-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c052-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3c052-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c052-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c052-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3c052-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c052-114">Application</span></span> | <span data-ttu-id="3c052-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c052-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c052-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c052-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="3c052-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3c052-117">Request headers</span></span>
| <span data-ttu-id="3c052-118">Name</span><span class="sxs-lookup"><span data-stu-id="3c052-118">Name</span></span>       | <span data-ttu-id="3c052-119">Typ</span><span class="sxs-lookup"><span data-stu-id="3c052-119">Type</span></span> | <span data-ttu-id="3c052-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c052-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c052-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c052-121">Authorization</span></span>  | <span data-ttu-id="3c052-122">string</span><span class="sxs-lookup"><span data-stu-id="3c052-122">string</span></span>  | <span data-ttu-id="3c052-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3c052-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c052-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c052-125">Content-Type</span></span> | <span data-ttu-id="3c052-126">string</span><span class="sxs-lookup"><span data-stu-id="3c052-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3c052-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3c052-127">Request body</span></span>
<span data-ttu-id="3c052-128">Geben Sie im Anforderungstext einen Namen für das Notizbuch an.</span><span class="sxs-lookup"><span data-stu-id="3c052-128">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="3c052-p103">Notizbuchnamen müssen eindeutig sein. Der Name darf nicht mehr als 128 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="3c052-p103">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="3c052-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c052-131">Response</span></span>

<span data-ttu-id="3c052-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das neue [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3c052-132">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c052-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3c052-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c052-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c052-134">Request</span></span>
<span data-ttu-id="3c052-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3c052-135">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3c052-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c052-136">Response</span></span>
<span data-ttu-id="3c052-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3c052-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/onenote-post-notebooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
