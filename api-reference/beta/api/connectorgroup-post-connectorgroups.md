---
title: Erstellen von connectorGroup
description: Verwenden Sie diese API, um eine neue ConnectorGroup erstellen.
localization_priority: Normal
ms.openlocfilehash: 65fe6dd901de6238c450b4896b37d56fa8ea602f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824297"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="dde19-103">Erstellen von connectorGroup</span><span class="sxs-lookup"><span data-stu-id="dde19-103">Create connectorGroup</span></span>

> <span data-ttu-id="dde19-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dde19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dde19-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dde19-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dde19-106">Verwenden Sie diese API, um eine neue ConnectorGroup erstellen.</span><span class="sxs-lookup"><span data-stu-id="dde19-106">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="dde19-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dde19-107">Permissions</span></span>
<span data-ttu-id="dde19-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dde19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dde19-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dde19-110">Permission type</span></span>      | <span data-ttu-id="dde19-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dde19-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dde19-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dde19-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dde19-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dde19-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dde19-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dde19-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dde19-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dde19-115">Not supported.</span></span>    |
|<span data-ttu-id="dde19-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dde19-116">Application</span></span> | <span data-ttu-id="dde19-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dde19-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dde19-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dde19-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="dde19-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dde19-119">Request headers</span></span>
| <span data-ttu-id="dde19-120">Name</span><span class="sxs-lookup"><span data-stu-id="dde19-120">Name</span></span>       | <span data-ttu-id="dde19-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dde19-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dde19-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dde19-122">Authorization</span></span>  | <span data-ttu-id="dde19-123">Bearer.</span><span class="sxs-lookup"><span data-stu-id="dde19-123">Bearer.</span></span> <span data-ttu-id="dde19-124">Benötigte</span><span class="sxs-lookup"><span data-stu-id="dde19-124">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="dde19-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dde19-125">Request body</span></span>
<span data-ttu-id="dde19-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ConnectorGroup](../resources/connectorgroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dde19-126">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dde19-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="dde19-127">Response</span></span>

<span data-ttu-id="dde19-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [ConnectorGroup](../resources/connectorgroup.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dde19-128">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dde19-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dde19-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dde19-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dde19-130">Request</span></span>
<span data-ttu-id="dde19-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dde19-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```
<span data-ttu-id="dde19-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ConnectorGroup](../resources/connectorgroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dde19-132">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dde19-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="dde19-133">Response</span></span>
<span data-ttu-id="dde19-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dde19-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
