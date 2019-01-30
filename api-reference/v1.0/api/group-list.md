---
title: Gruppen auflisten
description: Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 8ede194abffe745bee9a23906b965d43de93cec8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643741"
---
# <a name="list-groups"></a><span data-ttu-id="9990d-103">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="9990d-103">List groups</span></span>
<span data-ttu-id="9990d-104">Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="9990d-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="9990d-105">Dieser Vorgang gibt standardmäßig nur eine Untergruppe der Eigenschaften für jede Gruppe zurück.</span><span class="sxs-lookup"><span data-stu-id="9990d-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="9990d-106">Diese Standardeigenschaften werden im Abschnitt [Eigenschaften](../resources/group.md#properties) aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="9990d-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="9990d-107">Um Eigenschaften abzurufen, die _nicht_ standardmäßig zurückgegeben werden, führen Sie eine [GET](group-get.md)-Operation für die Gruppe aus, und geben Sie die Eigenschaften in einer OData-Abfrageoption `$select` an.</span><span class="sxs-lookup"><span data-stu-id="9990d-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="9990d-108">Sehen Sie sich das [Beispiel](group-get.md#request-2) an.</span><span class="sxs-lookup"><span data-stu-id="9990d-108">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="9990d-109">Eine Ausnahme ist die **hasMembersWithLicenseErrors**-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="9990d-109">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="9990d-110">Sehen Sie sich ein [Beispiel](#request-2) für die Verwendung dieser Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="9990d-110">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="9990d-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9990d-111">Permissions</span></span>
<span data-ttu-id="9990d-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9990d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9990d-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9990d-114">Permission type</span></span>      | <span data-ttu-id="9990d-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9990d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9990d-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9990d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9990d-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9990d-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9990d-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9990d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9990d-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9990d-119">Not supported.</span></span>    |
|<span data-ttu-id="9990d-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9990d-120">Application</span></span> | <span data-ttu-id="9990d-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9990d-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9990d-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9990d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9990d-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9990d-123">Optional query parameters</span></span>
<span data-ttu-id="9990d-124">Um nur Office 365-Gruppen (auch als einheitliche Gruppen bezeichnet) aufzulisten, wenden Sie einen Filter auf **groupTypes** an: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9990d-124">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**: <!-- { "blockType": "ignored" } --></span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="9990d-125">Sie können die OData-Abfrageoption `$orderby` verwenden, um Gruppen in einer Organisation nach ihrem jeweiligen Wert für **displayName** zu sortieren. Hier ein Beispiel: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9990d-125">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example: <!-- { "blockType": "ignored" } --></span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="9990d-126">Weitere Informationen zu OData-Abfrageoptionen finden Sie unter [OData-Abfrageparameter](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9990d-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9990d-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9990d-127">Request headers</span></span>
| <span data-ttu-id="9990d-128">Name</span><span class="sxs-lookup"><span data-stu-id="9990d-128">Name</span></span>       | <span data-ttu-id="9990d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9990d-129">Type</span></span> | <span data-ttu-id="9990d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9990d-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9990d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="9990d-131">Authorization</span></span>  | <span data-ttu-id="9990d-132">string</span><span class="sxs-lookup"><span data-stu-id="9990d-132">string</span></span>  | <span data-ttu-id="9990d-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9990d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9990d-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9990d-135">Request body</span></span>
<span data-ttu-id="9990d-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9990d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9990d-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="9990d-137">Response</span></span>
<span data-ttu-id="9990d-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9990d-138">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="9990d-139">Die Antwort enthält nur die Standardeigenschaften der einzelnen Gruppen.</span><span class="sxs-lookup"><span data-stu-id="9990d-139">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="9990d-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9990d-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="9990d-141">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="9990d-141">Request 1</span></span>
<span data-ttu-id="9990d-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9990d-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response-1"></a><span data-ttu-id="9990d-143">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="9990d-143">Response 1</span></span>
<span data-ttu-id="9990d-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9990d-144">The following is an example of the response.</span></span>

><span data-ttu-id="9990d-145">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="9990d-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9990d-146">Alle Standardeigenschaften werden für jede Gruppe in einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9990d-146">All the default properties are returned for each group in an actual call.</span></span>

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
#### <a name="request-2"></a><span data-ttu-id="9990d-147">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="9990d-147">Request 2</span></span>
<span data-ttu-id="9990d-148">Dieses Beispiel verwendet eine `$filter`-Abfrageoption, um die Gruppen abzurufen, die Mitglieder mit Lizenzfehlern in ihren gruppenbasierten Lizenzzuordnungen aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9990d-148">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="9990d-149">Außerdem wird eine `$select`-Abfrageoption verwendet, um nur die **id**- und die **displayName**-Eigenschaft jeder Gruppe in der Antwort und keine anderen standardmäßigen oder nicht standardmäßigen Eigenschaften abzurufen.</span><span class="sxs-lookup"><span data-stu-id="9990d-149">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="9990d-150">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="9990d-150">Response 2</span></span>
<span data-ttu-id="9990d-151">Nachfolgend finden Sie ein Beispiel der Antwort, die nur die angeforderten Eigenschaften umfasst.</span><span class="sxs-lookup"><span data-stu-id="9990d-151">The following is an example of the response which includes only the requested properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups_withlicenseerrors"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName)",
    "value": [
        {
            "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
            "displayName": "Library Assist"
        },
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "displayName": "Golf Assist"
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
