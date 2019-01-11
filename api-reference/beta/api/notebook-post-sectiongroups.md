---
title: sectionGroup erstellen
description: Mit dieser API können Sie eine neue Abschnittsgruppe in dem jeweils angegebenen Notizbuch erstellen.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 85e971719fd3074d78ab8ca857d6db324174c714
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875278"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="374cd-103">sectionGroup erstellen</span><span class="sxs-lookup"><span data-stu-id="374cd-103">Create sectionGroup</span></span>

> <span data-ttu-id="374cd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="374cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="374cd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="374cd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="374cd-106">Mit dieser API können Sie eine neue [Abschnittsgruppe](../resources/sectiongroup.md) in dem jeweils angegebenen Notizbuch erstellen.</span><span class="sxs-lookup"><span data-stu-id="374cd-106">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="374cd-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="374cd-107">Permissions</span></span>
<span data-ttu-id="374cd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="374cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="374cd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="374cd-110">Permission type</span></span>      | <span data-ttu-id="374cd-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="374cd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="374cd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="374cd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="374cd-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="374cd-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="374cd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="374cd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="374cd-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="374cd-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="374cd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="374cd-116">Application</span></span> | <span data-ttu-id="374cd-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="374cd-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="374cd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="374cd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="374cd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="374cd-119">Request headers</span></span>
| <span data-ttu-id="374cd-120">Name</span><span class="sxs-lookup"><span data-stu-id="374cd-120">Name</span></span>       | <span data-ttu-id="374cd-121">Typ</span><span class="sxs-lookup"><span data-stu-id="374cd-121">Type</span></span> | <span data-ttu-id="374cd-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="374cd-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="374cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="374cd-123">Authorization</span></span>  | <span data-ttu-id="374cd-124">string</span><span class="sxs-lookup"><span data-stu-id="374cd-124">string</span></span>  | <span data-ttu-id="374cd-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="374cd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="374cd-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="374cd-127">Content-Type</span></span> | <span data-ttu-id="374cd-128">string</span><span class="sxs-lookup"><span data-stu-id="374cd-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="374cd-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="374cd-129">Request body</span></span>
<span data-ttu-id="374cd-130">Geben Sie im Anforderungstext einen Namen für die Abschnittsgruppe an.</span><span class="sxs-lookup"><span data-stu-id="374cd-130">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="374cd-p104">Innerhalb der gleichen Hierarchieebene müssen Abschnittsgruppennamen eindeutig sein. Der Name darf nicht mehr als 50 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="374cd-p104">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="374cd-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="374cd-133">Response</span></span>

<span data-ttu-id="374cd-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [sectionGroup](../resources/sectiongroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="374cd-134">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="374cd-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="374cd-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="374cd-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="374cd-136">Request</span></span>
<span data-ttu-id="374cd-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="374cd-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```

##### <a name="response"></a><span data-ttu-id="374cd-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="374cd-138">Response</span></span>
<span data-ttu-id="374cd-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="374cd-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

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
