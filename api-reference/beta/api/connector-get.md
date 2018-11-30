---
title: Get-connector
description: Rufen Sie die Eigenschaften eines Connector-Objekts ab.
ms.openlocfilehash: f299648093350d4d91637268aa76908f69ca7a38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061264"
---
# <a name="get-connector"></a><span data-ttu-id="1e30b-103">Get-connector</span><span class="sxs-lookup"><span data-stu-id="1e30b-103">Get connector</span></span>

> <span data-ttu-id="1e30b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1e30b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e30b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e30b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e30b-106">Rufen Sie die Eigenschaften eines Connector-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="1e30b-106">Retrieve the properties of a connector object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e30b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1e30b-107">Permissions</span></span>
<span data-ttu-id="1e30b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e30b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e30b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e30b-110">Permission type</span></span>      | <span data-ttu-id="1e30b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e30b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e30b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e30b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e30b-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e30b-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e30b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e30b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e30b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e30b-115">Not supported.</span></span>    |
|<span data-ttu-id="1e30b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e30b-116">Application</span></span> | <span data-ttu-id="1e30b-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e30b-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e30b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e30b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e30b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1e30b-119">Optional query parameters</span></span>
<span data-ttu-id="1e30b-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1e30b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e30b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e30b-121">Request headers</span></span>
| <span data-ttu-id="1e30b-122">Name</span><span class="sxs-lookup"><span data-stu-id="1e30b-122">Name</span></span>      |<span data-ttu-id="1e30b-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e30b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e30b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e30b-124">Authorization</span></span>  | <span data-ttu-id="1e30b-125">Bearer.</span><span class="sxs-lookup"><span data-stu-id="1e30b-125">Bearer.</span></span> <span data-ttu-id="1e30b-126">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="1e30b-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e30b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e30b-127">Request body</span></span>
<span data-ttu-id="1e30b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1e30b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e30b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e30b-129">Response</span></span>

<span data-ttu-id="1e30b-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [Connector](../resources/connector.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1e30b-130">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e30b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e30b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e30b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e30b-132">Request</span></span>
<span data-ttu-id="1e30b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e30b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="1e30b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e30b-134">Response</span></span>
<span data-ttu-id="1e30b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e30b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
