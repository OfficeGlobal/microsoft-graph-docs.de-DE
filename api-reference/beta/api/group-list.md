---
title: Gruppen auflisten
description: Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 393381bfe5f21c4d4196251a4055fc65e0771e5c
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726603"
---
# <a name="list-groups"></a><span data-ttu-id="d0348-103">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="d0348-103">List groups</span></span>

> <span data-ttu-id="d0348-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d0348-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0348-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d0348-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0348-106">Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="d0348-106">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="d0348-107">Dieser Vorgang gibt standardmäßig nur eine Teilmenge der häufiger verwendeten Eigenschaften für jede Gruppe zurück.</span><span class="sxs-lookup"><span data-stu-id="d0348-107">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="d0348-108">Diese _Standard_eigenschaften werden im Abschnitt [Eigenschaften](../resources/group.md#properties) aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="d0348-108">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="d0348-109">Um Eigenschaften abzurufen, die _nicht_ standardmäßig zurückgegeben werden, führen Sie eine [GET](group-get.md)-Operation für die Gruppe aus, und geben Sie die Eigenschaften in einer OData-Abfrageoption `$select` an.</span><span class="sxs-lookup"><span data-stu-id="d0348-109">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="d0348-110">Sehen Sie sich das [Beispiel](group-get.md#request-2) an.</span><span class="sxs-lookup"><span data-stu-id="d0348-110">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="d0348-111">Eine Ausnahme ist die **hasMembersWithLicenseErrors**-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="d0348-111">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="d0348-112">Sehen Sie sich ein [Beispiel](#request-2) für die Verwendung dieser Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="d0348-112">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0348-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d0348-113">Permissions</span></span>
<span data-ttu-id="d0348-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0348-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0348-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d0348-116">Permission type</span></span>      | <span data-ttu-id="d0348-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d0348-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0348-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d0348-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d0348-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0348-119">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0348-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d0348-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0348-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0348-121">Not supported.</span></span>    |
|<span data-ttu-id="d0348-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d0348-122">Application</span></span> | <span data-ttu-id="d0348-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0348-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0348-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0348-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0348-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d0348-125">Optional query parameters</span></span>

<span data-ttu-id="d0348-126">Um nur Office 365-Gruppen (auch als einheitliche Gruppen bezeichnet) aufzulisten, wenden Sie einen Filter auf **groupTypes** an: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="d0348-126">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="d0348-127">Sie können die OData-Abfrageoption `$orderby` verwenden, um Gruppen in einer Organisation nach ihrem jeweiligen Wert für **displayName** zu sortieren. Hier ein Beispiel: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="d0348-127">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="d0348-128">Weitere Informationen zu OData-Abfrageoptionen finden Sie unter [OData-Abfrageparameter](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d0348-128">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0348-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d0348-129">Request headers</span></span>
| <span data-ttu-id="d0348-130">Name</span><span class="sxs-lookup"><span data-stu-id="d0348-130">Name</span></span>       | <span data-ttu-id="d0348-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d0348-131">Type</span></span> | <span data-ttu-id="d0348-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0348-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d0348-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0348-133">Authorization</span></span>  | <span data-ttu-id="d0348-134">string</span><span class="sxs-lookup"><span data-stu-id="d0348-134">string</span></span>  | <span data-ttu-id="d0348-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0348-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0348-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d0348-137">Request body</span></span>
<span data-ttu-id="d0348-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d0348-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0348-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0348-139">Response</span></span>
<span data-ttu-id="d0348-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d0348-140">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="d0348-141">Die Antwort enthält nur die Standardeigenschaften der einzelnen Gruppen.</span><span class="sxs-lookup"><span data-stu-id="d0348-141">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="d0348-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d0348-142">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="d0348-143">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="d0348-143">Request 1</span></span>
<span data-ttu-id="d0348-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d0348-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response-1"></a><span data-ttu-id="d0348-145">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="d0348-145">Response 1</span></span>
<span data-ttu-id="d0348-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d0348-146">The following is an example of the response.</span></span>
><span data-ttu-id="d0348-147">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="d0348-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d0348-148">Alle Standardeigenschaften werden für jede Gruppe in einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d0348-148">All the default properties are returned for each group in an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
    "value": [
         {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-12-22T02:21:05Z",
            "description": "Self help community for golf",
            "displayName": "Golf Assist",
            "expirationDateTime": null,
            "groupTypes": [
                "Unified"
            ],
            "mail": "golfassist@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golfassist",
            "membershipRule": null,
            "membershipRuleProcessingState": null,
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "preferredLanguage": null,
            "proxyAddresses": [
                "smtp:golfassist@contoso.onmicrosoft.com",
                "SMTP:golfassist@contoso.com"
            ],
            "renewedDateTime": "2018-12-22T02:21:05Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "theme": null,
            "visibility": "Public",
            "onPremisesProvisioningErrors": []
        },
        {
            "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-11-19T20:29:40Z",
            "description": "Talk about golf",
            "displayName": "Golf Discussion",
            "expirationDateTime": null,
            "groupTypes": [],
            "mail": "golftalk@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golftalk",
            "membershipRule": null,
            "membershipRuleProcessingState": null,
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "preferredLanguage": null,
            "proxyAddresses": [
                "smtp:golftalk@contoso.onmicrosoft.com",
                "SMTP:golftalk@contoso.com"
            ],
            "renewedDateTime": "2018-11-19T20:29:40Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "theme": null,
            "visibility": null,
            "onPremisesProvisioningErrors": []
        }
    ]
}

```

#### <a name="request-2"></a><span data-ttu-id="d0348-149">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="d0348-149">Request 2</span></span>
<span data-ttu-id="d0348-150">Dieses Beispiel verwendet eine `$filter`-Abfrageoption, um die Gruppen abzurufen, die Mitglieder mit Lizenzfehlern in ihren gruppenbasierten Lizenzzuordnungen aufweisen.</span><span class="sxs-lookup"><span data-stu-id="d0348-150">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="d0348-151">Außerdem wird eine `$select`-Abfrageoption verwendet, um nur die **id**- und die **displayName**-Eigenschaft jeder Gruppe in der Antwort und keine anderen standardmäßigen oder nicht standardmäßigen Eigenschaften abzurufen.</span><span class="sxs-lookup"><span data-stu-id="d0348-151">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="d0348-152">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="d0348-152">Response 2</span></span>
<span data-ttu-id="d0348-153">Nachfolgend finden Sie ein Beispiel der Antwort, die nur die angeforderten Eigenschaften umfasst.</span><span class="sxs-lookup"><span data-stu-id="d0348-153">The following is an example of the response which includes only the requested properties.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
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
