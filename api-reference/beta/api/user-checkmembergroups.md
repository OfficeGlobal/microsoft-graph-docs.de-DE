---
title: checkMemberGroups
description: Überprüfen Sie die Mitgliedschaft in der angegebenen Liste von Gruppen. Diese Gruppen, denen zurückgegeben aus der Liste
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d7452795cb0a8ffdf3a966a3e350a8634b2a7ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516896"
---
# <a name="checkmembergroups"></a><span data-ttu-id="817b0-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="817b0-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="817b0-p102">Sucht nach einer Mitgliedschaft in einer angegebenenListe von Gruppen. Gibt aus der Liste diesjenigen Gruppen zurück, bei denen der Benutzer über eine direkte oder transitive Mitgliedschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="817b0-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="817b0-p103">Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="817b0-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="817b0-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="817b0-111">Permissions</span></span>

<span data-ttu-id="817b0-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="817b0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="817b0-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="817b0-114">Permission type</span></span>                        | <span data-ttu-id="817b0-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="817b0-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="817b0-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="817b0-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="817b0-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="817b0-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="817b0-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="817b0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="817b0-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="817b0-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="817b0-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="817b0-120">Application</span></span>                            | <span data-ttu-id="817b0-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="817b0-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="817b0-122">**Hinweis:** Diese API erfordert derzeit mindestens die Berechtigung `Directory.Read.All`.</span><span class="sxs-lookup"><span data-stu-id="817b0-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="817b0-123">Mithilfe der `User.Read.All` oder `User.ReadWrite.All` Berechtigungen werden ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="817b0-123">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="817b0-124">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="817b0-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="817b0-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="817b0-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="817b0-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="817b0-126">Request headers</span></span>

| <span data-ttu-id="817b0-127">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="817b0-127">Header</span></span>        | <span data-ttu-id="817b0-128">Wert</span><span class="sxs-lookup"><span data-stu-id="817b0-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="817b0-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="817b0-129">Authorization</span></span> | <span data-ttu-id="817b0-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="817b0-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="817b0-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="817b0-132">Content-Type</span></span>  | <span data-ttu-id="817b0-133">application/json</span><span class="sxs-lookup"><span data-stu-id="817b0-133">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="817b0-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="817b0-134">Request body</span></span>

<span data-ttu-id="817b0-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="817b0-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="817b0-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="817b0-136">Parameter</span></span> | <span data-ttu-id="817b0-137">Typ</span><span class="sxs-lookup"><span data-stu-id="817b0-137">Type</span></span>   | <span data-ttu-id="817b0-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="817b0-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="817b0-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="817b0-139">groupIds</span></span>  | <span data-ttu-id="817b0-140">String</span><span class="sxs-lookup"><span data-stu-id="817b0-140">String</span></span> | <span data-ttu-id="817b0-141">Ein Array von Gruppen-IDs</span><span class="sxs-lookup"><span data-stu-id="817b0-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="817b0-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="817b0-142">Response</span></span>

<span data-ttu-id="817b0-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="817b0-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="817b0-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="817b0-144">Example</span></span>

<span data-ttu-id="817b0-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="817b0-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="817b0-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="817b0-146">Request</span></span>

<span data-ttu-id="817b0-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="817b0-147">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="817b0-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="817b0-148">Response</span></span>

<span data-ttu-id="817b0-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="817b0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
