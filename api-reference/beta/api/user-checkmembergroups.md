---
title: checkMemberGroups
description: Überprüfen Sie die Mitgliedschaft in der angegebenen Liste von Gruppen. Diese Gruppen, denen zurückgegeben aus der Liste
ms.openlocfilehash: c6e232a6c34c0bbffdb41695a51694a688fecc7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058535"
---
# <a name="checkmembergroups"></a><span data-ttu-id="e99b7-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e99b7-104">checkMemberGroups</span></span>

> <span data-ttu-id="e99b7-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e99b7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e99b7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e99b7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e99b7-p103">Sucht nach einer Mitgliedschaft in einer angegebenenListe von Gruppen. Gibt aus der Liste diesjenigen Gruppen zurück, bei denen der Benutzer über eine direkte oder transitive Mitgliedschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="e99b7-p103">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="e99b7-p104">Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="e99b7-p104">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="e99b7-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e99b7-113">Permissions</span></span>

<span data-ttu-id="e99b7-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e99b7-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e99b7-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e99b7-116">Permission type</span></span>                        | <span data-ttu-id="e99b7-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e99b7-117">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e99b7-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e99b7-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="e99b7-119">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e99b7-119">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="e99b7-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e99b7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e99b7-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e99b7-121">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="e99b7-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e99b7-122">Application</span></span>                            | <span data-ttu-id="e99b7-123">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e99b7-123">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="e99b7-124">**Hinweis:** Diese API derzeit erfordert die `Directory.Read.All` Berechtigung oder höher.</span><span class="sxs-lookup"><span data-stu-id="e99b7-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="e99b7-125">Mithilfe der `User.Read.All` oder `User.ReadWrite.All` Berechtigungen werden ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e99b7-125">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="e99b7-126">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="e99b7-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="e99b7-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e99b7-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="e99b7-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e99b7-128">Request headers</span></span>

| <span data-ttu-id="e99b7-129">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e99b7-129">Header</span></span>        | <span data-ttu-id="e99b7-130">Wert</span><span class="sxs-lookup"><span data-stu-id="e99b7-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="e99b7-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e99b7-131">Authorization</span></span> | <span data-ttu-id="e99b7-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e99b7-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e99b7-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e99b7-134">Content-Type</span></span>  | <span data-ttu-id="e99b7-135">application/json</span><span class="sxs-lookup"><span data-stu-id="e99b7-135">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="e99b7-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e99b7-136">Request body</span></span>

<span data-ttu-id="e99b7-137">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e99b7-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e99b7-138">Parameter</span><span class="sxs-lookup"><span data-stu-id="e99b7-138">Parameter</span></span> | <span data-ttu-id="e99b7-139">Typ</span><span class="sxs-lookup"><span data-stu-id="e99b7-139">Type</span></span>   | <span data-ttu-id="e99b7-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e99b7-140">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="e99b7-141">groupIds</span><span class="sxs-lookup"><span data-stu-id="e99b7-141">groupIds</span></span>  | <span data-ttu-id="e99b7-142">String</span><span class="sxs-lookup"><span data-stu-id="e99b7-142">String</span></span> | <span data-ttu-id="e99b7-143">Ein Array von Gruppen-IDs</span><span class="sxs-lookup"><span data-stu-id="e99b7-143">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="e99b7-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e99b7-144">Response</span></span>

<span data-ttu-id="e99b7-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e99b7-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e99b7-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e99b7-146">Example</span></span>

<span data-ttu-id="e99b7-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e99b7-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e99b7-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e99b7-148">Request</span></span>

<span data-ttu-id="e99b7-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e99b7-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="e99b7-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="e99b7-150">Response</span></span>

<span data-ttu-id="e99b7-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e99b7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
