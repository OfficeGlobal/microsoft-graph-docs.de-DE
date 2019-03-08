---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Senden einer Einladung für den Zugriff auf ein Element
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f7d3a974143b738b966a8953848f4837c16cd6c8
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480740"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="aa9de-102">Freigabeeinladung senden</span><span class="sxs-lookup"><span data-stu-id="aa9de-102">Send a sharing invitation</span></span>

<span data-ttu-id="aa9de-103">Sendet eine Freigabeeinladung für ein **DriveItem**-Element.</span><span class="sxs-lookup"><span data-stu-id="aa9de-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="aa9de-104">Eine Freigabeeinladung stellt den Empfängern Berechtigungen zur Verfügung und sendet optional eine e-Mail mit einem [Freigabe Link][].</span><span class="sxs-lookup"><span data-stu-id="aa9de-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="aa9de-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa9de-105">Permissions</span></span>

<span data-ttu-id="aa9de-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa9de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa9de-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa9de-108">Permission type</span></span>      | <span data-ttu-id="aa9de-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa9de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa9de-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa9de-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa9de-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa9de-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="aa9de-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa9de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa9de-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa9de-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="aa9de-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa9de-114">Application</span></span> | <span data-ttu-id="aa9de-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa9de-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa9de-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa9de-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="aa9de-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa9de-117">Request body</span></span>

<span data-ttu-id="aa9de-118">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="aa9de-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="aa9de-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="aa9de-119">Parameter</span></span>        | <span data-ttu-id="aa9de-120">Typ</span><span class="sxs-lookup"><span data-stu-id="aa9de-120">Type</span></span>                           | <span data-ttu-id="aa9de-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa9de-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="aa9de-122">recipients</span><span class="sxs-lookup"><span data-stu-id="aa9de-122">recipients</span></span>       | <span data-ttu-id="aa9de-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="aa9de-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="aa9de-124">Eine Sammlung der Empfänger, die Zugriff und die Freigabeeinladung erhalten.</span><span class="sxs-lookup"><span data-stu-id="aa9de-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="aa9de-125">message</span><span class="sxs-lookup"><span data-stu-id="aa9de-125">message</span></span>          | <span data-ttu-id="aa9de-126">String</span><span class="sxs-lookup"><span data-stu-id="aa9de-126">String</span></span>                         | <span data-ttu-id="aa9de-p103">Eine formatierte Nur-Text-Nachricht, die in der Freigabeeinladung enthalten ist. Die maximale Länge beträgt 2000 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="aa9de-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="aa9de-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="aa9de-129">requireSignIn</span></span>    | <span data-ttu-id="aa9de-130">Boolesch</span><span class="sxs-lookup"><span data-stu-id="aa9de-130">Boolean</span></span>                        | <span data-ttu-id="aa9de-131">Gibt an, ob sich der Empfänger der Einladung anmelden muss, um das freigegebene Element anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="aa9de-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="aa9de-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="aa9de-132">sendInvitation</span></span>   | <span data-ttu-id="aa9de-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa9de-133">Boolean</span></span>                        | <span data-ttu-id="aa9de-134">Wenn true, wird ein [Freigabe Link][] an den Empfänger gesendet.</span><span class="sxs-lookup"><span data-stu-id="aa9de-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="aa9de-135">Andernfalls wird eine Berechtigung direkt erteilt, ohne eine Benachrichtigung zu senden.</span><span class="sxs-lookup"><span data-stu-id="aa9de-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="aa9de-136">roles</span><span class="sxs-lookup"><span data-stu-id="aa9de-136">roles</span></span>            | <span data-ttu-id="aa9de-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="aa9de-137">Collection(String)</span></span>             | <span data-ttu-id="aa9de-138">Geben Sie die Rollen an, die den Empfängern der Freigabeeinladung erteilt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="aa9de-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="aa9de-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa9de-139">Example</span></span>

<span data-ttu-id="aa9de-140">In diesem Beispiel wird eine Freigabeeinladung an einen Benutzer mit der e-Mail-Adresse "ryan@contoso.com" mit einer Nachricht zu einer Datei gesendet, an der zusammengearbeitet wird.</span><span class="sxs-lookup"><span data-stu-id="aa9de-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="aa9de-141">Die Einladung gewährt Ryan Lese-/ Schreibzugriff auf die Datei.</span><span class="sxs-lookup"><span data-stu-id="aa9de-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="aa9de-142">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa9de-142">HTTP Request</span></span>

<span data-ttu-id="aa9de-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [permission](../resources/permission.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa9de-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="aa9de-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa9de-144">Response</span></span>

<span data-ttu-id="aa9de-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa9de-145">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="aa9de-146">Hinweise</span><span class="sxs-lookup"><span data-stu-id="aa9de-146">Remarks</span></span>

* <span data-ttu-id="aa9de-147">[Laufwerke](../resources/drive.md) mit dem**driveType**`personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="aa9de-147">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="aa9de-148">Eine Liste der verfügbaren Rollen finden Sie unter [Rollenaufzählung](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="aa9de-148">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="aa9de-149">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="aa9de-149">Error Responses</span></span>

<span data-ttu-id="aa9de-150">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="aa9de-150">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[Freigabe Link]: ../resources/permission.md#sharing-links
[sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
