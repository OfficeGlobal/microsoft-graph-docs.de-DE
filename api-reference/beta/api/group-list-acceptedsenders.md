---
title: acceptedSenders auflisten
description: Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der acceptedSenders für diese Gruppe befinden.
ms.openlocfilehash: a4a4970abe0a6a866ed26fa04ebe3f7a0cee1f8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065414"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="8e87c-103">acceptedSenders auflisten</span><span class="sxs-lookup"><span data-stu-id="8e87c-103">List acceptedSenders</span></span>

> <span data-ttu-id="8e87c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8e87c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e87c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e87c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e87c-106">Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der acceptedSenders für diese Gruppe befinden.</span><span class="sxs-lookup"><span data-stu-id="8e87c-106">Get a list of users or groups that are in the acceptedSenders list for this group.</span></span>

<span data-ttu-id="8e87c-p102">Benutzer in der Liste der zulässigenAbsender können Beiträge in Unterhaltungen der Gruppe (im GET-Anforderungs-URL identifiziert) bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für zulässige und abgelehnte Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8e87c-p102">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e87c-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8e87c-109">Permissions</span></span>
<span data-ttu-id="8e87c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e87c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e87c-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e87c-112">Permission type</span></span>      | <span data-ttu-id="8e87c-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e87c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e87c-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e87c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8e87c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e87c-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e87c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e87c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e87c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e87c-117">Not supported.</span></span>    |
|<span data-ttu-id="8e87c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e87c-118">Application</span></span> | <span data-ttu-id="8e87c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e87c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e87c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e87c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e87c-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8e87c-121">Optional query parameters</span></span>
<span data-ttu-id="8e87c-122">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8e87c-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e87c-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e87c-123">Request headers</span></span>
| <span data-ttu-id="8e87c-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8e87c-124">Header</span></span>       | <span data-ttu-id="8e87c-125">Wert</span><span class="sxs-lookup"><span data-stu-id="8e87c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e87c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e87c-126">Authorization</span></span>  | <span data-ttu-id="8e87c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8e87c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e87c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e87c-129">Request body</span></span>
<span data-ttu-id="8e87c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8e87c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e87c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e87c-131">Response</span></span>
<span data-ttu-id="8e87c-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e87c-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e87c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e87c-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8e87c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e87c-134">Request</span></span>
<span data-ttu-id="8e87c-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e87c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```

#### <a name="response"></a><span data-ttu-id="8e87c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e87c-136">Response</span></span>
<span data-ttu-id="8e87c-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8e87c-137">The following is an example of the response.</span></span>
><span data-ttu-id="8e87c-138">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="8e87c-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e87c-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8e87c-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->