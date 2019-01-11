---
title: Gruppen auflisten
description: Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.
localization_priority: Priority
ms.openlocfilehash: dd243d1f07b98564bb5aa4751664337c0f0654cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813272"
---
# <a name="list-groups"></a><span data-ttu-id="1f368-103">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="1f368-103">List groups</span></span>

> <span data-ttu-id="1f368-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1f368-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f368-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f368-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f368-p102">Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen. Die [Standardeigenschaften](../api/group-get.md#default-properties) jeder einzelnen Gruppe werden zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f368-p102">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="1f368-108">Um nur Office 365-Gruppen (auch als einheitliche Gruppen bezeichnet) aufzulisten, wenden Sie einen Filter auf **groupTypes** an:</span><span class="sxs-lookup"><span data-stu-id="1f368-108">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="1f368-109">Sie können die OData-Abfrageoption `$orderby` verwenden, um Gruppen in einer Organisation nach ihrem jeweiligen Wert für **displayName** zu sortieren. Hier ein Beispiel:</span><span class="sxs-lookup"><span data-stu-id="1f368-109">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="1f368-110">Verwenden Sie zum Zurückgeben von Gruppen, die Elemente mit Fehlern Lizenz enthält die **$filter** Abfragezeichenfolgen-Parameter:</span><span class="sxs-lookup"><span data-stu-id="1f368-110">To return groups containing members with license errors, use the **$filter** query parameter:</span></span> 

```http 
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true 
```
## <a name="permissions"></a><span data-ttu-id="1f368-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f368-111">Permissions</span></span>
<span data-ttu-id="1f368-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f368-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f368-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f368-114">Permission type</span></span>      | <span data-ttu-id="1f368-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f368-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f368-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f368-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1f368-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f368-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f368-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f368-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f368-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f368-119">Not supported.</span></span>    |
|<span data-ttu-id="1f368-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f368-120">Application</span></span> | <span data-ttu-id="1f368-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f368-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f368-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f368-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f368-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1f368-123">Optional query parameters</span></span>
<span data-ttu-id="1f368-124">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f368-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f368-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f368-125">Request headers</span></span>
| <span data-ttu-id="1f368-126">Name</span><span class="sxs-lookup"><span data-stu-id="1f368-126">Name</span></span>       | <span data-ttu-id="1f368-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1f368-127">Type</span></span> | <span data-ttu-id="1f368-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f368-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f368-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f368-129">Authorization</span></span>  | <span data-ttu-id="1f368-130">string</span><span class="sxs-lookup"><span data-stu-id="1f368-130">string</span></span>  | <span data-ttu-id="1f368-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f368-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f368-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f368-133">Request body</span></span>
<span data-ttu-id="1f368-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1f368-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f368-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f368-135">Response</span></span>
<span data-ttu-id="1f368-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f368-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f368-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f368-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1f368-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f368-138">Request</span></span>
<span data-ttu-id="1f368-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f368-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response"></a><span data-ttu-id="1f368-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f368-140">Response</span></span>
<span data-ttu-id="1f368-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f368-141">The following is an example of the response.</span></span>
><span data-ttu-id="1f368-142">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="1f368-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1f368-143">Von einem tatsächlichen Aufruf werden die [Standardeigenschaften](../api/group-get.md#default-properties) zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f368-143">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
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
