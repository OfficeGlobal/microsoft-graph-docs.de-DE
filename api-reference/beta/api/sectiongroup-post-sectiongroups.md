---
title: sectionGroup erstellen
description: Mit dieser API können Sie eine neue Abschnittsgruppe in der angegebenen Abschnittsgruppe erstellen.
ms.openlocfilehash: 62e88f65755006fb6cbb4755cd63ef02fbc19556
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061315"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="71f86-103">sectionGroup erstellen</span><span class="sxs-lookup"><span data-stu-id="71f86-103">Create sectionGroup</span></span>

> <span data-ttu-id="71f86-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="71f86-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71f86-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71f86-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71f86-106">Mit dieser API können Sie eine neue [Abschnittsgruppe](../resources/sectiongroup.md) in der angegebenen Abschnittsgruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="71f86-106">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="71f86-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="71f86-107">Permissions</span></span>
<span data-ttu-id="71f86-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71f86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71f86-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71f86-110">Permission type</span></span>      | <span data-ttu-id="71f86-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71f86-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71f86-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71f86-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71f86-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f86-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="71f86-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71f86-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71f86-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71f86-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="71f86-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71f86-116">Application</span></span> | <span data-ttu-id="71f86-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f86-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71f86-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71f86-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="71f86-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71f86-119">Request headers</span></span>
| <span data-ttu-id="71f86-120">Name</span><span class="sxs-lookup"><span data-stu-id="71f86-120">Name</span></span>       | <span data-ttu-id="71f86-121">Typ</span><span class="sxs-lookup"><span data-stu-id="71f86-121">Type</span></span> | <span data-ttu-id="71f86-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71f86-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71f86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71f86-123">Authorization</span></span>  | <span data-ttu-id="71f86-124">string</span><span class="sxs-lookup"><span data-stu-id="71f86-124">string</span></span>  | <span data-ttu-id="71f86-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71f86-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71f86-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71f86-127">Content-Type</span></span> | <span data-ttu-id="71f86-128">string</span><span class="sxs-lookup"><span data-stu-id="71f86-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="71f86-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71f86-129">Request body</span></span>
<span data-ttu-id="71f86-130">Geben Sie im Anforderungstext einen Namen für die Abschnittsgruppe an.</span><span class="sxs-lookup"><span data-stu-id="71f86-130">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="71f86-p104">Innerhalb der gleichen Hierarchieebene müssen Abschnittsgruppennamen eindeutig sein. Der Name darf nicht mehr als 50 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="71f86-p104">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="71f86-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="71f86-133">Response</span></span>

<span data-ttu-id="71f86-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [sectionGroup](../resources/sectiongroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71f86-134">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71f86-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71f86-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71f86-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71f86-136">Request</span></span>
<span data-ttu-id="71f86-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71f86-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="71f86-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="71f86-138">Response</span></span>
<span data-ttu-id="71f86-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71f86-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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