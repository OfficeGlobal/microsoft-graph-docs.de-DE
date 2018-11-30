---
title: 'group: checkMemberGroups'
description: Überprüfen Sie die Mitgliedschaft in der angegebenen Liste von Gruppen. Diese Gruppen, denen zurückgegeben aus der Liste
ms.openlocfilehash: d0dc617300e29950e820dd94701173829fa6bb7b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017966"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="9f4d0-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="9f4d0-104">group: checkMemberGroups</span></span>

<span data-ttu-id="9f4d0-p102">Sucht nach einer Mitgliedschaft in der angegebenen Liste von Gruppen. Gibt aus der Liste diejenigen Gruppen zurück, bei denen die angegebene Gruppe über eine direkte oder transitive Mitgliedschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="9f4d0-p103">Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f4d0-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f4d0-111">Permissions</span></span>

<span data-ttu-id="9f4d0-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f4d0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f4d0-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f4d0-114">Permission type</span></span>                        | <span data-ttu-id="9f4d0-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f4d0-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="9f4d0-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f4d0-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f4d0-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f4d0-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="9f4d0-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f4d0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f4d0-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f4d0-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="9f4d0-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f4d0-120">Application</span></span>                            | <span data-ttu-id="9f4d0-121">_Group.Read.All_, Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-121">_Group.Read.All_, Directory.Read.All.</span></span> <span data-ttu-id="9f4d0-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f4d0-122">Directory.ReadWrite.All</span></span>                               |

> <span data-ttu-id="9f4d0-123">**Hinweis:** Diese API derzeit erfordert die `Directory.Read.All` Berechtigung oder höher.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-123">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="9f4d0-124">Mithilfe der `Group.Read.All` Berechtigung gibt einen Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-124">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="9f4d0-125">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-125">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f4d0-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f4d0-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="9f4d0-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f4d0-127">Request headers</span></span>

| <span data-ttu-id="9f4d0-128">Name</span><span class="sxs-lookup"><span data-stu-id="9f4d0-128">Name</span></span>          | <span data-ttu-id="9f4d0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9f4d0-129">Type</span></span>   | <span data-ttu-id="9f4d0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f4d0-130">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="9f4d0-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f4d0-131">Authorization</span></span> | <span data-ttu-id="9f4d0-132">string</span><span class="sxs-lookup"><span data-stu-id="9f4d0-132">string</span></span> | <span data-ttu-id="9f4d0-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f4d0-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f4d0-135">Request body</span></span>

<span data-ttu-id="9f4d0-136">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9f4d0-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="9f4d0-137">Parameter</span></span> | <span data-ttu-id="9f4d0-138">Typ</span><span class="sxs-lookup"><span data-stu-id="9f4d0-138">Type</span></span>              | <span data-ttu-id="9f4d0-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f4d0-139">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="9f4d0-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="9f4d0-140">groupIds</span></span>  | <span data-ttu-id="9f4d0-141">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="9f4d0-141">String collection</span></span> | <span data-ttu-id="9f4d0-142">Ein Array von Gruppen-IDs</span><span class="sxs-lookup"><span data-stu-id="9f4d0-142">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="9f4d0-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f4d0-143">Response</span></span>

<span data-ttu-id="9f4d0-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f4d0-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f4d0-145">Example</span></span>

<span data-ttu-id="9f4d0-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9f4d0-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f4d0-147">Request</span></span>

<span data-ttu-id="9f4d0-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-148">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="9f4d0-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f4d0-149">Response</span></span>

<span data-ttu-id="9f4d0-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f4d0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
