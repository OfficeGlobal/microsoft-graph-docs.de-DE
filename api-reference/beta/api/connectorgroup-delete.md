---
title: ConnectorGroup löschen
description: Löschen einer ConnectorGroup.
ms.openlocfilehash: 3ba4a5a06e25f2fb1568ab9d7d6e92104ea083de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059049"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="5079a-103">ConnectorGroup löschen</span><span class="sxs-lookup"><span data-stu-id="5079a-103">Delete connectorGroup</span></span>

> <span data-ttu-id="5079a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5079a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5079a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5079a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5079a-106">Löschen einer ConnectorGroup.</span><span class="sxs-lookup"><span data-stu-id="5079a-106">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="5079a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5079a-107">Permissions</span></span>
<span data-ttu-id="5079a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5079a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5079a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5079a-110">Permission type</span></span>      | <span data-ttu-id="5079a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5079a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5079a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5079a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5079a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5079a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5079a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5079a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5079a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5079a-115">Not supported.</span></span>    |
|<span data-ttu-id="5079a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5079a-116">Application</span></span> | <span data-ttu-id="5079a-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5079a-117">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="5079a-118">**Hinweis:** Die Gruppe Connectors darf keine Connectors zugeordnet haben.</span><span class="sxs-lookup"><span data-stu-id="5079a-118">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="5079a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5079a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5079a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5079a-120">Request headers</span></span>
| <span data-ttu-id="5079a-121">Name</span><span class="sxs-lookup"><span data-stu-id="5079a-121">Name</span></span>       | <span data-ttu-id="5079a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5079a-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5079a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5079a-123">Authorization</span></span>  | <span data-ttu-id="5079a-124">Bearer.</span><span class="sxs-lookup"><span data-stu-id="5079a-124">Bearer.</span></span> <span data-ttu-id="5079a-125">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="5079a-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="5079a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5079a-126">Request body</span></span>
<span data-ttu-id="5079a-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5079a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5079a-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="5079a-128">Response</span></span>

<span data-ttu-id="5079a-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5079a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5079a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5079a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5079a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5079a-132">Request</span></span>
<span data-ttu-id="5079a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5079a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="5079a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5079a-134">Response</span></span>
<span data-ttu-id="5079a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5079a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
