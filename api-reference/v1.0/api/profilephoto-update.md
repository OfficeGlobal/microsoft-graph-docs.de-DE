---
title: profilephoto aktualisieren
description: Aktualisieren Sie das Foto für den angemeldeten **Benutzer**, oder der angegebenen **Gruppe** oder **wenden Sie sich an**. Seit dort
localization_priority: Priority
ms.openlocfilehash: 39c5a0405a05d46cbd77f161cd45fb19c40d8b7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871820"
---
# <a name="update-profilephoto"></a><span data-ttu-id="1a82a-104">profilephoto aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1a82a-104">Update profilephoto</span></span>

<span data-ttu-id="1a82a-p102">Aktualisieren Sie das Foto für den angemeldeten **Benutzer**, die angegebene **Gruppe** oder den angegebenen **Kontakt**. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe des Fotos, das Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="1a82a-p102">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="1a82a-107">In Version 1.0 können Sie PATCH oder PUT für diesen Vorgang verwenden.</span><span class="sxs-lookup"><span data-stu-id="1a82a-107">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="1a82a-108">**Hinweis:** Dieser Vorgang in Version 1.0 unterstützt ausschließlich Postfächer in Geschäfts-, Schul- oder Unikonten des Benutzers. Persönliche Postfächer werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a82a-108">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a82a-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1a82a-109">Permissions</span></span>
<span data-ttu-id="1a82a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a82a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

- <span data-ttu-id="1a82a-112">Profilfoto des angemeldeten **Benutzers**: User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a82a-112">Profile photo of the signed-in **user** - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="1a82a-113">Profilfoto einer **Gruppe**: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a82a-113">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="1a82a-114">Foto eines **Kontakts**: Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a82a-114">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="1a82a-p104">**Hinweis** Um das Foto eines Benutzers in der Organisation zu aktualisieren, muss Ihre App über die User.ReadWrite.All-Anwendungsberechtigung verfügen und diese API unter ihrer eigenen Identität und nicht im Auftrag eines Benutzers aufrufen. Weitere Informationen hierzu finden Sie unter [Zugriff ohne einen angemeldeten Benutzer erlangen](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="1a82a-p104">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="1a82a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a82a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="1a82a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a82a-118">Request headers</span></span>
| <span data-ttu-id="1a82a-119">Header</span><span class="sxs-lookup"><span data-stu-id="1a82a-119">Header</span></span>       | <span data-ttu-id="1a82a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1a82a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a82a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a82a-121">Authorization</span></span>  | <span data-ttu-id="1a82a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a82a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1a82a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a82a-124">Content-Type</span></span>  | <span data-ttu-id="1a82a-p106">image/jpeg. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a82a-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a82a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a82a-127">Request body</span></span>
<span data-ttu-id="1a82a-128">Fügen Sie in den Anforderungstext die Binärdaten des Fotos ein.</span><span class="sxs-lookup"><span data-stu-id="1a82a-128">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="1a82a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a82a-129">Response</span></span>

<span data-ttu-id="1a82a-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a82a-130">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="1a82a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a82a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a82a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a82a-132">Request</span></span>
<span data-ttu-id="1a82a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a82a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="1a82a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a82a-134">Response</span></span>
<span data-ttu-id="1a82a-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a82a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
