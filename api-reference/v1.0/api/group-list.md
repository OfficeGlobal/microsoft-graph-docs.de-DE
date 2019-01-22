---
title: Gruppen auflisten
description: Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5081c5013c1bf7c1a1bfbcff58afe5a83aa67bc9
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726575"
---
# <a name="list-groups"></a><span data-ttu-id="f36ee-103">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="f36ee-103">List groups</span></span>
<span data-ttu-id="f36ee-104">Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="f36ee-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="f36ee-105">Dieser Vorgang gibt standardmäßig nur eine Untergruppe der Eigenschaften für jede Gruppe zurück.</span><span class="sxs-lookup"><span data-stu-id="f36ee-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="f36ee-106">Diese Standardeigenschaften werden im Abschnitt [Eigenschaften](../resources/group.md#properties) aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="f36ee-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="f36ee-107">Um Eigenschaften abzurufen, die _nicht_ standardmäßig zurückgegeben werden, führen Sie eine [GET](group-get.md)-Operation für die Gruppe aus, und geben Sie die Eigenschaften in einer OData-Abfrageoption `$select` an.</span><span class="sxs-lookup"><span data-stu-id="f36ee-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="f36ee-108">Sehen Sie sich das [Beispiel](group-get.md#request-2) an.</span><span class="sxs-lookup"><span data-stu-id="f36ee-108">See an [example](group-get.md#request-2).</span></span>

## <a name="permissions"></a><span data-ttu-id="f36ee-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f36ee-109">Permissions</span></span>
<span data-ttu-id="f36ee-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f36ee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f36ee-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f36ee-112">Permission type</span></span>      | <span data-ttu-id="f36ee-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f36ee-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f36ee-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f36ee-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f36ee-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f36ee-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f36ee-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f36ee-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f36ee-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f36ee-117">Not supported.</span></span>    |
|<span data-ttu-id="f36ee-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f36ee-118">Application</span></span> | <span data-ttu-id="f36ee-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f36ee-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f36ee-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f36ee-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f36ee-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f36ee-121">Optional query parameters</span></span>
<span data-ttu-id="f36ee-122">Um nur Office 365-Gruppen (auch als einheitliche Gruppen bezeichnet) aufzulisten, wenden Sie einen Filter auf **groupTypes** an: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="f36ee-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="f36ee-123">Sie können die OData-Abfrageoption `$orderby` verwenden, um Gruppen in einer Organisation nach ihrem jeweiligen Wert für **displayName** zu sortieren. Hier ein Beispiel: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="f36ee-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="f36ee-124">Weitere Informationen zu OData-Abfrageoptionen finden Sie unter [OData-Abfrageparameter](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f36ee-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f36ee-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f36ee-125">Request headers</span></span>
| <span data-ttu-id="f36ee-126">Name</span><span class="sxs-lookup"><span data-stu-id="f36ee-126">Name</span></span>       | <span data-ttu-id="f36ee-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f36ee-127">Type</span></span> | <span data-ttu-id="f36ee-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f36ee-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f36ee-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f36ee-129">Authorization</span></span>  | <span data-ttu-id="f36ee-130">string</span><span class="sxs-lookup"><span data-stu-id="f36ee-130">string</span></span>  | <span data-ttu-id="f36ee-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f36ee-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f36ee-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f36ee-133">Request body</span></span>
<span data-ttu-id="f36ee-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f36ee-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f36ee-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f36ee-135">Response</span></span>
<span data-ttu-id="f36ee-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f36ee-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="f36ee-137">Die Antwort enthält nur die Standardeigenschaften der einzelnen Gruppen.</span><span class="sxs-lookup"><span data-stu-id="f36ee-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="f36ee-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f36ee-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f36ee-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f36ee-139">Request</span></span>
<span data-ttu-id="f36ee-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f36ee-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="f36ee-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f36ee-141">Response</span></span>
<span data-ttu-id="f36ee-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f36ee-142">The following is an example of the response.</span></span>

><span data-ttu-id="f36ee-143">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="f36ee-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f36ee-144">Alle Standardeigenschaften werden für jede Gruppe einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f36ee-144">All the default properties are returned for each group in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-12-22T02:21:05Z",
            "creationOptions": [],
            "description": "Self help community for golf",
            "displayName": "Golf Assist",
            "groupTypes": [
                "Unified"
            ],
            "mail": "golfassist@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golfassist",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golfassist@contoso.onmicrosoft.com",
                "SMTP:golfassist@contoso.com"
            ],
            "renewedDateTime": "2018-12-22T02:21:05Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": "Public",
            "onPremisesProvisioningErrors": []
        },
        {
            "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-11-19T20:29:40Z",
            "creationOptions": [],
            "description": "Talk about golf",
            "displayName": "Golf Discussion",
            "groupTypes": [],
            "mail": "golftalk@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golftalk",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golftalk@contoso.onmicrosoft.com",
                "SMTP:golftalk@contoso.com"
            ],
            "renewedDateTime": "2018-11-19T20:29:40Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": null,
            "onPremisesProvisioningErrors": []
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
