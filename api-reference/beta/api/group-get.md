---
title: Gruppe abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines Gruppenobjekts.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 8455985891701e0d1a9fd1062eebc648375c0a2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526284"
---
# <a name="get-group"></a><span data-ttu-id="cd4ec-103">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="cd4ec-103">Get group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd4ec-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines [group](../resources/group.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-104">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

<span data-ttu-id="cd4ec-105">Dieser Vorgang gibt standardmäßig nur eine Teilmenge aller verfügbaren Eigenschaften zurück, wie im Abschnitt [Eigenschaften](../resources/group.md#properties) beschrieben.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="cd4ec-106">Zum Abrufen von Eigenschaften, die _nicht_ standardmäßig zurückgegeben werden, geben sie diese in einer OData-Abfrageoption `$select` an.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="cd4ec-107">Sehen Sie sich ein [Beispiel](#request-2) für `$select` an.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="cd4ec-108">Eine Ausnahme ist die **hasMembersWithLicenseErrors**-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="cd4ec-109">Sehen Sie sich ein [Beispiel](group-list.md#request-2) für die Verwendung dieser Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

<span data-ttu-id="cd4ec-110">Da die **group**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **group**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-110">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd4ec-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd4ec-111">Permissions</span></span>
<span data-ttu-id="cd4ec-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd4ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd4ec-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd4ec-114">Permission type</span></span>      | <span data-ttu-id="cd4ec-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd4ec-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd4ec-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd4ec-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cd4ec-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd4ec-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd4ec-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd4ec-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd4ec-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd4ec-119">Not supported.</span></span>    |
|<span data-ttu-id="cd4ec-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd4ec-120">Application</span></span> | <span data-ttu-id="cd4ec-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd4ec-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd4ec-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd4ec-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cd4ec-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cd4ec-123">Optional query parameters</span></span>
<span data-ttu-id="cd4ec-124">Mit `$select` können Sie bestimmte Gruppeneigenschaften abrufen, einschließlich derjenigen, die standardmäßig nicht zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="cd4ec-125">Unten finden Sie ein [Beispiel](#request-2).</span><span class="sxs-lookup"><span data-stu-id="cd4ec-125">See an [example](#request-2) below.</span></span>

<span data-ttu-id="cd4ec-126">Weitere Informationen zu OData-Abfrageoptionen finden Sie unter [OData-Abfrageparameter](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cd4ec-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd4ec-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd4ec-127">Request headers</span></span>
| <span data-ttu-id="cd4ec-128">Name</span><span class="sxs-lookup"><span data-stu-id="cd4ec-128">Name</span></span>       | <span data-ttu-id="cd4ec-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cd4ec-129">Type</span></span> | <span data-ttu-id="cd4ec-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd4ec-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cd4ec-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd4ec-131">Authorization</span></span>  | <span data-ttu-id="cd4ec-132">string</span><span class="sxs-lookup"><span data-stu-id="cd4ec-132">string</span></span>  | <span data-ttu-id="cd4ec-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd4ec-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd4ec-135">Request body</span></span>
<span data-ttu-id="cd4ec-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd4ec-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd4ec-137">Response</span></span>
<span data-ttu-id="cd4ec-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-138">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="cd4ec-139">Es werden die Standardeigenschaften zurückgegeben, sofern Sie nicht mit `$select` bestimmte Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-139">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="cd4ec-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd4ec-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="cd4ec-141">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="cd4ec-141">Request 1</span></span>
<span data-ttu-id="cd4ec-142">Nachfolgend sehen Sie ein Beispiel für eine GET-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-142">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```

#### <a name="response-1"></a><span data-ttu-id="cd4ec-143">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="cd4ec-143">Response 1</span></span>
<span data-ttu-id="cd4ec-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-144">The following is an example of the response.</span></span> <span data-ttu-id="cd4ec-145">Es enthält nur die Standardeigenschaften.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-145">It includes only the default properties.</span></span>

><span data-ttu-id="cd4ec-146">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cd4ec-147">Bei einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-147">All the default properties are returned in an actual call.</span></span>
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
}
```

#### <a name="request-2"></a><span data-ttu-id="cd4ec-148">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="cd4ec-148">Request 2</span></span>
<span data-ttu-id="cd4ec-149">Das nächste Beispiel verwendet eine `$select`-Abfrageoption, um einige Eigenschaften abzurufen, die standardmäßig nicht zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-149">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="cd4ec-150">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="cd4ec-150">Response 2</span></span>
<span data-ttu-id="cd4ec-151">Nachfolgend finden Sie ein Beispiel der Antwort, die die angeforderten nicht standardmäßigen Eigenschaften umfasst.</span><span class="sxs-lookup"><span data-stu-id="cd4ec-151">The following is an example of the response which includes the requested non-default properties.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```

## <a name="see-also"></a><span data-ttu-id="cd4ec-152">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="cd4ec-152">See also</span></span>

- [<span data-ttu-id="cd4ec-153">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="cd4ec-153">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cd4ec-154">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="cd4ec-154">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="cd4ec-155">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="cd4ec-155">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
