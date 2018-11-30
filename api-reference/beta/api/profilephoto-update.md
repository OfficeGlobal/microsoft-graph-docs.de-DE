---
title: profilephoto aktualisieren
description: Aktualisieren Sie das Foto für jeden Benutzer in den Mandanten, einschließlich der angemeldeten Benutzer oder der angegebenen Gruppe oder des Kontakts. Seit dort
ms.openlocfilehash: 801ccd58e57cb02c1805f927dc22c9fd593cbae5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062866"
---
# <a name="update-profilephoto"></a><span data-ttu-id="e3df8-104">profilephoto aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e3df8-104">Update profilephoto</span></span>

> <span data-ttu-id="e3df8-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e3df8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3df8-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3df8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3df8-p103">Aktualisieren Sie das Foto für einen beliebigen Benutzer im Mandanten, einschließlich des angemeldeten Benutzers, der angegebenen Gruppe oder des angegebenen Kontakts. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe des Fotos, das Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="e3df8-p103">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="e3df8-109">Verwenden Sie für diesen Vorgang nur PUT in der Betaversion.</span><span class="sxs-lookup"><span data-stu-id="e3df8-109">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="e3df8-110">**Hinweis** Dieser Vorgang des Aktualisierens eines Fotos in der Betaversion unterstützt nur Geschäfts- oder Schulpostfächer eines Benutzers, keine persönlichen Postfächer.</span><span class="sxs-lookup"><span data-stu-id="e3df8-110">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3df8-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3df8-111">Permissions</span></span>
<span data-ttu-id="e3df8-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3df8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3df8-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3df8-114">Permission type</span></span>      | <span data-ttu-id="e3df8-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3df8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3df8-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3df8-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3df8-117">Profilfoto des angemeldeten **Benutzers**:</span><span class="sxs-lookup"><span data-stu-id="e3df8-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="e3df8-118">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3df8-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e3df8-119">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="e3df8-119">For **group** resource:</span></span><br /><span data-ttu-id="e3df8-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3df8-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e3df8-121">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="e3df8-121">For **contact** resource:</span></span><br /><span data-ttu-id="e3df8-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3df8-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="e3df8-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3df8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3df8-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3df8-124">Not supported.</span></span> |
|<span data-ttu-id="e3df8-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3df8-125">Application</span></span>                            | <span data-ttu-id="e3df8-126">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="e3df8-126">For **user** resource:</span></span><br/><span data-ttu-id="e3df8-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3df8-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e3df8-128">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="e3df8-128">For **group** resource:</span></span><br /><span data-ttu-id="e3df8-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3df8-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e3df8-130">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="e3df8-130">For **contact** resource:</span></span><br /><span data-ttu-id="e3df8-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3df8-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="e3df8-p105">**Hinweis** Um das Foto eines Benutzers in der Organisation zu aktualisieren, muss Ihre App über die User.ReadWrite.All-Anwendungsberechtigung verfügen und diese API unter ihrer eigenen Identität und nicht im Auftrag eines Benutzers aufrufen. Weitere Informationen hierzu finden Sie unter [Zugriff ohne einen angemeldeten Benutzer erlangen](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="e3df8-p105">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="e3df8-134">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3df8-134">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="e3df8-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3df8-135">Request headers</span></span>
| <span data-ttu-id="e3df8-136">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e3df8-136">Header</span></span>       | <span data-ttu-id="e3df8-137">Wert</span><span class="sxs-lookup"><span data-stu-id="e3df8-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3df8-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3df8-138">Authorization</span></span>  | <span data-ttu-id="e3df8-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3df8-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e3df8-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3df8-141">Content-Type</span></span>  | <span data-ttu-id="e3df8-p107">image/jpeg. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3df8-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3df8-144">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3df8-144">Request body</span></span>
<span data-ttu-id="e3df8-145">Fügen Sie in den Anforderungstext die Binärdaten des Fotos ein.</span><span class="sxs-lookup"><span data-stu-id="e3df8-145">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="e3df8-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3df8-146">Response</span></span>

<span data-ttu-id="e3df8-147">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3df8-147">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="e3df8-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3df8-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3df8-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3df8-149">Request</span></span>
<span data-ttu-id="e3df8-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3df8-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="e3df8-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3df8-151">Response</span></span>
<span data-ttu-id="e3df8-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3df8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
