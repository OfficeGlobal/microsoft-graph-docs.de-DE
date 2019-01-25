---
title: profilephoto aktualisieren
description: Aktualisieren Sie das Foto für jeden Benutzer in den Mandanten, einschließlich der angemeldeten Benutzer oder der angegebenen Gruppe oder des Kontakts. Seit dort
localization_priority: Normal
ms.openlocfilehash: f8191716471cba565b27ef316b5b13e3b32ecaff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521131"
---
# <a name="update-profilephoto"></a><span data-ttu-id="3da06-104">profilephoto aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3da06-104">Update profilephoto</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3da06-p102">Aktualisieren Sie das Foto für einen beliebigen Benutzer im Mandanten, einschließlich des angemeldeten Benutzers, der angegebenen Gruppe oder des angegebenen Kontakts. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe des Fotos, das Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="3da06-p102">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="3da06-107">Verwenden Sie für diesen Vorgang nur PUT in der Betaversion.</span><span class="sxs-lookup"><span data-stu-id="3da06-107">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="3da06-108">Hinweis Dieser Vorgang des Aktualisierens eines Fotos in der Betaversion unterstützt nur Geschäfts- oder Schulpostfächer eines Benutzers, keine persönlichen Postfächer.</span><span class="sxs-lookup"><span data-stu-id="3da06-108">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="3da06-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3da06-109">Permissions</span></span>
<span data-ttu-id="3da06-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3da06-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3da06-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3da06-112">Permission type</span></span>      | <span data-ttu-id="3da06-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3da06-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3da06-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3da06-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3da06-115">Profilfoto des angemeldeten **Benutzers**:</span><span class="sxs-lookup"><span data-stu-id="3da06-115">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="3da06-116">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da06-116">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="3da06-117">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="3da06-117">For **group** resource:</span></span><br /><span data-ttu-id="3da06-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da06-118">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="3da06-119">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="3da06-119">For **contact** resource:</span></span><br /><span data-ttu-id="3da06-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3da06-120">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="3da06-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3da06-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3da06-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3da06-122">Not supported.</span></span> |
|<span data-ttu-id="3da06-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3da06-123">Application</span></span>                            | <span data-ttu-id="3da06-124">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="3da06-124">For **user** resource:</span></span><br/><span data-ttu-id="3da06-125">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da06-125">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="3da06-126">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="3da06-126">For **group** resource:</span></span><br /><span data-ttu-id="3da06-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da06-127">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="3da06-128">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="3da06-128">For **contact** resource:</span></span><br /><span data-ttu-id="3da06-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3da06-129">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="3da06-p104">**Hinweis** Um das Foto eines Benutzers in der Organisation zu aktualisieren, muss Ihre App über die User.ReadWrite.All-Anwendungsberechtigung verfügen und diese API unter ihrer eigenen Identität und nicht im Auftrag eines Benutzers aufrufen. Weitere Informationen hierzu finden Sie unter [Zugriff ohne einen angemeldeten Benutzer erlangen](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="3da06-p104">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="3da06-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3da06-132">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="3da06-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3da06-133">Request headers</span></span>
| <span data-ttu-id="3da06-134">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3da06-134">Header</span></span>       | <span data-ttu-id="3da06-135">Wert</span><span class="sxs-lookup"><span data-stu-id="3da06-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3da06-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="3da06-136">Authorization</span></span>  | <span data-ttu-id="3da06-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3da06-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3da06-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3da06-139">Content-Type</span></span>  | <span data-ttu-id="3da06-p106">image/jpeg. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3da06-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3da06-142">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3da06-142">Request body</span></span>
<span data-ttu-id="3da06-143">Fügen Sie in den Anforderungstext die Binärdaten des Fotos ein.</span><span class="sxs-lookup"><span data-stu-id="3da06-143">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="3da06-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="3da06-144">Response</span></span>

<span data-ttu-id="3da06-145">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3da06-145">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="3da06-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3da06-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3da06-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3da06-147">Request</span></span>
<span data-ttu-id="3da06-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3da06-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="3da06-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="3da06-149">Response</span></span>
<span data-ttu-id="3da06-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3da06-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/profilephoto-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
