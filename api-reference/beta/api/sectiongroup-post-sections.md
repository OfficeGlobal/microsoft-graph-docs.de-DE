---
title: Abschnitt erstellen
description: Mit dieser API können Sie eine neue Ressource des Typs section in der angegebenen Abschnittsgruppe erstellen.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 25c66aa1b1db1f40e3cd9d2b9902288f36ccd766
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510505"
---
# <a name="create-section"></a><span data-ttu-id="9a106-103">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="9a106-103">Create section</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a106-104">Mit dieser API können Sie eine neue Ressource des Typs [section](../resources/section.md) in der angegebenen Abschnittsgruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="9a106-104">Create a new [section](../resources/section.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a106-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9a106-105">Permissions</span></span>
<span data-ttu-id="9a106-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a106-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a106-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a106-108">Permission type</span></span>      | <span data-ttu-id="9a106-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a106-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a106-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a106-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a106-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a106-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a106-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a106-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a106-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a106-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9a106-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a106-114">Application</span></span> | <span data-ttu-id="9a106-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a106-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a106-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a106-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="9a106-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a106-117">Request headers</span></span>
| <span data-ttu-id="9a106-118">Name</span><span class="sxs-lookup"><span data-stu-id="9a106-118">Name</span></span>       | <span data-ttu-id="9a106-119">Typ</span><span class="sxs-lookup"><span data-stu-id="9a106-119">Type</span></span> | <span data-ttu-id="9a106-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a106-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a106-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a106-121">Authorization</span></span>  | <span data-ttu-id="9a106-122">string</span><span class="sxs-lookup"><span data-stu-id="9a106-122">string</span></span>  | <span data-ttu-id="9a106-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a106-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a106-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a106-125">Content-Type</span></span> | <span data-ttu-id="9a106-126">string</span><span class="sxs-lookup"><span data-stu-id="9a106-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9a106-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a106-127">Request body</span></span>
<span data-ttu-id="9a106-128">Geben Sie im Anforderungstext einen Namen für den Abschnitt an.</span><span class="sxs-lookup"><span data-stu-id="9a106-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="9a106-p103">Innerhalb der gleichen Hierarchieebene müssen Abschnittsnamen eindeutig sein. Der Name darf nicht mehr als 50 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="9a106-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="9a106-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a106-131">Response</span></span>

<span data-ttu-id="9a106-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [section](../resources/section.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a106-132">If successful, this method returns a `201 Created` response code and a [section](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a106-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a106-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a106-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a106-134">Request</span></span>
<span data-ttu-id="9a106-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a106-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```

##### <a name="response"></a><span data-ttu-id="9a106-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a106-136">Response</span></span>
<span data-ttu-id="9a106-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a106-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/sectiongroup-post-sections.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
