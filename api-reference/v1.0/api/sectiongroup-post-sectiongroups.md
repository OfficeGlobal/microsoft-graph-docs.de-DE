---
title: sectionGroup erstellen
description: Mit dieser API können Sie eine neue Abschnittsgruppe in der angegebenen Abschnittsgruppe erstellen.
localization_priority: Normal
ms.openlocfilehash: 1b07c108c3fcc53ddd1cea06320ce8bbd79c11c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821238"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="bc307-103">sectionGroup erstellen</span><span class="sxs-lookup"><span data-stu-id="bc307-103">Create sectionGroup</span></span>

<span data-ttu-id="bc307-104">Mit dieser API können Sie eine neue [Abschnittsgruppe](../resources/sectiongroup.md) in der angegebenen Abschnittsgruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="bc307-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc307-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc307-105">Permissions</span></span>
<span data-ttu-id="bc307-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc307-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc307-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc307-108">Permission type</span></span>      | <span data-ttu-id="bc307-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc307-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc307-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc307-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc307-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc307-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc307-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc307-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc307-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc307-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="bc307-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc307-114">Application</span></span> | <span data-ttu-id="bc307-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc307-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc307-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc307-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="bc307-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc307-117">Request headers</span></span>
| <span data-ttu-id="bc307-118">Name</span><span class="sxs-lookup"><span data-stu-id="bc307-118">Name</span></span>       | <span data-ttu-id="bc307-119">Typ</span><span class="sxs-lookup"><span data-stu-id="bc307-119">Type</span></span> | <span data-ttu-id="bc307-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc307-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bc307-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc307-121">Authorization</span></span>  | <span data-ttu-id="bc307-122">string</span><span class="sxs-lookup"><span data-stu-id="bc307-122">string</span></span>  | <span data-ttu-id="bc307-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc307-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc307-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc307-125">Content-Type</span></span> | <span data-ttu-id="bc307-126">string</span><span class="sxs-lookup"><span data-stu-id="bc307-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="bc307-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc307-127">Request body</span></span>
<span data-ttu-id="bc307-128">Geben Sie im Anforderungstext einen Namen für die Abschnittsgruppe an.</span><span class="sxs-lookup"><span data-stu-id="bc307-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="bc307-p103">Innerhalb der gleichen Hierarchieebene müssen Abschnittsgruppennamen eindeutig sein. Der Name darf nicht mehr als 50 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="bc307-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="bc307-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc307-131">Response</span></span>

<span data-ttu-id="bc307-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [sectionGroup](../resources/sectiongroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc307-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc307-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc307-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc307-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc307-134">Request</span></span>
<span data-ttu-id="bc307-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc307-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="bc307-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc307-136">Response</span></span>
<span data-ttu-id="bc307-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc307-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
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
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
