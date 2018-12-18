---
title: Erstellen Sie eine Einstellung für die Verzeichnis auf Gruppen
description: Verwenden Sie diese API, um eine neue Einstellung Verzeichnis für die Gruppe zu erstellen.
author: dkershaw10
ms.openlocfilehash: 2e400babc809bdc8d9277cad1bd41b8b714e4e92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358996"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="aedc4-103">Erstellen Sie eine Einstellung für die Verzeichnis auf Gruppen</span><span class="sxs-lookup"><span data-stu-id="aedc4-103">Create a directory setting on groups</span></span>

> <span data-ttu-id="aedc4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aedc4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aedc4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aedc4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aedc4-106">Verwenden Sie diese API, um eine neue Einstellung Verzeichnis für die Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="aedc4-106">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="aedc4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aedc4-107">Permissions</span></span>
<span data-ttu-id="aedc4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aedc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aedc4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aedc4-110">Permission type</span></span>      | <span data-ttu-id="aedc4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aedc4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aedc4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aedc4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aedc4-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aedc4-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aedc4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aedc4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aedc4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aedc4-115">Not supported.</span></span>    |
|<span data-ttu-id="aedc4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aedc4-116">Application</span></span> | <span data-ttu-id="aedc4-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aedc4-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aedc4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aedc4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="aedc4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aedc4-119">Request headers</span></span>
| <span data-ttu-id="aedc4-120">Name</span><span class="sxs-lookup"><span data-stu-id="aedc4-120">Name</span></span>       | <span data-ttu-id="aedc4-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aedc4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aedc4-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="aedc4-122">Authorization</span></span>  | <span data-ttu-id="aedc4-123">Bearer <token>.</span><span class="sxs-lookup"><span data-stu-id="aedc4-123">Bearer <token>.</span></span> <span data-ttu-id="aedc4-124">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="aedc4-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="aedc4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aedc4-125">Request body</span></span>
<span data-ttu-id="aedc4-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="aedc4-126">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aedc4-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="aedc4-127">Response</span></span>

<span data-ttu-id="aedc4-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Code und [Verzeichnisberechtigungen](../resources/directorysetting.md) Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="aedc4-128">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aedc4-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aedc4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aedc4-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aedc4-130">Request</span></span>
<span data-ttu-id="aedc4-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aedc4-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="aedc4-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="aedc4-132">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="aedc4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="aedc4-133">Response</span></span>
<span data-ttu-id="aedc4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aedc4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->