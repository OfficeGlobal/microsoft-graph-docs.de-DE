---
title: Einladung erstellen
description: Verwenden Sie diese API zum Erstellen einer neuen Einladung. „Invitation“ fügt einen externen Benutzer zur Organisation hinzu.
ms.openlocfilehash: 220b90cafdd7825dbb6dff9bb8635a51de2ee267
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065452"
---
# <a name="create-invitation"></a><span data-ttu-id="a53b8-104">Einladung erstellen</span><span class="sxs-lookup"><span data-stu-id="a53b8-104">Create invitation</span></span>

> <span data-ttu-id="a53b8-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a53b8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a53b8-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a53b8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a53b8-p103">Verwenden Sie diese API zum Erstellen einer neuen [Einladung](../resources/invitation.md). „Invitation“ fügt einen externen Benutzer zur Organisation hinzu.</span><span class="sxs-lookup"><span data-stu-id="a53b8-p103">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="a53b8-109">Wenn Sie eine neue Einladung erstellen, stehen Ihnen mehrere Optionen zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="a53b8-109">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="a53b8-p104">Bei der Erstellung der Einladung, kann Microsoft Graph automatisch eine Einladungs-E-Mail direkt an die eingeladenen Benutzer senden, oder Ihre App kann die in der Erstellungsantwort zurückgegebene *inviteRedeemUrl* verwenden, um eine eigene Einladung (über den gewünschten Kommunikationsmechanismus) an den eingeladenen Benutzer zu erstellen. Wenn Sie sich entscheiden, dass Microsoft Graph automatisch eine Einladungs-E-Mail senden soll, können Sie den Inhalt und die Sprache der E-Mail mithilfe von [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md) steuern.</span><span class="sxs-lookup"><span data-stu-id="a53b8-p104">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="a53b8-p105">Wenn der Benutzer eingeladen wird, wird eine Benutzerentität (userTyp Guest) erstellt, die nun zum Steuern des Zugriffs auf Ressourcen verwendet werden kann. Der eingeladene Benutzer muss den Einlösevorgang durchlaufen, um auf Ressourcen zuzugreifen, zu denen er eingeladen wurde.</span><span class="sxs-lookup"><span data-stu-id="a53b8-p105">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="a53b8-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a53b8-114">Permissions</span></span>
<span data-ttu-id="a53b8-p106">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a53b8-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a53b8-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a53b8-117">Permission type</span></span>      | <span data-ttu-id="a53b8-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a53b8-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a53b8-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a53b8-119">Delegated (work or school account)</span></span> | <span data-ttu-id="a53b8-120">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a53b8-120">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a53b8-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a53b8-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a53b8-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a53b8-122">Not supported.</span></span>    |
|<span data-ttu-id="a53b8-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a53b8-123">Application</span></span> | <span data-ttu-id="a53b8-124">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a53b8-124">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a53b8-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a53b8-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="a53b8-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a53b8-126">Request headers</span></span>
| <span data-ttu-id="a53b8-127">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a53b8-127">Header</span></span>       | <span data-ttu-id="a53b8-128">Wert</span><span class="sxs-lookup"><span data-stu-id="a53b8-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a53b8-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="a53b8-129">Authorization</span></span>  | <span data-ttu-id="a53b8-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a53b8-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a53b8-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a53b8-132">Content-Type</span></span>  | <span data-ttu-id="a53b8-133">application/json</span><span class="sxs-lookup"><span data-stu-id="a53b8-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a53b8-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a53b8-134">Request body</span></span>
<span data-ttu-id="a53b8-135">Geben Sie im Anforderungstext eine JSON-Darstellung eines [invitation](../resources/invitation.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a53b8-135">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="a53b8-136">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen einer Einladung erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a53b8-136">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="a53b8-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="a53b8-137">Parameter</span></span> | <span data-ttu-id="a53b8-138">Typ</span><span class="sxs-lookup"><span data-stu-id="a53b8-138">Type</span></span> | <span data-ttu-id="a53b8-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a53b8-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a53b8-140">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a53b8-140">invitedUserEmailAddress</span></span> |<span data-ttu-id="a53b8-141">string</span><span class="sxs-lookup"><span data-stu-id="a53b8-141">string</span></span> | <span data-ttu-id="a53b8-142">Die E-Mail-Adresse des Benutzers, den Sie einladen.</span><span class="sxs-lookup"><span data-stu-id="a53b8-142">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="a53b8-143">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="a53b8-143">inviteRedirectUrl</span></span> |<span data-ttu-id="a53b8-144">string</span><span class="sxs-lookup"><span data-stu-id="a53b8-144">string</span></span> |<span data-ttu-id="a53b8-145">Die URL, zu der der Benutzer nach der Einlösung umgeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="a53b8-145">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="a53b8-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="a53b8-146">Response</span></span>

<span data-ttu-id="a53b8-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [invitation](../resources/invitation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a53b8-147">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a53b8-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a53b8-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a53b8-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a53b8-149">Request</span></span>
<span data-ttu-id="a53b8-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a53b8-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/beta/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.com"
}
```

##### <a name="response"></a><span data-ttu-id="a53b8-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="a53b8-151">Response</span></span>
<span data-ttu-id="a53b8-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a53b8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitations"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 551

{
  "id": "7b92124c-9fa9-406f-8b8e-225df8376ba9",
  "inviteRedeemUrl": "https://invitations.microsoft.com/redeem/?tenant=04dcc6ab-388a-4559-b527-fbec656300ea&user=7b92124c-9fa9-406f-8b8e-225df8376ba9&ticket=VV9dmiExBsfRIVNFjb9ITj9VXAd07Ypv4gTg%2f8PiuJs%3d&lc=1033&ver=2.0",
  "invitedUserDisplayName": "yyy",
  "invitedUserEmailAddress": "yyy@test.com",
  "sendInvitationMessage": false,
  "invitedUserMessageInfo": {
     "messageLanguage": null,
     "ccRecipients": [
          {
             "emailAddress": {
                 "name": null,
                 "address": null
              }
          }
     ],
     "customizedMessageBody": null
  },
  "inviteRedirectUrl": "https://myapp.com/",
  "status": "Completed",
  "invitedUser":  [ {  "id": "243b1de4-ad9f-421c-a933-d55305fb165d" } ]
}
```
