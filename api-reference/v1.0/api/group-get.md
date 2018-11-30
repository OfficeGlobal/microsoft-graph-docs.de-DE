---
title: Gruppe abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen eines Gruppenobjekts.
ms.openlocfilehash: fbae878043580a9c5495b0462290e1da7af3bdd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017974"
---
# <a name="get-group"></a><span data-ttu-id="07e4b-103">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="07e4b-103">Get group</span></span>
<span data-ttu-id="07e4b-104">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Gruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="07e4b-104">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="07e4b-105">Standardeigenschaften</span><span class="sxs-lookup"><span data-stu-id="07e4b-105">Default properties</span></span>

<span data-ttu-id="07e4b-p101">Im Folgenden werden standardmäßige Eigenschaften dargestellt, die beim Abrufen oder beim Auflisten von Gruppen zurückgegeben werden. Diese stellen eine Teilmenge aller verfügbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="07e4b-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="07e4b-108">description</span><span class="sxs-lookup"><span data-stu-id="07e4b-108">description</span></span>
* <span data-ttu-id="07e4b-109">displayName</span><span class="sxs-lookup"><span data-stu-id="07e4b-109">displayName</span></span>
* <span data-ttu-id="07e4b-110">groupTypes</span><span class="sxs-lookup"><span data-stu-id="07e4b-110">groupTypes</span></span>
* <span data-ttu-id="07e4b-111">id</span><span class="sxs-lookup"><span data-stu-id="07e4b-111">id</span></span>
* <span data-ttu-id="07e4b-112">Mail</span><span class="sxs-lookup"><span data-stu-id="07e4b-112">mail</span></span>
* <span data-ttu-id="07e4b-113">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="07e4b-113">mailEnabled</span></span>
* <span data-ttu-id="07e4b-114">mailNickname</span><span class="sxs-lookup"><span data-stu-id="07e4b-114">mailNickname</span></span>
* <span data-ttu-id="07e4b-115">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="07e4b-115">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="07e4b-116">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="07e4b-116">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="07e4b-117">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="07e4b-117">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="07e4b-118">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="07e4b-118">proxyAddresses</span></span>
* <span data-ttu-id="07e4b-119">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="07e4b-119">securityEnabled</span></span>
* <span data-ttu-id="07e4b-120">visibility</span><span class="sxs-lookup"><span data-stu-id="07e4b-120">visibility</span></span>

<span data-ttu-id="07e4b-121">Die folgenden Gruppeneigenschaften werden standardmäßig nicht zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="07e4b-121">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="07e4b-122">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="07e4b-122">allowExternalSenders</span></span>
* <span data-ttu-id="07e4b-123">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="07e4b-123">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="07e4b-124">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="07e4b-124">isSubscribedByMail</span></span>
* <span data-ttu-id="07e4b-125">unseenCount</span><span class="sxs-lookup"><span data-stu-id="07e4b-125">unseenCount</span></span>

<span data-ttu-id="07e4b-p102">Verwenden Sie zum Abrufen dieser Eigenschaften den **$select**-Abfrageparameter. Es folgen Beispiele:</span><span class="sxs-lookup"><span data-stu-id="07e4b-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="07e4b-128">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07e4b-128">Permissions</span></span>
<span data-ttu-id="07e4b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07e4b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07e4b-131">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07e4b-131">Permission type</span></span>      | <span data-ttu-id="07e4b-132">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07e4b-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07e4b-133">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07e4b-133">Delegated (work or school account)</span></span> | <span data-ttu-id="07e4b-134">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07e4b-134">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="07e4b-135">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07e4b-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07e4b-136">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07e4b-136">Not supported.</span></span>    |
|<span data-ttu-id="07e4b-137">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07e4b-137">Application</span></span> | <span data-ttu-id="07e4b-138">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07e4b-138">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07e4b-139">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07e4b-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07e4b-140">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="07e4b-140">Optional query parameters</span></span>
<span data-ttu-id="07e4b-141">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="07e4b-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07e4b-142">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07e4b-142">Request headers</span></span>
| <span data-ttu-id="07e4b-143">Name</span><span class="sxs-lookup"><span data-stu-id="07e4b-143">Name</span></span>       | <span data-ttu-id="07e4b-144">Typ</span><span class="sxs-lookup"><span data-stu-id="07e4b-144">Type</span></span> | <span data-ttu-id="07e4b-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07e4b-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="07e4b-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="07e4b-146">Authorization</span></span>  | <span data-ttu-id="07e4b-147">string</span><span class="sxs-lookup"><span data-stu-id="07e4b-147">string</span></span>  | <span data-ttu-id="07e4b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07e4b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07e4b-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07e4b-150">Request body</span></span>
<span data-ttu-id="07e4b-151">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="07e4b-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07e4b-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="07e4b-152">Response</span></span>
<span data-ttu-id="07e4b-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07e4b-153">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07e4b-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07e4b-154">Example</span></span>
#### <a name="request"></a><span data-ttu-id="07e4b-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07e4b-155">Request</span></span>
<span data-ttu-id="07e4b-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07e4b-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="07e4b-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="07e4b-157">Response</span></span>
<span data-ttu-id="07e4b-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="07e4b-158">The following is an example of the response.</span></span>

><span data-ttu-id="07e4b-159">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="07e4b-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07e4b-160">Von einem tatsächlichen Aufruf werden, wie zuvor beschrieben, die Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07e4b-160">The default properties will be returned from an actual call, as described before.</span></span>
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
