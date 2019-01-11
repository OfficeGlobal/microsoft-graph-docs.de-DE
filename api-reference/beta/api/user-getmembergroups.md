---
title: 'user: getMemberGroups'
description: Zurückgeben Sie aller Gruppen, denen der Benutzer Mitglied ist. Das Kontrollkästchen ist transitiv, im Gegensatz zum Lesen der
localization_priority: Normal
ms.openlocfilehash: 097d6d6eafa031bf86460e97ced58d0063eee4ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879786"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="230d2-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="230d2-104">user: getMemberGroups</span></span>

> <span data-ttu-id="230d2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="230d2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="230d2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="230d2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="230d2-p103">Gibt alle Gruppen zurück, bei denen der Benutzer Mitglied ist. Die Überprüfung ist transitiv; im Gegensatz zum Lesen der Navigationseigenschaft [memberOf](../api/user-list-memberof.md), die nur die Gruppen zurückgibt, von denen der Benutzer ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="230d2-p103">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="230d2-p104">Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Die maximale Anzahl von Gruppen, die jede Anfrage zurückgeben kann, ist 2046. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten können. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="230d2-p104">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="230d2-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="230d2-113">Permissions</span></span>

<span data-ttu-id="230d2-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="230d2-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="230d2-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="230d2-116">Permission type</span></span>                        | <span data-ttu-id="230d2-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="230d2-117">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="230d2-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="230d2-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="230d2-119">~~User.Read and Group.Read.All~~, ~~User.ReadBasic.All and Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="230d2-119">~~User.Read and Group.Read.All~~, ~~User.ReadBasic.All and Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="230d2-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="230d2-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="230d2-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="230d2-121">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="230d2-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="230d2-122">Application</span></span>                            | <span data-ttu-id="230d2-123">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="230d2-123">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span></span>                                                                                        |

> <span data-ttu-id="230d2-124">**Hinweis:** Diese API derzeit erfordert die `Directory.Read.All` Berechtigung oder höher.</span><span class="sxs-lookup"><span data-stu-id="230d2-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="230d2-125">Verwenden die Berechtigung Group.Read.All eigenständig oder in Kombination mit einem `User.` Berechtigung, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="230d2-125">Using the Group.Read.All permission, either alone or in combination with a `User.` permission, will return an error.</span></span> <span data-ttu-id="230d2-126">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="230d2-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="230d2-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="230d2-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="230d2-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="230d2-128">Request headers</span></span>

| <span data-ttu-id="230d2-129">Header</span><span class="sxs-lookup"><span data-stu-id="230d2-129">Header</span></span>        | <span data-ttu-id="230d2-130">Wert</span><span class="sxs-lookup"><span data-stu-id="230d2-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="230d2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="230d2-131">Authorization</span></span> | <span data-ttu-id="230d2-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="230d2-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="230d2-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="230d2-134">Content-Type</span></span>  | <span data-ttu-id="230d2-135">application/json</span><span class="sxs-lookup"><span data-stu-id="230d2-135">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="230d2-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="230d2-136">Request body</span></span>

<span data-ttu-id="230d2-137">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="230d2-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="230d2-138">Parameter</span><span class="sxs-lookup"><span data-stu-id="230d2-138">Parameter</span></span>           | <span data-ttu-id="230d2-139">Typ</span><span class="sxs-lookup"><span data-stu-id="230d2-139">Type</span></span>    | <span data-ttu-id="230d2-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="230d2-140">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="230d2-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="230d2-141">securityEnabledOnly</span></span> | <span data-ttu-id="230d2-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="230d2-142">Boolean</span></span> | <span data-ttu-id="230d2-p108">**true** gibt an, dass nur Sicherheitsgruppen, in denen der Benutzer Mitglied ist, zurückgegeben werden sollen; **false** gibt an, dass alle Gruppen, von denen der Benutzer ein Mitglied ist, zurückgegeben werden sollen. Hinweis: Dieser Parameter darf nur auf **true** gesetzt werden, wenn diese Methode auf einen Benutzer angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="230d2-p108">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="230d2-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="230d2-145">Response</span></span>

<span data-ttu-id="230d2-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen der Benutzer ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="230d2-146">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="230d2-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="230d2-147">Example</span></span>

<span data-ttu-id="230d2-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="230d2-148">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="230d2-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="230d2-149">Request</span></span>

<span data-ttu-id="230d2-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="230d2-150">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="230d2-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="230d2-151">Response</span></span>

<span data-ttu-id="230d2-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="230d2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
