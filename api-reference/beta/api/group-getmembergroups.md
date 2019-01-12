---
title: 'group: getMemberGroups'
description: Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist von. Die Überprüfung ist transitiv; im Gegensatz zum Lesen der Navigationseigenschaft Mitglied, die nur die Gruppen zurückgibt, deren direktes Mitglied die Gruppe ist.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e485c80a06fc2d124dec728ab3ffcdfb8dcce105
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921535"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="8ee7b-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="8ee7b-104">group: getMemberGroups</span></span>

> <span data-ttu-id="8ee7b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ee7b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ee7b-p103">Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist von. Die Überprüfung ist transitiv; im Gegensatz zum Lesen der Navigationseigenschaft [Mitglied](../api/group-list-memberof.md), die nur die Gruppen zurückgibt, deren direktes Mitglied die Gruppe ist.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-p103">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="8ee7b-p104">Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Die maximale Anzahl von Gruppen, die jede Anfrage zurückgeben kann, ist 2046. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten können. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-p104">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ee7b-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ee7b-113">Permissions</span></span>

<span data-ttu-id="8ee7b-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ee7b-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ee7b-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ee7b-116">Permission type</span></span>                        | <span data-ttu-id="8ee7b-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ee7b-117">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="8ee7b-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ee7b-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ee7b-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ee7b-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8ee7b-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ee7b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ee7b-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ee7b-121">Not supported.</span></span>                                                                              |
| <span data-ttu-id="8ee7b-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ee7b-122">Application</span></span>                            | <span data-ttu-id="8ee7b-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ee7b-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="8ee7b-124">**Hinweis:** Diese API derzeit erfordert die `Directory.Read.All` Berechtigung oder höher.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="8ee7b-125">Mithilfe der `Group.Read.All` Berechtigung gibt einen Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-125">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="8ee7b-126">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="8ee7b-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ee7b-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="8ee7b-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ee7b-128">Request headers</span></span>

| <span data-ttu-id="8ee7b-129">Name</span><span class="sxs-lookup"><span data-stu-id="8ee7b-129">Name</span></span>          | <span data-ttu-id="8ee7b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="8ee7b-130">Type</span></span>   | <span data-ttu-id="8ee7b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ee7b-131">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="8ee7b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ee7b-132">Authorization</span></span> | <span data-ttu-id="8ee7b-133">string</span><span class="sxs-lookup"><span data-stu-id="8ee7b-133">string</span></span> | <span data-ttu-id="8ee7b-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ee7b-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ee7b-136">Request body</span></span>

<span data-ttu-id="8ee7b-137">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ee7b-138">Parameter</span><span class="sxs-lookup"><span data-stu-id="8ee7b-138">Parameter</span></span>           | <span data-ttu-id="8ee7b-139">Typ</span><span class="sxs-lookup"><span data-stu-id="8ee7b-139">Type</span></span>    | <span data-ttu-id="8ee7b-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ee7b-140">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="8ee7b-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="8ee7b-141">securityEnabledOnly</span></span> | <span data-ttu-id="8ee7b-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8ee7b-142">Boolean</span></span> | <span data-ttu-id="8ee7b-p108">Festgelegt auf **false**. Die Option, dass nur Gruppen mit aktivierter Sicherheit zurückgegeben werden, wird nur für Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-p108">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="8ee7b-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ee7b-145">Response</span></span>

<span data-ttu-id="8ee7b-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-146">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="8ee7b-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ee7b-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8ee7b-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ee7b-148">Request</span></span>

<span data-ttu-id="8ee7b-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="8ee7b-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ee7b-150">Response</span></span>

<span data-ttu-id="8ee7b-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-151">The following is an example of the response.</span></span>

> <span data-ttu-id="8ee7b-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
