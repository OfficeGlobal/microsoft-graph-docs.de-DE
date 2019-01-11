---
title: 'group: getMemberGroups'
description: Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist von. Die Überprüfung ist transitiv; im Gegensatz zum Lesen der Navigationseigenschaft Mitglied, die nur die Gruppen zurückgibt, deren direktes Mitglied die Gruppe ist.
localization_priority: Priority
ms.openlocfilehash: 3af6672b38271cea3fea94de535b91d2efee9b45
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875656"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="a20bb-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="a20bb-104">group: getMemberGroups</span></span>

<span data-ttu-id="a20bb-p102">Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist von. Die Überprüfung ist transitiv; im Gegensatz zum Lesen der Navigationseigenschaft [Mitglied](../api/group-list-memberof.md), die nur die Gruppen zurückgibt, deren direktes Mitglied die Gruppe ist.</span><span class="sxs-lookup"><span data-stu-id="a20bb-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="a20bb-p103">Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Die maximale Anzahl von Gruppen, die jede Anfrage zurückgeben kann, ist 2046. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten können. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="a20bb-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="a20bb-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a20bb-111">Permissions</span></span>

<span data-ttu-id="a20bb-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a20bb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a20bb-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a20bb-114">Permission type</span></span>                        | <span data-ttu-id="a20bb-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a20bb-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="a20bb-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a20bb-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="a20bb-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a20bb-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="a20bb-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a20bb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a20bb-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a20bb-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="a20bb-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a20bb-120">Application</span></span>                            | <span data-ttu-id="a20bb-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a20bb-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="a20bb-122">**Hinweis:** Diese API derzeit erfordert die `Directory.Read.All` Berechtigung oder höher.</span><span class="sxs-lookup"><span data-stu-id="a20bb-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="a20bb-123">Mithilfe der `Group.Read.All` Berechtigung gibt einen Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="a20bb-123">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="a20bb-124">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="a20bb-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="a20bb-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a20bb-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="a20bb-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a20bb-126">Request headers</span></span>

| <span data-ttu-id="a20bb-127">Name</span><span class="sxs-lookup"><span data-stu-id="a20bb-127">Name</span></span>          | <span data-ttu-id="a20bb-128">Typ</span><span class="sxs-lookup"><span data-stu-id="a20bb-128">Type</span></span>   | <span data-ttu-id="a20bb-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a20bb-129">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="a20bb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a20bb-130">Authorization</span></span> | <span data-ttu-id="a20bb-131">string</span><span class="sxs-lookup"><span data-stu-id="a20bb-131">string</span></span> | <span data-ttu-id="a20bb-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a20bb-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a20bb-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a20bb-134">Request body</span></span>

<span data-ttu-id="a20bb-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a20bb-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a20bb-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="a20bb-136">Parameter</span></span>           | <span data-ttu-id="a20bb-137">Typ</span><span class="sxs-lookup"><span data-stu-id="a20bb-137">Type</span></span>    | <span data-ttu-id="a20bb-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a20bb-138">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="a20bb-139">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a20bb-139">securityEnabledOnly</span></span> | <span data-ttu-id="a20bb-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a20bb-140">Boolean</span></span> | <span data-ttu-id="a20bb-p107">Festgelegt auf **false**. Die Option, dass nur Gruppen mit aktivierter Sicherheit zurückgegeben werden, wird nur für Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a20bb-p107">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="a20bb-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="a20bb-143">Response</span></span>

<span data-ttu-id="a20bb-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="a20bb-144">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="a20bb-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a20bb-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a20bb-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a20bb-146">Request</span></span>

<span data-ttu-id="a20bb-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a20bb-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="a20bb-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="a20bb-148">Response</span></span>

<span data-ttu-id="a20bb-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a20bb-149">The following is an example of the response.</span></span>

> <span data-ttu-id="a20bb-150">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="a20bb-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a20bb-151">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a20bb-151">All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
