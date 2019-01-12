---
title: Verzeichnisrollenmitglied hinzufügen
description: Mit dieser API können Sie ein neues Verzeichnisrollenmitglied erstellen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e0a5217f10fe0e1a3bd7bd13aec86c4565016a45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931489"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="8d527-103">Verzeichnisrollenmitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8d527-103">Add directory role member</span></span>

> <span data-ttu-id="8d527-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d527-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d527-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d527-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d527-106">Mit dieser API können Sie ein neues Verzeichnisrollenmitglied erstellen.</span><span class="sxs-lookup"><span data-stu-id="8d527-106">Use this API to create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d527-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8d527-107">Permissions</span></span>
<span data-ttu-id="8d527-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d527-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d527-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d527-110">Permission type</span></span>      | <span data-ttu-id="8d527-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d527-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d527-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d527-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d527-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d527-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8d527-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d527-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d527-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d527-115">Not supported.</span></span>    |
|<span data-ttu-id="8d527-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d527-116">Application</span></span> | <span data-ttu-id="8d527-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d527-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d527-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d527-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="8d527-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d527-119">Request headers</span></span>
| <span data-ttu-id="8d527-120">Name</span><span class="sxs-lookup"><span data-stu-id="8d527-120">Name</span></span>       | <span data-ttu-id="8d527-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8d527-121">Type</span></span> | <span data-ttu-id="8d527-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d527-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8d527-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d527-123">Authorization</span></span>  | <span data-ttu-id="8d527-124">string</span><span class="sxs-lookup"><span data-stu-id="8d527-124">string</span></span>  | <span data-ttu-id="8d527-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8d527-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d527-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d527-127">Request body</span></span>
<span data-ttu-id="8d527-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8d527-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8d527-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d527-129">Response</span></span>

<span data-ttu-id="8d527-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d527-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d527-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d527-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d527-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d527-132">Request</span></span>
<span data-ttu-id="8d527-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d527-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="8d527-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8d527-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8d527-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d527-135">Response</span></span>
<span data-ttu-id="8d527-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d527-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
