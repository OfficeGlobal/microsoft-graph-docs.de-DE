---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Versenden einer Einladung für den Zugriff auf ein Element
localization_priority: Normal
ms.openlocfilehash: 93fa30cc3e7999ba00bbcf591876c90253b77a7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823933"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="efbac-102">Freigabeeinladung senden</span><span class="sxs-lookup"><span data-stu-id="efbac-102">Send a sharing invitation</span></span>

> <span data-ttu-id="efbac-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="efbac-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efbac-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="efbac-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="efbac-p102">Sendet eine Freigabeeinladung für ein **DriveItem**-Element. Eine Freigabeeinladung stellt Berechtigungen für Empfänger bereit und sendet optional eine E-Mail-Nachricht an den Empfänger, um diesen über die Freigabe in Kenntnis zu setzen.</span><span class="sxs-lookup"><span data-stu-id="efbac-p102">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="efbac-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="efbac-107">Permissions</span></span>

<span data-ttu-id="efbac-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efbac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efbac-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="efbac-110">Permission type</span></span>      | <span data-ttu-id="efbac-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="efbac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efbac-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="efbac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="efbac-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efbac-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="efbac-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="efbac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efbac-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efbac-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="efbac-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="efbac-116">Application</span></span> | <span data-ttu-id="efbac-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efbac-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efbac-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="efbac-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="efbac-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="efbac-119">Request body</span></span>

<span data-ttu-id="efbac-120">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="efbac-120">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="efbac-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="efbac-121">Parameter</span></span>        | <span data-ttu-id="efbac-122">Typ</span><span class="sxs-lookup"><span data-stu-id="efbac-122">Type</span></span>                                            | <span data-ttu-id="efbac-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efbac-123">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="efbac-124">recipients</span><span class="sxs-lookup"><span data-stu-id="efbac-124">recipients</span></span>       | <span data-ttu-id="efbac-125">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="efbac-125">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="efbac-126">Eine Sammlung der Empfänger, die Zugriff und die Freigabeeinladung erhalten.</span><span class="sxs-lookup"><span data-stu-id="efbac-126">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="efbac-127">message</span><span class="sxs-lookup"><span data-stu-id="efbac-127">message</span></span>          | <span data-ttu-id="efbac-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="efbac-128">String</span></span>                                          | <span data-ttu-id="efbac-p104">Eine formatierte Nur-Text-Nachricht, die in der Freigabeeinladung enthalten ist. Die maximale Länge beträgt 2000 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="efbac-p104">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="efbac-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="efbac-131">requireSignIn</span></span>    | <span data-ttu-id="efbac-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="efbac-132">Boolean</span></span>                                         | <span data-ttu-id="efbac-133">Gibt an, ob der Empfänger der Einladung sich anmelden muss, um auf das freigegebene Element zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="efbac-133">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="efbac-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="efbac-134">sendInvitation</span></span>   | <span data-ttu-id="efbac-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="efbac-135">Boolean</span></span>                                         | <span data-ttu-id="efbac-136">Gibt an, ob eine E-Mail oder ein Beitrag generiert (falsch) oder ob nur die Berechtigung erstellt (true) wurde.</span><span class="sxs-lookup"><span data-stu-id="efbac-136">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="efbac-137">roles</span><span class="sxs-lookup"><span data-stu-id="efbac-137">roles</span></span>            | <span data-ttu-id="efbac-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="efbac-138">Collection(String)</span></span>                              | <span data-ttu-id="efbac-139">Gibt die Rollen an, die den Empfängern der Freigabeeinladung erteilt werden.</span><span class="sxs-lookup"><span data-stu-id="efbac-139">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="example"></a><span data-ttu-id="efbac-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="efbac-140">Example</span></span>

<span data-ttu-id="efbac-141">In diesem Beispiel wird eine Einladung zur Freigabe an einen Benutzer mit der E-Mail-Adresse "ryan@contoso.org" versandt, in der dieser über eine Datei für die Zusammenarbeit benachrichtigt wird.</span><span class="sxs-lookup"><span data-stu-id="efbac-141">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="efbac-142">Die Einladung gewährt Ryan Lese-/ Schreibzugriff auf die Datei.</span><span class="sxs-lookup"><span data-stu-id="efbac-142">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="efbac-143">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="efbac-143">HTTP Request</span></span>

<span data-ttu-id="efbac-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [permission](../resources/permission.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="efbac-144">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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
  "roles": [ "write" ]
}
```

### <a name="response"></a><span data-ttu-id="efbac-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="efbac-145">Response</span></span>

<span data-ttu-id="efbac-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="efbac-146">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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

## <a name="remarks"></a><span data-ttu-id="efbac-147">Hinweise</span><span class="sxs-lookup"><span data-stu-id="efbac-147">Remarks</span></span>

* <span data-ttu-id="efbac-148">[Laufwerke](../resources/drive.md) mit dem**driveType**`personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="efbac-148">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="efbac-149">Eine Liste der verfügbaren Rollen finden Sie unter [Rollenaufzählung](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="efbac-149">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="efbac-150">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="efbac-150">Error Responses</span></span>

<span data-ttu-id="efbac-151">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="efbac-151">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
