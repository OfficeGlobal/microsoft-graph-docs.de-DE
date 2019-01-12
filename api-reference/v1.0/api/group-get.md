---
title: Gruppe abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen eines Gruppenobjekts.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 7de0b9dac4d1bf3295cd01bbd522d1f18314c098
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917188"
---
# <a name="get-group"></a><span data-ttu-id="fd371-103">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="fd371-103">Get group</span></span>
<span data-ttu-id="fd371-104">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Gruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="fd371-104">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="fd371-105">Standardeigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd371-105">Default properties</span></span>

<span data-ttu-id="fd371-p101">Im Folgenden werden standardmäßige Eigenschaften dargestellt, die beim Abrufen oder beim Auflisten von Gruppen zurückgegeben werden. Diese stellen eine Teilmenge aller verfügbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="fd371-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="fd371-108">description</span><span class="sxs-lookup"><span data-stu-id="fd371-108">description</span></span>
* <span data-ttu-id="fd371-109">displayName</span><span class="sxs-lookup"><span data-stu-id="fd371-109">displayName</span></span>
* <span data-ttu-id="fd371-110">groupTypes</span><span class="sxs-lookup"><span data-stu-id="fd371-110">groupTypes</span></span>
* <span data-ttu-id="fd371-111">id</span><span class="sxs-lookup"><span data-stu-id="fd371-111">id</span></span>
* <span data-ttu-id="fd371-112">Mail</span><span class="sxs-lookup"><span data-stu-id="fd371-112">mail</span></span>
* <span data-ttu-id="fd371-113">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="fd371-113">mailEnabled</span></span>
* <span data-ttu-id="fd371-114">mailNickname</span><span class="sxs-lookup"><span data-stu-id="fd371-114">mailNickname</span></span>
* <span data-ttu-id="fd371-115">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fd371-115">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="fd371-116">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd371-116">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="fd371-117">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="fd371-117">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="fd371-118">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="fd371-118">proxyAddresses</span></span>
* <span data-ttu-id="fd371-119">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="fd371-119">securityEnabled</span></span>
* <span data-ttu-id="fd371-120">visibility</span><span class="sxs-lookup"><span data-stu-id="fd371-120">visibility</span></span>

<span data-ttu-id="fd371-121">Die folgenden Gruppeneigenschaften werden standardmäßig nicht zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="fd371-121">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="fd371-122">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="fd371-122">allowExternalSenders</span></span>
* <span data-ttu-id="fd371-123">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="fd371-123">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="fd371-124">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="fd371-124">isSubscribedByMail</span></span>
* <span data-ttu-id="fd371-125">unseenCount</span><span class="sxs-lookup"><span data-stu-id="fd371-125">unseenCount</span></span>

<span data-ttu-id="fd371-p102">Verwenden Sie zum Abrufen dieser Eigenschaften den **$select**-Abfrageparameter. Es folgen Beispiele:</span><span class="sxs-lookup"><span data-stu-id="fd371-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="fd371-128">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd371-128">Permissions</span></span>
<span data-ttu-id="fd371-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd371-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd371-131">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd371-131">Permission type</span></span>      | <span data-ttu-id="fd371-132">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd371-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd371-133">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd371-133">Delegated (work or school account)</span></span> | <span data-ttu-id="fd371-134">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd371-134">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd371-135">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd371-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd371-136">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd371-136">Not supported.</span></span>    |
|<span data-ttu-id="fd371-137">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd371-137">Application</span></span> | <span data-ttu-id="fd371-138">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd371-138">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd371-139">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd371-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd371-140">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fd371-140">Optional query parameters</span></span>
<span data-ttu-id="fd371-141">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd371-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd371-142">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd371-142">Request headers</span></span>
| <span data-ttu-id="fd371-143">Name</span><span class="sxs-lookup"><span data-stu-id="fd371-143">Name</span></span>       | <span data-ttu-id="fd371-144">Typ</span><span class="sxs-lookup"><span data-stu-id="fd371-144">Type</span></span> | <span data-ttu-id="fd371-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd371-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fd371-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd371-146">Authorization</span></span>  | <span data-ttu-id="fd371-147">string</span><span class="sxs-lookup"><span data-stu-id="fd371-147">string</span></span>  | <span data-ttu-id="fd371-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd371-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd371-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd371-150">Request body</span></span>
<span data-ttu-id="fd371-151">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd371-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd371-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd371-152">Response</span></span>
<span data-ttu-id="fd371-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd371-153">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd371-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd371-154">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fd371-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd371-155">Request</span></span>
<span data-ttu-id="fd371-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd371-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="fd371-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd371-157">Response</span></span>
<span data-ttu-id="fd371-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd371-158">The following is an example of the response.</span></span>

><span data-ttu-id="fd371-159">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="fd371-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fd371-160">Von einem tatsächlichen Aufruf werden, wie zuvor beschrieben, die Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd371-160">The default properties will be returned from an actual call, as described before.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
