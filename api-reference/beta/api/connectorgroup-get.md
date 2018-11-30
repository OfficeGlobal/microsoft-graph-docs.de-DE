---
title: Abrufen von connectorGroup
description: Rufen Sie die Eigenschaften eines ConnectorGroup-Objekts ab.
ms.openlocfilehash: 8677432bf14559d47811218dc20cd0af6837dd3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061260"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="fed2a-103">Abrufen von connectorGroup</span><span class="sxs-lookup"><span data-stu-id="fed2a-103">Get connectorGroup</span></span>

> <span data-ttu-id="fed2a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fed2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fed2a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fed2a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fed2a-106">Rufen Sie die Eigenschaften eines ConnectorGroup-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="fed2a-106">Retrieve the properties of a connectorGroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fed2a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fed2a-107">Permissions</span></span>
<span data-ttu-id="fed2a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fed2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fed2a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fed2a-110">Permission type</span></span>      | <span data-ttu-id="fed2a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fed2a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fed2a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fed2a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fed2a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fed2a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fed2a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fed2a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fed2a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fed2a-115">Not supported.</span></span>    |
|<span data-ttu-id="fed2a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fed2a-116">Application</span></span> | <span data-ttu-id="fed2a-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fed2a-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fed2a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fed2a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fed2a-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fed2a-119">Optional query parameters</span></span>
<span data-ttu-id="fed2a-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fed2a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fed2a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fed2a-121">Request headers</span></span>
| <span data-ttu-id="fed2a-122">Name</span><span class="sxs-lookup"><span data-stu-id="fed2a-122">Name</span></span>      |<span data-ttu-id="fed2a-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fed2a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fed2a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fed2a-124">Authorization</span></span>  | <span data-ttu-id="fed2a-125">Bearer.</span><span class="sxs-lookup"><span data-stu-id="fed2a-125">Bearer.</span></span> <span data-ttu-id="fed2a-126">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="fed2a-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="fed2a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fed2a-127">Request body</span></span>
<span data-ttu-id="fed2a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fed2a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fed2a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fed2a-129">Response</span></span>

<span data-ttu-id="fed2a-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [ConnectorGroup](../resources/connectorgroup.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fed2a-130">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fed2a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fed2a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fed2a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fed2a-132">Request</span></span>
<span data-ttu-id="fed2a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fed2a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="fed2a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fed2a-134">Response</span></span>
<span data-ttu-id="fed2a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fed2a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
