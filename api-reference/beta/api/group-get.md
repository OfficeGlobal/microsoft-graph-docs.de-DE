---
title: Gruppe abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen eines Gruppenobjekts.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 99215af564be186edaf57563ae493f363c9cc2fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941051"
---
# <a name="get-group"></a><span data-ttu-id="89100-103">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="89100-103">Get group</span></span>

> <span data-ttu-id="89100-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="89100-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89100-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="89100-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89100-106">Rufen Sie die Eigenschaften und die Beziehungen eines [Group](../resources/group.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="89100-106">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="89100-107">Standardeigenschaften</span><span class="sxs-lookup"><span data-stu-id="89100-107">Default properties</span></span>

<span data-ttu-id="89100-p102">Im Folgenden werden standardmäßige Eigenschaften dargestellt, die beim Abrufen oder beim Auflisten von Gruppen zurückgegeben werden. Diese stellen eine Teilmenge aller verfügbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="89100-p102">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="89100-110">Klassifikation</span><span class="sxs-lookup"><span data-stu-id="89100-110">classification</span></span>
* <span data-ttu-id="89100-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89100-111">createdDateTime</span></span>
* <span data-ttu-id="89100-112">description</span><span class="sxs-lookup"><span data-stu-id="89100-112">description</span></span>
* <span data-ttu-id="89100-113">displayName</span><span class="sxs-lookup"><span data-stu-id="89100-113">displayName</span></span>
* <span data-ttu-id="89100-114">groupTypes</span><span class="sxs-lookup"><span data-stu-id="89100-114">groupTypes</span></span>
* <span data-ttu-id="89100-115">id</span><span class="sxs-lookup"><span data-stu-id="89100-115">id</span></span>
* <span data-ttu-id="89100-116">Mail</span><span class="sxs-lookup"><span data-stu-id="89100-116">mail</span></span>
* <span data-ttu-id="89100-117">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="89100-117">mailEnabled</span></span>
* <span data-ttu-id="89100-118">mailNickname</span><span class="sxs-lookup"><span data-stu-id="89100-118">mailNickname</span></span>
* <span data-ttu-id="89100-119">membershipRule</span><span class="sxs-lookup"><span data-stu-id="89100-119">membershipRule</span></span>
* <span data-ttu-id="89100-120">membershipRuleProcessingState</span><span class="sxs-lookup"><span data-stu-id="89100-120">membershipRuleProcessingState</span></span>
* <span data-ttu-id="89100-121">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="89100-121">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="89100-122">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="89100-122">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="89100-123">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="89100-123">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="89100-124">PreferredLanguage - nicht unterstützt; Set und gibt ein Wert für diese Eigenschaft nicht `null` aufgerufen.</span><span class="sxs-lookup"><span data-stu-id="89100-124">preferredLanguage - Not supported; a value for this property cannot be set and returns `null` when called.</span></span>
* <span data-ttu-id="89100-125">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="89100-125">proxyAddresses</span></span>
* <span data-ttu-id="89100-126">renewedDateTime</span><span class="sxs-lookup"><span data-stu-id="89100-126">renewedDateTime</span></span>
* <span data-ttu-id="89100-127">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="89100-127">securityEnabled</span></span>
* <span data-ttu-id="89100-128">Design</span><span class="sxs-lookup"><span data-stu-id="89100-128">theme</span></span>
* <span data-ttu-id="89100-129">visibility</span><span class="sxs-lookup"><span data-stu-id="89100-129">visibility</span></span>

<span data-ttu-id="89100-130">Die folgenden Gruppeneigenschaften werden standardmäßig nicht zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="89100-130">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="89100-131">accessType</span><span class="sxs-lookup"><span data-stu-id="89100-131">accessType</span></span>
* <span data-ttu-id="89100-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="89100-132">allowExternalSenders</span></span>
* <span data-ttu-id="89100-133">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="89100-133">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="89100-134">hasMembersWithLicenseErrors</span><span class="sxs-lookup"><span data-stu-id="89100-134">hasMembersWithLicenseErrors</span></span>
* <span data-ttu-id="89100-135">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="89100-135">isSubscribedByMail</span></span>
* <span data-ttu-id="89100-136">isFavorite</span><span class="sxs-lookup"><span data-stu-id="89100-136">isFavorite</span></span>
* <span data-ttu-id="89100-137">unseenConversationsCount</span><span class="sxs-lookup"><span data-stu-id="89100-137">unseenConversationsCount</span></span>
* <span data-ttu-id="89100-138">unseenCount</span><span class="sxs-lookup"><span data-stu-id="89100-138">unseenCount</span></span>
* <span data-ttu-id="89100-139">unseenMessagesCount</span><span class="sxs-lookup"><span data-stu-id="89100-139">unseenMessagesCount</span></span>

<span data-ttu-id="89100-140">Wenn Sie diese Eigenschaften (außer **IsFavorite** und **HasMembersWithLicenseErrors**) erhalten möchten, verwenden Sie die `$select` Parameter Abfragen.</span><span class="sxs-lookup"><span data-stu-id="89100-140">To get these properties (except **isFavorite** and **hasMembersWithLicenseErrors**), use the `$select` query parameter.</span></span> <span data-ttu-id="89100-141">Es folgen Beispiele:</span><span class="sxs-lookup"><span data-stu-id="89100-141">The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```

<span data-ttu-id="89100-142">Verwenden Sie zum Zurückgeben von Gruppen, die Elemente mit Fehlern Lizenz enthält die **$filter** Abfragezeichenfolgen-Parameter:</span><span class="sxs-lookup"><span data-stu-id="89100-142">To return groups containing members with license errors, use the **$filter** query parameter:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true
```

<span data-ttu-id="89100-143">Da die **Group** -Ressource [Extensions](/graph/extensibility-overview)unterstützt, können Sie auch die `GET` Vorgang zum Abrufen von benutzerdefinierten Eigenschaften und Erweiterungsdaten in eine **Gruppe** -Instanz.</span><span class="sxs-lookup"><span data-stu-id="89100-143">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="89100-144">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="89100-144">Permissions</span></span>
<span data-ttu-id="89100-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89100-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89100-147">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89100-147">Permission type</span></span>      | <span data-ttu-id="89100-148">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89100-148">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89100-149">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89100-149">Delegated (work or school account)</span></span> | <span data-ttu-id="89100-150">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89100-150">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="89100-151">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89100-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89100-152">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89100-152">Not supported.</span></span>    |
|<span data-ttu-id="89100-153">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89100-153">Application</span></span> | <span data-ttu-id="89100-154">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89100-154">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89100-155">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89100-155">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89100-156">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="89100-156">Optional query parameters</span></span>
<span data-ttu-id="89100-157">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="89100-157">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89100-158">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89100-158">Request headers</span></span>
| <span data-ttu-id="89100-159">Name</span><span class="sxs-lookup"><span data-stu-id="89100-159">Name</span></span>       | <span data-ttu-id="89100-160">Typ</span><span class="sxs-lookup"><span data-stu-id="89100-160">Type</span></span> | <span data-ttu-id="89100-161">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89100-161">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="89100-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="89100-162">Authorization</span></span>  | <span data-ttu-id="89100-163">string</span><span class="sxs-lookup"><span data-stu-id="89100-163">string</span></span>  | <span data-ttu-id="89100-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="89100-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89100-166">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89100-166">Request body</span></span>
<span data-ttu-id="89100-167">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="89100-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89100-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="89100-168">Response</span></span>
<span data-ttu-id="89100-169">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89100-169">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89100-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89100-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="89100-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89100-171">Request</span></span>
<span data-ttu-id="89100-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89100-172">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="89100-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="89100-173">Response</span></span>
<span data-ttu-id="89100-174">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="89100-174">The following is an example of the response.</span></span> 
><span data-ttu-id="89100-175">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="89100-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="89100-176">Von einem tatsächlichen Aufruf werden, wie zuvor beschrieben, die Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89100-176">The default properties will be returned from an actual call, as described before.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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
```

## <a name="see-also"></a><span data-ttu-id="89100-177">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="89100-177">See also</span></span>

- [<span data-ttu-id="89100-178">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="89100-178">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="89100-179">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="89100-179">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="89100-180">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="89100-180">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
