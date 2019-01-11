---
title: rejectedSenders auflisten
description: 'Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der rejectedSenders für diese Gruppe befinden. '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 58d8b15c6d20c3fbec895cc3a8050238bbe9507b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867662"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="bd56b-103">rejectedSenders auflisten</span><span class="sxs-lookup"><span data-stu-id="bd56b-103">List rejectedSenders</span></span>
<span data-ttu-id="bd56b-104">Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der rejectedSenders für diese Gruppe befinden.</span><span class="sxs-lookup"><span data-stu-id="bd56b-104">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="bd56b-p101">Benutzer in der Liste der abgelehnten Absender können keine Beiträge in Unterhaltungen der Gruppe (im GET-Anforderungs-URL identifiziert) bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für abgelehnte und zulässige Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="bd56b-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd56b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bd56b-107">Permissions</span></span>
<span data-ttu-id="bd56b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd56b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd56b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd56b-110">Permission type</span></span>      | <span data-ttu-id="bd56b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd56b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd56b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd56b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bd56b-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd56b-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd56b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd56b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd56b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd56b-115">Not supported.</span></span>    |
|<span data-ttu-id="bd56b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd56b-116">Application</span></span> | <span data-ttu-id="bd56b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd56b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd56b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd56b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd56b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bd56b-119">Optional query parameters</span></span>
<span data-ttu-id="bd56b-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bd56b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd56b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd56b-121">Request headers</span></span>
| <span data-ttu-id="bd56b-122">Header</span><span class="sxs-lookup"><span data-stu-id="bd56b-122">Header</span></span>       | <span data-ttu-id="bd56b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="bd56b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd56b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd56b-124">Authorization</span></span>  | <span data-ttu-id="bd56b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bd56b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd56b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd56b-127">Request body</span></span>
<span data-ttu-id="bd56b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bd56b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd56b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd56b-129">Response</span></span>
<span data-ttu-id="bd56b-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd56b-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd56b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd56b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bd56b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd56b-132">Request</span></span>
<span data-ttu-id="bd56b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd56b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="bd56b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd56b-134">Response</span></span>
<span data-ttu-id="bd56b-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bd56b-135">The following is an example of the response.</span></span>
><span data-ttu-id="bd56b-136">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="bd56b-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bd56b-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="bd56b-137">All the properties will be returned from an actual call.</span></span>
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
