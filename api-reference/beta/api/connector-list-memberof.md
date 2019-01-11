---
title: memberOf auflisten
description: Abrufen der Connectorgroup, für der Connector ein Mitglied ist.
localization_priority: Normal
ms.openlocfilehash: 4eb56931aa134375370167f989d6348760010647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864721"
---
# <a name="list-memberof"></a><span data-ttu-id="edf25-103">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="edf25-103">List memberOf</span></span>

> <span data-ttu-id="edf25-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="edf25-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edf25-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="edf25-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="edf25-106">Abrufen der Connectorgroup, für der Connector ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="edf25-106">Retrieve the connectorgroup the connector is a member of.</span></span>
## <a name="permissions"></a><span data-ttu-id="edf25-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="edf25-107">Permissions</span></span>
<span data-ttu-id="edf25-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edf25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edf25-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="edf25-110">Permission type</span></span>      | <span data-ttu-id="edf25-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="edf25-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edf25-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="edf25-112">Delegated (work or school account)</span></span> | <span data-ttu-id="edf25-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edf25-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="edf25-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="edf25-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edf25-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="edf25-115">Not supported.</span></span>    |
|<span data-ttu-id="edf25-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="edf25-116">Application</span></span> | <span data-ttu-id="edf25-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edf25-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="edf25-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="edf25-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="edf25-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="edf25-119">Optional query parameters</span></span>
<span data-ttu-id="edf25-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="edf25-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="edf25-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="edf25-121">Request headers</span></span>
| <span data-ttu-id="edf25-122">Name</span><span class="sxs-lookup"><span data-stu-id="edf25-122">Name</span></span>      |<span data-ttu-id="edf25-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edf25-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="edf25-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="edf25-124">Authorization</span></span>  | <span data-ttu-id="edf25-125">Bearer.</span><span class="sxs-lookup"><span data-stu-id="edf25-125">Bearer.</span></span> <span data-ttu-id="edf25-126">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="edf25-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="edf25-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="edf25-127">Request body</span></span>
<span data-ttu-id="edf25-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="edf25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edf25-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="edf25-129">Response</span></span>

<span data-ttu-id="edf25-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [ConnectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="edf25-130">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="edf25-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="edf25-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="edf25-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="edf25-132">Request</span></span>
<span data-ttu-id="edf25-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="edf25-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="edf25-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="edf25-134">Response</span></span>
<span data-ttu-id="edf25-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="edf25-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
