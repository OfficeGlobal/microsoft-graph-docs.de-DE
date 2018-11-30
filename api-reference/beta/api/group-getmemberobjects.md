---
title: 'group: getMemberObjects'
description: 'Zurückgeben Sie aller Gruppen und administrative Einheiten, denen die Gruppe ein Mitglied ist. Die Überprüfung ist transitiv. Hinweis: Gruppen können nicht Mitglieder der Directory Rollen sein, damit keine Directory Rollen zurückgegeben werden.'
ms.openlocfilehash: e0ff719b58f13f036cbf8502725fb1e146cb1227
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061529"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="21b81-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="21b81-105">group: getMemberObjects</span></span>

> <span data-ttu-id="21b81-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="21b81-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21b81-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21b81-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21b81-108">Zurückgeben Sie aller Gruppen und administrative Einheiten, denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="21b81-108">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="21b81-109">Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="21b81-109">The check is transitive.</span></span> <span data-ttu-id="21b81-110">Hinweis: Gruppen können nicht Mitglieder der Directory Rollen sein, damit keine Directory Rollen zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="21b81-110">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="21b81-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="21b81-111">Permissions</span></span>
<span data-ttu-id="21b81-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21b81-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21b81-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21b81-114">Permission type</span></span>      | <span data-ttu-id="21b81-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21b81-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21b81-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21b81-116">Delegated (work or school account)</span></span> | <span data-ttu-id="21b81-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="21b81-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="21b81-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21b81-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21b81-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21b81-119">Not supported.</span></span>    |
|<span data-ttu-id="21b81-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21b81-120">Application</span></span> | <span data-ttu-id="21b81-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21b81-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21b81-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21b81-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="21b81-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21b81-123">Request headers</span></span>
| <span data-ttu-id="21b81-124">Name</span><span class="sxs-lookup"><span data-stu-id="21b81-124">Name</span></span>       | <span data-ttu-id="21b81-125">Typ</span><span class="sxs-lookup"><span data-stu-id="21b81-125">Type</span></span> | <span data-ttu-id="21b81-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21b81-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="21b81-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="21b81-127">Authorization</span></span>  | <span data-ttu-id="21b81-128">string</span><span class="sxs-lookup"><span data-stu-id="21b81-128">string</span></span>  | <span data-ttu-id="21b81-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21b81-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21b81-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21b81-131">Request body</span></span>
<span data-ttu-id="21b81-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="21b81-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="21b81-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="21b81-133">Parameter</span></span>    | <span data-ttu-id="21b81-134">Typ</span><span class="sxs-lookup"><span data-stu-id="21b81-134">Type</span></span>   |<span data-ttu-id="21b81-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21b81-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21b81-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="21b81-136">securityEnabledOnly</span></span>|<span data-ttu-id="21b81-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="21b81-137">Boolean</span></span>|<span data-ttu-id="21b81-p106">Festgelegt auf **false**. Die Option, dass nur Gruppen mit aktivierter Sicherheit zurückgegeben werden, wird nur für Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21b81-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="21b81-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="21b81-140">Response</span></span>
<span data-ttu-id="21b81-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="21b81-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="21b81-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21b81-142">Example</span></span>
#### <a name="request"></a><span data-ttu-id="21b81-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21b81-143">Request</span></span>
<span data-ttu-id="21b81-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21b81-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="21b81-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="21b81-145">Response</span></span>
<span data-ttu-id="21b81-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="21b81-146">The following is an example of the response.</span></span>
><span data-ttu-id="21b81-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="21b81-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
