---
title: Abschnitt erstellen
description: Erstellen Sie eine neue OnenoteSection in der angegebenen Abschnittsgruppe aus.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 91ed02c363de0fc39af594e2e0932e4c4ad605bf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947078"
---
# <a name="create-section"></a><span data-ttu-id="e99ab-103">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="e99ab-103">Create section</span></span>

<span data-ttu-id="e99ab-104">Erstellen Sie eine neue [OnenoteSection](../resources/section.md) in der angegebenen Abschnittsgruppe aus.</span><span class="sxs-lookup"><span data-stu-id="e99ab-104">Create a new [onenoteSection](../resources/section.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="e99ab-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e99ab-105">Permissions</span></span>
<span data-ttu-id="e99ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e99ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e99ab-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e99ab-108">Permission type</span></span>      | <span data-ttu-id="e99ab-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e99ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e99ab-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e99ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e99ab-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e99ab-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e99ab-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e99ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e99ab-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e99ab-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e99ab-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e99ab-114">Application</span></span> | <span data-ttu-id="e99ab-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e99ab-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e99ab-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e99ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="e99ab-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e99ab-117">Request headers</span></span>
| <span data-ttu-id="e99ab-118">Name</span><span class="sxs-lookup"><span data-stu-id="e99ab-118">Name</span></span>       | <span data-ttu-id="e99ab-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e99ab-119">Type</span></span> | <span data-ttu-id="e99ab-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e99ab-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e99ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e99ab-121">Authorization</span></span>  | <span data-ttu-id="e99ab-122">string</span><span class="sxs-lookup"><span data-stu-id="e99ab-122">string</span></span>  | <span data-ttu-id="e99ab-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e99ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e99ab-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e99ab-125">Content-Type</span></span> | <span data-ttu-id="e99ab-126">string</span><span class="sxs-lookup"><span data-stu-id="e99ab-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e99ab-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e99ab-127">Request body</span></span>
<span data-ttu-id="e99ab-128">Geben Sie im Anforderungstext einen Namen für den Abschnitt an.</span><span class="sxs-lookup"><span data-stu-id="e99ab-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="e99ab-p103">Innerhalb der gleichen Hierarchieebene müssen Abschnittsnamen eindeutig sein. Der Name darf nicht mehr als 50 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="e99ab-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="e99ab-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e99ab-131">Response</span></span>

<span data-ttu-id="e99ab-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [OnenoteSection](../resources/section.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e99ab-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e99ab-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e99ab-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e99ab-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e99ab-134">Request</span></span>
<span data-ttu-id="e99ab-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e99ab-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```

##### <a name="response"></a><span data-ttu-id="e99ab-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e99ab-136">Response</span></span>
<span data-ttu-id="e99ab-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e99ab-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
