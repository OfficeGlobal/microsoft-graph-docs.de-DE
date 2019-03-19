---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Senden einer Einladung für den Zugriff auf ein Element
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1e02af913702aace46a5e3ca2f2e2650a2c7839e
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676975"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="fc914-102">Freigabeeinladung senden</span><span class="sxs-lookup"><span data-stu-id="fc914-102">Send a sharing invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc914-p101">Sendet eine Freigabeeinladung für ein **DriveItem**-Element. Eine Freigabeeinladung stellt Berechtigungen für Empfänger bereit und sendet optional eine E-Mail-Nachricht an den Empfänger, um diesen über die Freigabe in Kenntnis zu setzen.</span><span class="sxs-lookup"><span data-stu-id="fc914-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc914-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fc914-105">Permissions</span></span>

<span data-ttu-id="fc914-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc914-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc914-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc914-108">Permission type</span></span>      | <span data-ttu-id="fc914-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc914-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc914-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc914-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc914-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc914-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fc914-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc914-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc914-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc914-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fc914-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc914-114">Application</span></span> | <span data-ttu-id="fc914-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc914-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc914-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc914-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="fc914-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc914-117">Request body</span></span>

<span data-ttu-id="fc914-118">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="fc914-118">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

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

| <span data-ttu-id="fc914-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="fc914-119">Parameter</span></span>        | <span data-ttu-id="fc914-120">Typ</span><span class="sxs-lookup"><span data-stu-id="fc914-120">Type</span></span>                                            | <span data-ttu-id="fc914-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc914-121">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fc914-122">recipients</span><span class="sxs-lookup"><span data-stu-id="fc914-122">recipients</span></span>       | <span data-ttu-id="fc914-123">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="fc914-123">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="fc914-124">Eine Sammlung der Empfänger, die Zugriff und die Freigabeeinladung erhalten.</span><span class="sxs-lookup"><span data-stu-id="fc914-124">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="fc914-125">message</span><span class="sxs-lookup"><span data-stu-id="fc914-125">message</span></span>          | <span data-ttu-id="fc914-126">String</span><span class="sxs-lookup"><span data-stu-id="fc914-126">String</span></span>                                          | <span data-ttu-id="fc914-p103">Eine formatierte Nur-Text-Nachricht, die in der Freigabeeinladung enthalten ist. Die maximale Länge beträgt 2000 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="fc914-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="fc914-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="fc914-129">requireSignIn</span></span>    | <span data-ttu-id="fc914-130">Boolesch</span><span class="sxs-lookup"><span data-stu-id="fc914-130">Boolean</span></span>                                         | <span data-ttu-id="fc914-131">Gibt an, ob der Empfänger der Einladung sich anmelden muss, um auf das freigegebene Element zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="fc914-131">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="fc914-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="fc914-132">sendInvitation</span></span>   | <span data-ttu-id="fc914-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc914-133">Boolean</span></span>                                         | <span data-ttu-id="fc914-134">Gibt an, ob eine E-Mail oder ein Beitrag generiert (falsch) oder ob nur die Berechtigung erstellt (true) wurde.</span><span class="sxs-lookup"><span data-stu-id="fc914-134">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="fc914-135">roles</span><span class="sxs-lookup"><span data-stu-id="fc914-135">roles</span></span>            | <span data-ttu-id="fc914-136">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="fc914-136">Collection(String)</span></span>                              | <span data-ttu-id="fc914-137">Gibt die Rollen an, die den Empfängern der Freigabeeinladung erteilt werden.</span><span class="sxs-lookup"><span data-stu-id="fc914-137">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="fc914-138">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fc914-138">expirationDateTime</span></span> | <span data-ttu-id="fc914-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc914-139">DateTimeOffset</span></span>                       | <span data-ttu-id="fc914-140">Geben Sie den DateTime-Datentyp an, nach dem die Berechtigung abläuft.</span><span class="sxs-lookup"><span data-stu-id="fc914-140">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="fc914-141">Verfügbar unter OneDrive for Business-, SharePoint-und Premium-persönlichen OneDrive-Konten.</span><span class="sxs-lookup"><span data-stu-id="fc914-141">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="fc914-142">password</span><span class="sxs-lookup"><span data-stu-id="fc914-142">password</span></span>           | <span data-ttu-id="fc914-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc914-143">String</span></span>                         | <span data-ttu-id="fc914-144">Das auf der Einladung vom Ersteller festgelegte Kennwort.</span><span class="sxs-lookup"><span data-stu-id="fc914-144">The password set on the invite by the creator.</span></span> <span data-ttu-id="fc914-145">Nur optional und OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="fc914-145">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="fc914-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc914-146">Example</span></span>

<span data-ttu-id="fc914-147">In diesem Beispiel wird eine Einladung zur Freigabe an einen Benutzer mit der E-Mail-Adresse "ryan@contoso.org" versandt, in der dieser über eine Datei für die Zusammenarbeit benachrichtigt wird.</span><span class="sxs-lookup"><span data-stu-id="fc914-147">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="fc914-148">Die Einladung gewährt Ryan Lese-/ Schreibzugriff auf die Datei.</span><span class="sxs-lookup"><span data-stu-id="fc914-148">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="fc914-149">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc914-149">HTTP request</span></span>

<span data-ttu-id="fc914-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [permission](../resources/permission.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc914-150">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```

### <a name="response"></a><span data-ttu-id="fc914-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc914-151">Response</span></span>

<span data-ttu-id="fc914-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fc914-152">Here is an example of the response.</span></span>

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
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="partial-success-response"></a><span data-ttu-id="fc914-153">Partielle Erfolgsantwort</span><span class="sxs-lookup"><span data-stu-id="fc914-153">Partial success response</span></span>

<span data-ttu-id="fc914-154">Bei der Einladung mehrerer Empfänger ist es möglich, dass die Benachrichtigung für einige erfolgreich ist und für andere Benutzer fehlschlägt.</span><span class="sxs-lookup"><span data-stu-id="fc914-154">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="fc914-155">In diesem Fall gibt der Dienst eine teilweisen Erfolgsantwort mit einem HTTP-Statuscode von 207 zurück.</span><span class="sxs-lookup"><span data-stu-id="fc914-155">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="fc914-156">Wenn ein teilweiser Erfolg zurückgegeben wird, enthält die Antwort für jeden Fehler `error` haften Empfänger ein Objekt mit Informationen darüber, was schief gelaufen ist und wie es behoben werden kann.</span><span class="sxs-lookup"><span data-stu-id="fc914-156">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="fc914-157">Hier ist ein Beispiel für die partielle Antwort.</span><span class="sxs-lookup"><span data-stu-id="fc914-157">Here is an example of the partial response.</span></span>  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "John Adams",
          "id": "5D8CA5D0-FFF8-4A97-B0A6-8F5AEA339681"
        }
      },
      "id": "1EFG7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "adams@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "error": {
        "code":"notAllowed",
        "message":"Account verification needed to unblock sending emails.",
        "localizedMessage": "Kontobestätigung erforderlich, um das Senden von E-Mails zu entsperren.",
        "fixItUrl":"http://g.live.com/8SESkydrive/VerifyAccount",
        "innererror":{  
          "code":"accountVerificationRequired" 
        }
      }
    },
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
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="sendnotification-errors"></a><span data-ttu-id="fc914-158">SendNotification-Fehler</span><span class="sxs-lookup"><span data-stu-id="fc914-158">SendNotification errors</span></span>
<span data-ttu-id="fc914-159">Im folgenden finden Sie einige zusätzliche Fehler, die Ihre APP in den geschachtelten `innererror` Objekten auftreten kann, wenn beim Senden der Benachrichtigung ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="fc914-159">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="fc914-160">Apps müssen diese nicht verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="fc914-160">Apps are not required to handle these.</span></span>

| <span data-ttu-id="fc914-161">Code</span><span class="sxs-lookup"><span data-stu-id="fc914-161">Code</span></span>                           | <span data-ttu-id="fc914-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc914-162">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="fc914-163">accountVerificationRequired</span><span class="sxs-lookup"><span data-stu-id="fc914-163">accountVerificationRequired</span></span>    | <span data-ttu-id="fc914-164">Die Kontoüberprüfung ist erforderlich, um das Senden von Benachrichtigungen aufzuheben.</span><span class="sxs-lookup"><span data-stu-id="fc914-164">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="fc914-165">hipCheckRequired</span><span class="sxs-lookup"><span data-stu-id="fc914-165">hipCheckRequired</span></span>               | <span data-ttu-id="fc914-166">Sie müssen die HIP (Host Intrusion Prevention)-Überprüfung lösen, um das Senden von Benachrichtigungen aufzuheben.</span><span class="sxs-lookup"><span data-stu-id="fc914-166">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="fc914-167">exchangeInvalidUser</span><span class="sxs-lookup"><span data-stu-id="fc914-167">exchangeInvalidUser</span></span>            | <span data-ttu-id="fc914-168">Das Postfach des aktuellen Benutzers wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="fc914-168">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="fc914-169">exchangeOutOfMailboxQuota</span><span class="sxs-lookup"><span data-stu-id="fc914-169">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="fc914-170">Außerhalb des Kontingents.</span><span class="sxs-lookup"><span data-stu-id="fc914-170">Out of quota.</span></span>
| <span data-ttu-id="fc914-171">exchangeMaxRecipients</span><span class="sxs-lookup"><span data-stu-id="fc914-171">exchangeMaxRecipients</span></span>          | <span data-ttu-id="fc914-172">Die maximale Anzahl von Empfängern, die gleichzeitig gesendet werden können, wurde überschritten.</span><span class="sxs-lookup"><span data-stu-id="fc914-172">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="fc914-173">**Hinweis:** Der Dienst kann neue Fehlercodes hinzufügen oder die Rückgabe von alten Dateien jederzeit beenden.</span><span class="sxs-lookup"><span data-stu-id="fc914-173">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="fc914-174">Hinweise</span><span class="sxs-lookup"><span data-stu-id="fc914-174">Remarks</span></span>

* <span data-ttu-id="fc914-175">[Laufwerke](../resources/drive.md) mit dem**driveType**`personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="fc914-175">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="fc914-176">Eine Liste der verfügbaren Rollen finden Sie unter [Rollenaufzählung](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="fc914-176">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="fc914-177">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="fc914-177">Error responses</span></span>

<span data-ttu-id="fc914-178">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="fc914-178">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-invite.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
