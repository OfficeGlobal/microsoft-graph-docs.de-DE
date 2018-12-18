---
title: Erstellen der Anlage
description: Verwenden Sie diese API, um eine Anlage zu einer OutlookTask hinzuzufügen.
author: angelgolfer-ms
ms.openlocfilehash: 9b4f74ee469783cd6e143446cd3fc28f28000aa8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355685"
---
# <a name="create-attachment"></a><span data-ttu-id="f00c5-103">Anlage erstellen</span><span class="sxs-lookup"><span data-stu-id="f00c5-103">Create attachment</span></span>

> <span data-ttu-id="f00c5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f00c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f00c5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f00c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f00c5-106">Verwenden Sie diese API, um eine [OutlookTask](../resources/outlooktask.md)eine [Anlage](../resources/attachment.md) hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f00c5-106">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f00c5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f00c5-107">Permissions</span></span>
<span data-ttu-id="f00c5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f00c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f00c5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f00c5-110">Permission type</span></span>      | <span data-ttu-id="f00c5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f00c5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f00c5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f00c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f00c5-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f00c5-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f00c5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f00c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f00c5-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f00c5-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f00c5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f00c5-116">Application</span></span> | <span data-ttu-id="f00c5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f00c5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f00c5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f00c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}/attachments

```
## <a name="request-headers"></a><span data-ttu-id="f00c5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f00c5-119">Request headers</span></span>
| <span data-ttu-id="f00c5-120">Name</span><span class="sxs-lookup"><span data-stu-id="f00c5-120">Name</span></span>       | <span data-ttu-id="f00c5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f00c5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f00c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f00c5-122">Authorization</span></span>  | <span data-ttu-id="f00c5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f00c5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f00c5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f00c5-125">Content-Type</span></span> | <span data-ttu-id="f00c5-126">Eine Zeichenfolge, die den Typ der Daten im Textkörper einer Entität darstellt.</span><span class="sxs-lookup"><span data-stu-id="f00c5-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="f00c5-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f00c5-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f00c5-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f00c5-128">Request body</span></span>
<span data-ttu-id="f00c5-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f00c5-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f00c5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f00c5-130">Response</span></span>

<span data-ttu-id="f00c5-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f00c5-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f00c5-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f00c5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f00c5-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f00c5-133">Request</span></span>
<span data-ttu-id="f00c5-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f00c5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_attachment_from_outlooktask"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true
}
```
<span data-ttu-id="f00c5-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f00c5-135">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f00c5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f00c5-136">Response</span></span>
<span data-ttu-id="f00c5-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f00c5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->