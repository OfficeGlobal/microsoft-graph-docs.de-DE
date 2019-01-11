---
title: 'group: getMemberObjects'
description: 'Diese API gibt alle Gruppen zurück, in denen die angegebene Gruppe Mitglied ist. Die Überprüfung ist transitiv. Hinweis: Gruppen können nicht Mitglieder von Verzeichnisrollen sein, es werden daher keine Verzeichnisrollen zurückgegeben.'
localization_priority: Normal
ms.openlocfilehash: fac39adebc8220458b3fcd0a46a5de5f6e27ab4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891259"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="40fc2-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="40fc2-105">group: getMemberObjects</span></span>
<span data-ttu-id="40fc2-p102">Diese API gibt alle Gruppen zurück, in denen die angegebene Gruppe Mitglied ist. Die Überprüfung ist transitiv. Hinweis: Gruppen können nicht Mitglieder von Verzeichnisrollen sein, es werden daher keine Verzeichnisrollen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40fc2-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="40fc2-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="40fc2-109">Permissions</span></span>
<span data-ttu-id="40fc2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40fc2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40fc2-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40fc2-112">Permission type</span></span>      | <span data-ttu-id="40fc2-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40fc2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40fc2-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40fc2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="40fc2-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40fc2-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40fc2-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40fc2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40fc2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40fc2-117">Not supported.</span></span>    |
|<span data-ttu-id="40fc2-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40fc2-118">Application</span></span> | <span data-ttu-id="40fc2-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40fc2-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40fc2-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40fc2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="40fc2-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40fc2-121">Request headers</span></span>
| <span data-ttu-id="40fc2-122">Name</span><span class="sxs-lookup"><span data-stu-id="40fc2-122">Name</span></span>       | <span data-ttu-id="40fc2-123">Typ</span><span class="sxs-lookup"><span data-stu-id="40fc2-123">Type</span></span> | <span data-ttu-id="40fc2-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40fc2-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="40fc2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="40fc2-125">Authorization</span></span>  | <span data-ttu-id="40fc2-126">string</span><span class="sxs-lookup"><span data-stu-id="40fc2-126">string</span></span>  | <span data-ttu-id="40fc2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="40fc2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40fc2-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40fc2-129">Request body</span></span>
<span data-ttu-id="40fc2-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="40fc2-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="40fc2-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="40fc2-131">Parameter</span></span>    | <span data-ttu-id="40fc2-132">Typ</span><span class="sxs-lookup"><span data-stu-id="40fc2-132">Type</span></span>   |<span data-ttu-id="40fc2-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40fc2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40fc2-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="40fc2-134">securityEnabledOnly</span></span>|<span data-ttu-id="40fc2-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="40fc2-135">Boolean</span></span>| <span data-ttu-id="40fc2-p105">Festgelegt auf **false**. Die Option, dass nur Gruppen mit aktivierter Sicherheit zurückgegeben werden, wird nur für Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40fc2-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="40fc2-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="40fc2-138">Response</span></span>
<span data-ttu-id="40fc2-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="40fc2-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="40fc2-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40fc2-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="40fc2-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40fc2-141">Request</span></span>
<span data-ttu-id="40fc2-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40fc2-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="40fc2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="40fc2-143">Response</span></span>
<span data-ttu-id="40fc2-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40fc2-144">The following is an example of the response.</span></span>
><span data-ttu-id="40fc2-145">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="40fc2-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="40fc2-146">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="40fc2-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
