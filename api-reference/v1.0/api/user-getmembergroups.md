---
title: 'user: getMemberGroups'
description: Zurückgeben Sie aller Gruppen, denen der Benutzer Mitglied ist. Das Kontrollkästchen ist transitiv, im Gegensatz zum Lesen der
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb8caefae8b7c3ced9630309cae51a3b74b45937
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969205"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="15ccf-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="15ccf-104">user: getMemberGroups</span></span>

<span data-ttu-id="15ccf-p102">Gibt alle Gruppen zurück, bei denen der Benutzer Mitglied ist. Die Überprüfung ist transitiv; im Gegensatz zum Lesen der Navigationseigenschaft [memberOf](../api/user-list-memberof.md), die nur die Gruppen zurückgibt, von denen der Benutzer ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="15ccf-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="15ccf-p103">Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Die maximale Anzahl von Gruppen, die jede Anfrage zurückgeben kann, ist 2046. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten können. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="15ccf-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="15ccf-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="15ccf-111">Permissions</span></span>

<span data-ttu-id="15ccf-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ccf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15ccf-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15ccf-114">Permission type</span></span>                        | <span data-ttu-id="15ccf-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15ccf-115">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="15ccf-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15ccf-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="15ccf-117">~~User.Read and Group.Read.All~~, ~~User.ReadBasic.All and Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15ccf-117">~~User.Read and Group.Read.All~~, ~~User.ReadBasic.All and Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="15ccf-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15ccf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15ccf-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15ccf-119">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="15ccf-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15ccf-120">Application</span></span>                            | <span data-ttu-id="15ccf-121">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ccf-121">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span></span>                                                                                        |

> <span data-ttu-id="15ccf-122">**Hinweis:** Diese API derzeit erfordert die `Directory.Read.All` Berechtigung oder höher.</span><span class="sxs-lookup"><span data-stu-id="15ccf-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="15ccf-123">Verwenden die Berechtigung Group.Read.All eigenständig oder in Kombination mit einem `User.` Berechtigung, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ccf-123">Using the Group.Read.All permission, either alone or in combination with a `User.` permission, will return an error.</span></span> <span data-ttu-id="15ccf-124">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="15ccf-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="15ccf-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15ccf-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="15ccf-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15ccf-126">Request headers</span></span>

| <span data-ttu-id="15ccf-127">Header</span><span class="sxs-lookup"><span data-stu-id="15ccf-127">Header</span></span>        | <span data-ttu-id="15ccf-128">Wert</span><span class="sxs-lookup"><span data-stu-id="15ccf-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="15ccf-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="15ccf-129">Authorization</span></span> | <span data-ttu-id="15ccf-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15ccf-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15ccf-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15ccf-132">Content-Type</span></span>  | <span data-ttu-id="15ccf-133">application/json</span><span class="sxs-lookup"><span data-stu-id="15ccf-133">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="15ccf-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15ccf-134">Request body</span></span>

<span data-ttu-id="15ccf-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="15ccf-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="15ccf-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="15ccf-136">Parameter</span></span>           | <span data-ttu-id="15ccf-137">Typ</span><span class="sxs-lookup"><span data-stu-id="15ccf-137">Type</span></span>    | <span data-ttu-id="15ccf-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15ccf-138">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="15ccf-139">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="15ccf-139">securityEnabledOnly</span></span> | <span data-ttu-id="15ccf-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="15ccf-140">Boolean</span></span> | <span data-ttu-id="15ccf-p107">**true** gibt an, dass nur Sicherheitsgruppen, in denen der Benutzer Mitglied ist, zurückgegeben werden sollen; **false** gibt an, dass alle Gruppen, von denen der Benutzer ein Mitglied ist, zurückgegeben werden sollen. Hinweis: Dieser Parameter darf nur auf **true** gesetzt werden, wenn diese Methode auf einen Benutzer angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="15ccf-p107">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="15ccf-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="15ccf-143">Response</span></span>

<span data-ttu-id="15ccf-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen der Benutzer ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="15ccf-144">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="15ccf-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15ccf-145">Example</span></span>

<span data-ttu-id="15ccf-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="15ccf-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="15ccf-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15ccf-147">Request</span></span>

<span data-ttu-id="15ccf-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15ccf-148">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="15ccf-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="15ccf-149">Response</span></span>

<span data-ttu-id="15ccf-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ccf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
