---
title: rejectedSenders auflisten
description: 'Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der rejectedSenders für diese Gruppe befinden. '
author: dkershaw10
ms.openlocfilehash: aa79ec70982e75349c41ecb551cbf0150b82ad60
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336078"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="be8c7-103">rejectedSenders auflisten</span><span class="sxs-lookup"><span data-stu-id="be8c7-103">List rejectedSenders</span></span>

> <span data-ttu-id="be8c7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="be8c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be8c7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be8c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be8c7-106">Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der rejectedSenders für diese Gruppe befinden.</span><span class="sxs-lookup"><span data-stu-id="be8c7-106">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="be8c7-p102">Benutzer in der Liste der abgelehnten Absender können keine Beiträge in Unterhaltungen der Gruppe (im GET-Anforderungs-URL identifiziert) bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für abgelehnte und zulässige Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="be8c7-p102">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="be8c7-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be8c7-109">Permissions</span></span>
<span data-ttu-id="be8c7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be8c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be8c7-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be8c7-112">Permission type</span></span>      | <span data-ttu-id="be8c7-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be8c7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be8c7-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be8c7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="be8c7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be8c7-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="be8c7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be8c7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be8c7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be8c7-117">Not supported.</span></span>    |
|<span data-ttu-id="be8c7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be8c7-118">Application</span></span> | <span data-ttu-id="be8c7-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be8c7-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be8c7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be8c7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be8c7-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="be8c7-121">Optional query parameters</span></span>
<span data-ttu-id="be8c7-122">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be8c7-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be8c7-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be8c7-123">Request headers</span></span>
| <span data-ttu-id="be8c7-124">Header</span><span class="sxs-lookup"><span data-stu-id="be8c7-124">Header</span></span>       | <span data-ttu-id="be8c7-125">Wert</span><span class="sxs-lookup"><span data-stu-id="be8c7-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="be8c7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="be8c7-126">Authorization</span></span>  | <span data-ttu-id="be8c7-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="be8c7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be8c7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be8c7-129">Request body</span></span>
<span data-ttu-id="be8c7-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="be8c7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be8c7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="be8c7-131">Response</span></span>
<span data-ttu-id="be8c7-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be8c7-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be8c7-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be8c7-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="be8c7-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be8c7-134">Request</span></span>
<span data-ttu-id="be8c7-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be8c7-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="be8c7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="be8c7-136">Response</span></span>
<span data-ttu-id="be8c7-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be8c7-137">The following is an example of the response.</span></span>
><span data-ttu-id="be8c7-138">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="be8c7-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be8c7-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="be8c7-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->