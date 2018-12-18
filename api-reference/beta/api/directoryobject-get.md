---
title: directoryObject abrufen
description: Rufen Sie die Eigenschaften und Beziehungen des Directoryobject-Objekts ab.
author: lleonard-msft
ms.openlocfilehash: 52862d10c8361ea8ba365d06dcbaf0ce06b2779f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316373"
---
# <a name="get-directoryobject"></a><span data-ttu-id="07500-103">directoryObject abrufen</span><span class="sxs-lookup"><span data-stu-id="07500-103">Get directoryObject</span></span>

> <span data-ttu-id="07500-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07500-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07500-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07500-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07500-106">Rufen Sie die Eigenschaften und Beziehungen des Directoryobject-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="07500-106">Retrieve the properties and relationships of directoryobject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="07500-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07500-107">Permissions</span></span>
<span data-ttu-id="07500-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07500-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07500-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07500-110">Permission type</span></span>      | <span data-ttu-id="07500-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07500-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07500-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07500-112">Delegated (work or school account)</span></span> | <span data-ttu-id="07500-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07500-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07500-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07500-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07500-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07500-115">Not supported.</span></span>    |
|<span data-ttu-id="07500-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07500-116">Application</span></span> | <span data-ttu-id="07500-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="07500-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07500-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07500-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="07500-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="07500-119">Optional query parameters</span></span>
<span data-ttu-id="07500-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="07500-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="07500-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07500-121">Request headers</span></span>
| <span data-ttu-id="07500-122">Name</span><span class="sxs-lookup"><span data-stu-id="07500-122">Name</span></span>       | <span data-ttu-id="07500-123">Typ</span><span class="sxs-lookup"><span data-stu-id="07500-123">Type</span></span> | <span data-ttu-id="07500-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07500-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="07500-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="07500-125">Authorization</span></span>  | <span data-ttu-id="07500-126">string</span><span class="sxs-lookup"><span data-stu-id="07500-126">string</span></span>  | <span data-ttu-id="07500-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07500-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07500-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07500-129">Request body</span></span>
<span data-ttu-id="07500-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="07500-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07500-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="07500-131">Response</span></span>

<span data-ttu-id="07500-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07500-132">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07500-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07500-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07500-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07500-134">Request</span></span>
<span data-ttu-id="07500-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07500-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/beta/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="07500-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="07500-136">Response</span></span>
<span data-ttu-id="07500-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07500-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
