---
title: checkMemberGroups
description: Überprüfen Sie die Mitgliedschaft in der angegebenen Liste von Gruppen. Diese Gruppen, denen zurückgegeben aus der Liste
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: ee19b25648131cfa56e110c252c245436816ccbd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805523"
---
# <a name="checkmembergroups"></a><span data-ttu-id="8a75f-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="8a75f-104">checkMemberGroups</span></span>

<span data-ttu-id="8a75f-p102">Sucht nach einer Mitgliedschaft in einer angegebenenListe von Gruppen. Gibt aus der Liste diesjenigen Gruppen zurück, bei denen der Benutzer über eine direkte oder transitive Mitgliedschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="8a75f-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="8a75f-p103">Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="8a75f-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a75f-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a75f-111">Permissions</span></span>

<span data-ttu-id="8a75f-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a75f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a75f-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a75f-114">Permission type</span></span>                        | <span data-ttu-id="8a75f-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a75f-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8a75f-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a75f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a75f-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a75f-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8a75f-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a75f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a75f-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a75f-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="8a75f-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a75f-120">Application</span></span>                            | <span data-ttu-id="8a75f-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a75f-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="8a75f-122">**Hinweis:** Diese API derzeit erfordert die `Directory.Read.All` Berechtigung oder höher.</span><span class="sxs-lookup"><span data-stu-id="8a75f-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="8a75f-123">Mithilfe der `User.Read.All` oder `User.ReadWrite.All` Berechtigungen werden ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a75f-123">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="8a75f-124">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="8a75f-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a75f-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a75f-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="8a75f-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a75f-126">Request headers</span></span>

| <span data-ttu-id="8a75f-127">Header</span><span class="sxs-lookup"><span data-stu-id="8a75f-127">Header</span></span>        | <span data-ttu-id="8a75f-128">Wert</span><span class="sxs-lookup"><span data-stu-id="8a75f-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="8a75f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a75f-129">Authorization</span></span> | <span data-ttu-id="8a75f-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a75f-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a75f-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a75f-132">Content-Type</span></span>  | <span data-ttu-id="8a75f-133">application/json</span><span class="sxs-lookup"><span data-stu-id="8a75f-133">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="8a75f-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a75f-134">Request body</span></span>

<span data-ttu-id="8a75f-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8a75f-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8a75f-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="8a75f-136">Parameter</span></span> | <span data-ttu-id="8a75f-137">Typ</span><span class="sxs-lookup"><span data-stu-id="8a75f-137">Type</span></span>              | <span data-ttu-id="8a75f-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a75f-138">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="8a75f-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="8a75f-139">groupIds</span></span>  | <span data-ttu-id="8a75f-140">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="8a75f-140">String collection</span></span> | <span data-ttu-id="8a75f-141">Ein Array von Gruppen-IDs</span><span class="sxs-lookup"><span data-stu-id="8a75f-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="8a75f-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a75f-142">Response</span></span>

<span data-ttu-id="8a75f-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a75f-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a75f-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a75f-144">Example</span></span>

<span data-ttu-id="8a75f-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8a75f-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8a75f-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a75f-146">Request</span></span>

<span data-ttu-id="8a75f-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a75f-147">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="8a75f-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a75f-148">Response</span></span>

<span data-ttu-id="8a75f-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a75f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
