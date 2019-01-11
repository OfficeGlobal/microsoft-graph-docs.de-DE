---
title: Gruppen auflisten
description: Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.
localization_priority: Priority
ms.openlocfilehash: 1122685cfbd4f1a1f2ff0ca3367e913c983866a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867718"
---
# <a name="list-groups"></a><span data-ttu-id="69482-103">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="69482-103">List groups</span></span>
<span data-ttu-id="69482-p101">Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen. Die [Standardeigenschaften](../api/group-get.md#default-properties) jeder einzelnen Gruppe werden zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69482-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="69482-106">Um nur Office 365-Gruppen (auch als einheitliche Gruppen bezeichnet) aufzulisten, wenden Sie einen Filter auf **groupTypes** an:</span><span class="sxs-lookup"><span data-stu-id="69482-106">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="69482-107">Sie können die OData-Abfrageoption `$orderby` verwenden, um Gruppen in einer Organisation nach ihrem jeweiligen Wert für **displayName** zu sortieren. Hier ein Beispiel:</span><span class="sxs-lookup"><span data-stu-id="69482-107">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

## <a name="permissions"></a><span data-ttu-id="69482-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="69482-108">Permissions</span></span>
<span data-ttu-id="69482-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69482-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69482-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69482-111">Permission type</span></span>      | <span data-ttu-id="69482-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69482-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69482-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69482-113">Delegated (work or school account)</span></span> | <span data-ttu-id="69482-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69482-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="69482-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69482-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69482-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69482-116">Not supported.</span></span>    |
|<span data-ttu-id="69482-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69482-117">Application</span></span> | <span data-ttu-id="69482-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69482-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69482-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69482-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69482-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="69482-120">Optional query parameters</span></span>
<span data-ttu-id="69482-121">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="69482-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69482-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69482-122">Request headers</span></span>
| <span data-ttu-id="69482-123">Name</span><span class="sxs-lookup"><span data-stu-id="69482-123">Name</span></span>       | <span data-ttu-id="69482-124">Typ</span><span class="sxs-lookup"><span data-stu-id="69482-124">Type</span></span> | <span data-ttu-id="69482-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69482-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="69482-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="69482-126">Authorization</span></span>  | <span data-ttu-id="69482-127">string</span><span class="sxs-lookup"><span data-stu-id="69482-127">string</span></span>  | <span data-ttu-id="69482-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="69482-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69482-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69482-130">Request body</span></span>
<span data-ttu-id="69482-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="69482-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69482-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="69482-132">Response</span></span>
<span data-ttu-id="69482-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69482-133">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69482-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69482-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="69482-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69482-135">Request</span></span>
<span data-ttu-id="69482-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69482-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="69482-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="69482-137">Response</span></span>
<span data-ttu-id="69482-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="69482-138">The following is an example of the response.</span></span>

><span data-ttu-id="69482-139">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="69482-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="69482-140">Von einem tatsächlichen Aufruf werden die [Standardeigenschaften](../api/group-get.md#default-properties) zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69482-140">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

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
