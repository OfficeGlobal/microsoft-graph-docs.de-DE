---
title: Erstellen Sie eine Einstellung für die Verzeichnis auf Gruppen
description: Verwenden Sie diese API, um eine neue Einstellung Verzeichnis für die Gruppe zu erstellen.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3ba33de148e34ce80c0a709a6a1b5faf99d5f32d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515846"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="97a86-103">Erstellen Sie eine Einstellung für die Verzeichnis auf Gruppen</span><span class="sxs-lookup"><span data-stu-id="97a86-103">Create a directory setting on groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97a86-104">Verwenden Sie diese API, um eine neue Einstellung Verzeichnis für die Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="97a86-104">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="97a86-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97a86-105">Permissions</span></span>
<span data-ttu-id="97a86-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97a86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97a86-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97a86-108">Permission type</span></span>      | <span data-ttu-id="97a86-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97a86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97a86-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97a86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="97a86-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97a86-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="97a86-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97a86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97a86-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97a86-113">Not supported.</span></span>    |
|<span data-ttu-id="97a86-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97a86-114">Application</span></span> | <span data-ttu-id="97a86-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97a86-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97a86-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97a86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="97a86-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97a86-117">Request headers</span></span>
| <span data-ttu-id="97a86-118">Name</span><span class="sxs-lookup"><span data-stu-id="97a86-118">Name</span></span>       | <span data-ttu-id="97a86-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97a86-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97a86-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="97a86-120">Authorization</span></span>  | <span data-ttu-id="97a86-121">Bearer <token>.</span><span class="sxs-lookup"><span data-stu-id="97a86-121">Bearer <token>.</span></span> <span data-ttu-id="97a86-122">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="97a86-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="97a86-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97a86-123">Request body</span></span>
<span data-ttu-id="97a86-124">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="97a86-124">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="97a86-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="97a86-125">Response</span></span>

<span data-ttu-id="97a86-126">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Code und [Verzeichnisberechtigungen](../resources/directorysetting.md) Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="97a86-126">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97a86-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97a86-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97a86-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97a86-128">Request</span></span>
<span data-ttu-id="97a86-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97a86-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/settings
Content-type: application/json
Content-length: 222

{
  "directorySetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
<span data-ttu-id="97a86-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="97a86-130">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="97a86-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="97a86-131">Response</span></span>
<span data-ttu-id="97a86-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97a86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "directorySetting": {
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
