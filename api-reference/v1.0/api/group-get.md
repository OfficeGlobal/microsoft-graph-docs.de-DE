---
title: Gruppe abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines Gruppenobjekts.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 92b9c8de30f0070491d84acf9cfc56225c1a7981
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353090"
---
# <a name="get-group"></a><span data-ttu-id="14ae4-103">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="14ae4-103">Get group</span></span>
<span data-ttu-id="14ae4-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines Gruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="14ae4-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="14ae4-105">Dieser Vorgang gibt standardmäßig nur eine Teilmenge aller verfügbaren Eigenschaften zurück, wie im Abschnitt [Eigenschaften](../resources/group.md#properties) beschrieben.</span><span class="sxs-lookup"><span data-stu-id="14ae4-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="14ae4-106">Zum Abrufen von Eigenschaften, die _nicht_ standardmäßig zurückgegeben werden, geben sie diese in einer OData-Abfrageoption `$select` an.</span><span class="sxs-lookup"><span data-stu-id="14ae4-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="14ae4-107">Sehen Sie sich das [Beispiel](#request-2) an.</span><span class="sxs-lookup"><span data-stu-id="14ae4-107">See an [example](#request-2).</span></span>

## <a name="permissions"></a><span data-ttu-id="14ae4-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="14ae4-108">Permissions</span></span>
<span data-ttu-id="14ae4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14ae4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14ae4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="14ae4-111">Permission type</span></span>      | <span data-ttu-id="14ae4-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="14ae4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14ae4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="14ae4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="14ae4-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ae4-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14ae4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="14ae4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14ae4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14ae4-116">Not supported.</span></span>    |
|<span data-ttu-id="14ae4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="14ae4-117">Application</span></span> | <span data-ttu-id="14ae4-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ae4-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14ae4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="14ae4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14ae4-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="14ae4-120">Optional query parameters</span></span>
<span data-ttu-id="14ae4-121">Mit `$select` können Sie bestimmte Gruppeneigenschaften abrufen, einschließlich derjenigen, die standardmäßig nicht zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="14ae4-121">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="14ae4-122">Unten finden Sie ein [Beispiel](#request-2).</span><span class="sxs-lookup"><span data-stu-id="14ae4-122">See an [example](#request-2).</span></span>

<span data-ttu-id="14ae4-123">Weitere Informationen zu OData-Abfrageoptionen finden Sie unter [OData-Abfrageparameter](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="14ae4-123">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="14ae4-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="14ae4-124">Request headers</span></span>
| <span data-ttu-id="14ae4-125">Name</span><span class="sxs-lookup"><span data-stu-id="14ae4-125">Name</span></span>       | <span data-ttu-id="14ae4-126">Typ</span><span class="sxs-lookup"><span data-stu-id="14ae4-126">Type</span></span> | <span data-ttu-id="14ae4-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14ae4-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14ae4-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="14ae4-128">Authorization</span></span>  | <span data-ttu-id="14ae4-129">string</span><span class="sxs-lookup"><span data-stu-id="14ae4-129">string</span></span>  | <span data-ttu-id="14ae4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="14ae4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14ae4-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="14ae4-132">Request body</span></span>
<span data-ttu-id="14ae4-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="14ae4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14ae4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="14ae4-134">Response</span></span>
<span data-ttu-id="14ae4-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14ae4-135">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="14ae4-136">Es werden die Standardeigenschaften zurückgegeben, sofern Sie nicht mit `$select` bestimmte Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="14ae4-136">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="14ae4-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="14ae4-137">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="14ae4-138">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="14ae4-138">Request 1</span></span>
<span data-ttu-id="14ae4-139">Nachfolgend sehen Sie ein Beispiel für eine GET-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="14ae4-139">The following is an example of the GET request with sample query string values.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response-1"></a><span data-ttu-id="14ae4-140">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="14ae4-140">Response 1</span></span>
<span data-ttu-id="14ae4-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="14ae4-141">The following is an example of the response.</span></span> <span data-ttu-id="14ae4-142">Es enthält nur die Standardeigenschaften.</span><span class="sxs-lookup"><span data-stu-id="14ae4-142">It includes only the default properties.</span></span>

><span data-ttu-id="14ae4-143">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="14ae4-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="14ae4-144">Bei einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14ae4-144">All the default properties are returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-22T00:51:37Z",
    "creationOptions": [],
    "description": "Self help community for library",
    "displayName": "Library Assist",
    "groupTypes": [
        "Unified"
    ],
    "mail": "library2@contoso.com",
    "mailEnabled": true,
    "mailNickname": "library",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "smtp:library7423@contoso.com",
        "SMTP:library2@contoso.com"
    ],
    "renewedDateTime": "2018-12-22T00:51:37Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a><span data-ttu-id="14ae4-145">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="14ae4-145">Request 2</span></span>
<span data-ttu-id="14ae4-146">Das nächste Beispiel verwendet eine `$select`-Abfrageoption, um einige Eigenschaften abzurufen, die standardmäßig nicht zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="14ae4-146">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="14ae4-147">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="14ae4-147">Response 2</span></span>
<span data-ttu-id="14ae4-148">Nachfolgend finden Sie ein Beispiel der Antwort, die die angeforderten nicht standardmäßigen Eigenschaften umfasst.</span><span class="sxs-lookup"><span data-stu-id="14ae4-148">The following is an example of the response which includes the requested non-default properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group_non_default"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
