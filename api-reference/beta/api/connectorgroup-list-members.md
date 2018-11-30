---
title: Mitglieder auflisten
description: Abrufen einer Liste der Connectorobjekten, die eine ConnectorGroup zugeordnet.
ms.openlocfilehash: 504cba20c0d93db9f0c0333dcf7578e051b3009f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062679"
---
# <a name="list-members"></a><span data-ttu-id="49fcd-103">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="49fcd-103">List members</span></span>

> <span data-ttu-id="49fcd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="49fcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49fcd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49fcd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49fcd-106">Abrufen einer Liste der Connectorobjekten, die eine ConnectorGroup zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="49fcd-106">Retrieve a list of connector objects associated with a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="49fcd-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="49fcd-107">Permissions</span></span>
<span data-ttu-id="49fcd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49fcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49fcd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49fcd-110">Permission type</span></span>      | <span data-ttu-id="49fcd-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49fcd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49fcd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49fcd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49fcd-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49fcd-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49fcd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49fcd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49fcd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49fcd-115">Not supported.</span></span>    |
|<span data-ttu-id="49fcd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49fcd-116">Application</span></span> | <span data-ttu-id="49fcd-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49fcd-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49fcd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49fcd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49fcd-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="49fcd-119">Optional query parameters</span></span>
<span data-ttu-id="49fcd-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="49fcd-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49fcd-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49fcd-121">Request headers</span></span>
| <span data-ttu-id="49fcd-122">Name</span><span class="sxs-lookup"><span data-stu-id="49fcd-122">Name</span></span>      |<span data-ttu-id="49fcd-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49fcd-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49fcd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="49fcd-124">Authorization</span></span>  | <span data-ttu-id="49fcd-125">Bearer.</span><span class="sxs-lookup"><span data-stu-id="49fcd-125">Bearer.</span></span> <span data-ttu-id="49fcd-126">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="49fcd-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="49fcd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49fcd-127">Request body</span></span>
<span data-ttu-id="49fcd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="49fcd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49fcd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="49fcd-129">Response</span></span>

<span data-ttu-id="49fcd-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="49fcd-130">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49fcd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49fcd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49fcd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49fcd-132">Request</span></span>
<span data-ttu-id="49fcd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49fcd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="49fcd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="49fcd-134">Response</span></span>
<span data-ttu-id="49fcd-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49fcd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
