---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Versenden einer Einladung für den Zugriff auf ein Element
ms.openlocfilehash: c68289049503e70e04b2e403ca09cfc1f67e4096
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268732"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="98b55-102">Freigabeeinladung versenden</span><span class="sxs-lookup"><span data-stu-id="98b55-102">Send a sharing invitation</span></span>

<span data-ttu-id="98b55-103">Sendet eine Einladung zur Freigabe für ein **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="98b55-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="98b55-104">Eine Einladung zur Freigabe stellt Berechtigungen für die Empfänger bereit und sendet ihnen optional eine E-Mail mit einem [Freigabelink][].</span><span class="sxs-lookup"><span data-stu-id="98b55-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="98b55-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="98b55-105">Permissions</span></span>

<span data-ttu-id="98b55-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="98b55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="98b55-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="98b55-108">Permission type</span></span>      | <span data-ttu-id="98b55-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="98b55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98b55-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="98b55-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98b55-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98b55-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="98b55-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="98b55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98b55-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98b55-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="98b55-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="98b55-114">Application</span></span> | <span data-ttu-id="98b55-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98b55-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98b55-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98b55-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="98b55-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="98b55-117">Request body</span></span>

<span data-ttu-id="98b55-118">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="98b55-118">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| <span data-ttu-id="98b55-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="98b55-119">Parameter</span></span>        | <span data-ttu-id="98b55-120">Typ</span><span class="sxs-lookup"><span data-stu-id="98b55-120">Type</span></span>                           | <span data-ttu-id="98b55-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98b55-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="98b55-122">recipients</span><span class="sxs-lookup"><span data-stu-id="98b55-122">recipients</span></span>       | <span data-ttu-id="98b55-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="98b55-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="98b55-124">Eine Sammlung der Empfänger, die Zugriff und die Freigabeeinladung erhalten.</span><span class="sxs-lookup"><span data-stu-id="98b55-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="98b55-125">message</span><span class="sxs-lookup"><span data-stu-id="98b55-125">message</span></span>          | <span data-ttu-id="98b55-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="98b55-126">String</span></span>                         | <span data-ttu-id="98b55-p103">Eine formatierte Nur-Text-Nachricht, die in der Freigabeeinladung enthalten ist. Die maximale Länge beträgt 2000 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="98b55-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="98b55-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="98b55-129">requireSignIn</span></span>    | <span data-ttu-id="98b55-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="98b55-130">Boolean</span></span>                        | <span data-ttu-id="98b55-131">Gibt an, ob der Empfänger der Einladung sich anmelden muss, um auf das freigegebene Element zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="98b55-131">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="98b55-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="98b55-132">sendInvitation</span></span>   | <span data-ttu-id="98b55-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="98b55-133">Boolean</span></span>                        | <span data-ttu-id="98b55-134">Bei true wird ein [Freigabelink][] an den Empfänger gesendet.</span><span class="sxs-lookup"><span data-stu-id="98b55-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="98b55-135">Andernfalls wird direkt eine Berechtigung erteilt, ohne dass eine Benachrichtigung gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="98b55-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="98b55-136">roles</span><span class="sxs-lookup"><span data-stu-id="98b55-136">roles</span></span>            | <span data-ttu-id="98b55-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="98b55-137">Collection(String)</span></span>             | <span data-ttu-id="98b55-138">Gibt die Rollen an, die den Empfängern der Freigabeeinladung erteilt werden.</span><span class="sxs-lookup"><span data-stu-id="98b55-138">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="98b55-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98b55-139">Example</span></span>

<span data-ttu-id="98b55-140">In diesem Beispiel wird eine Einladung zur Freigabe an einen Benutzer mit der E-Mail-Adresse "ryan@contoso.com" versandt, in der dieser über eine Datei für die Zusammenarbeit benachrichtigt wird.</span><span class="sxs-lookup"><span data-stu-id="98b55-140">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="98b55-141">Die Einladung gewährt Ryan Lese-/ Schreibzugriff auf die Datei.</span><span class="sxs-lookup"><span data-stu-id="98b55-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="98b55-142">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98b55-142">HTTP Request</span></span>

<span data-ttu-id="98b55-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [permission](../resources/permission.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98b55-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

### <a name="response"></a><span data-ttu-id="98b55-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="98b55-144">Response</span></span>

<span data-ttu-id="98b55-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="98b55-145">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="98b55-146">Hinweise</span><span class="sxs-lookup"><span data-stu-id="98b55-146">Remarks</span></span>

* <span data-ttu-id="98b55-147">[Laufwerke](../resources/drive.md) mit dem**driveType**`personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="98b55-147">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="98b55-148">Eine Liste der verfügbaren Rollen finden Sie unter [Rollenaufzählung](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="98b55-148">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="98b55-149">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="98b55-149">Error Responses</span></span>

<span data-ttu-id="98b55-150">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="98b55-150">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[DriveRecipient]: ../resources/driverecipient.md
[error-response]: ../../../concepts/errors.md
[sharing link]: ../resources/permission.md#sharing-links
[Create sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
