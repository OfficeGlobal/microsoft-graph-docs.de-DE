---
title: 'ServicePrincipals: OwnedObjects auflisten'
description: Abrufen einer Liste der Objekte im Besitz der ServicePrincipal.  Dies kann Anwendungen oder Gruppen umfassen.
ms.openlocfilehash: 79ca70c5c86e535a7d8a11598509e7ebf61780a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064355"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="3f6e9-104">ServicePrincipals: OwnedObjects auflisten</span><span class="sxs-lookup"><span data-stu-id="3f6e9-104">servicePrincipals: List ownedObjects</span></span>

> <span data-ttu-id="3f6e9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f6e9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3f6e9-107">Abrufen einer Liste der Objekte im Besitz der ServicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-107">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="3f6e9-108">Dies kann Anwendungen oder Gruppen umfassen.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-108">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f6e9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3f6e9-109">Permissions</span></span>
<span data-ttu-id="3f6e9-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f6e9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f6e9-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3f6e9-112">Permission type</span></span>      | <span data-ttu-id="3f6e9-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3f6e9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f6e9-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3f6e9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3f6e9-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f6e9-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f6e9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3f6e9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f6e9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f6e9-117">Not supported.</span></span>    |
|<span data-ttu-id="3f6e9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3f6e9-118">Application</span></span> | <span data-ttu-id="3f6e9-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f6e9-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f6e9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f6e9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f6e9-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3f6e9-121">Optional query parameters</span></span>
<span data-ttu-id="3f6e9-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f6e9-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3f6e9-123">Request headers</span></span>
| <span data-ttu-id="3f6e9-124">Name</span><span class="sxs-lookup"><span data-stu-id="3f6e9-124">Name</span></span>       | <span data-ttu-id="3f6e9-125">Typ</span><span class="sxs-lookup"><span data-stu-id="3f6e9-125">Type</span></span> | <span data-ttu-id="3f6e9-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f6e9-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3f6e9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f6e9-127">Authorization</span></span>  | <span data-ttu-id="3f6e9-128">string</span><span class="sxs-lookup"><span data-stu-id="3f6e9-128">string</span></span>  | <span data-ttu-id="3f6e9-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f6e9-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3f6e9-131">Request body</span></span>
<span data-ttu-id="3f6e9-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f6e9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f6e9-133">Response</span></span>

<span data-ttu-id="3f6e9-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f6e9-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3f6e9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f6e9-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f6e9-136">Request</span></span>
<span data-ttu-id="3f6e9-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="3f6e9-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f6e9-138">Response</span></span>
<span data-ttu-id="3f6e9-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3f6e9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->