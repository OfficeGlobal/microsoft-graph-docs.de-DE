---
title: 'group: checkMemberGroups'
description: Überprüfen Sie die Mitgliedschaft in der angegebenen Liste von Gruppen. Diese Gruppen, denen zurückgegeben aus der Liste
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 2d7755e495eafb93ced334eb4148f7bd29baf1ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966160"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="1b7f1-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="1b7f1-104">group: checkMemberGroups</span></span>

> <span data-ttu-id="1b7f1-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b7f1-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b7f1-p103">Sucht nach einer Mitgliedschaft in der angegebenen Liste von Gruppen. Gibt aus der Liste diejenigen Gruppen zurück, bei denen die angegebene Gruppe über eine direkte oder transitive Mitgliedschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-p103">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="1b7f1-p104">Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-p104">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b7f1-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1b7f1-113">Permissions</span></span>

<span data-ttu-id="1b7f1-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b7f1-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b7f1-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b7f1-116">Permission type</span></span>                        | <span data-ttu-id="1b7f1-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b7f1-117">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="1b7f1-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b7f1-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b7f1-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b7f1-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1b7f1-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b7f1-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b7f1-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b7f1-121">Not supported.</span></span>                                                                              |
| <span data-ttu-id="1b7f1-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b7f1-122">Application</span></span>                            | <span data-ttu-id="1b7f1-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b7f1-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="1b7f1-124">**Hinweis:** Diese API derzeit erfordert die `Directory.Read.All` Berechtigung oder höher.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="1b7f1-125">Mithilfe der `Group.Read.All` Berechtigung gibt einen Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-125">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="1b7f1-126">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="1b7f1-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b7f1-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="1b7f1-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b7f1-128">Request headers</span></span>

| <span data-ttu-id="1b7f1-129">Name</span><span class="sxs-lookup"><span data-stu-id="1b7f1-129">Name</span></span>          | <span data-ttu-id="1b7f1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1b7f1-130">Type</span></span>   | <span data-ttu-id="1b7f1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b7f1-131">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="1b7f1-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b7f1-132">Authorization</span></span> | <span data-ttu-id="1b7f1-133">string</span><span class="sxs-lookup"><span data-stu-id="1b7f1-133">string</span></span> | <span data-ttu-id="1b7f1-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b7f1-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b7f1-136">Request body</span></span>

<span data-ttu-id="1b7f1-137">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1b7f1-138">Parameter</span><span class="sxs-lookup"><span data-stu-id="1b7f1-138">Parameter</span></span> | <span data-ttu-id="1b7f1-139">Typ</span><span class="sxs-lookup"><span data-stu-id="1b7f1-139">Type</span></span>   | <span data-ttu-id="1b7f1-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b7f1-140">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="1b7f1-141">groupIds</span><span class="sxs-lookup"><span data-stu-id="1b7f1-141">groupIds</span></span>  | <span data-ttu-id="1b7f1-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b7f1-142">String</span></span> | <span data-ttu-id="1b7f1-143">Ein Array von Gruppen-IDs</span><span class="sxs-lookup"><span data-stu-id="1b7f1-143">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="1b7f1-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b7f1-144">Response</span></span>

<span data-ttu-id="1b7f1-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b7f1-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b7f1-146">Example</span></span>

<span data-ttu-id="1b7f1-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1b7f1-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b7f1-148">Request</span></span>

<span data-ttu-id="1b7f1-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="1b7f1-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b7f1-150">Response</span></span>

<span data-ttu-id="1b7f1-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b7f1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
