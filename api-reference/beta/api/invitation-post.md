---
title: Einladung erstellen
description: Verwenden Sie diese API zum Erstellen einer neuen Einladung. „Invitation“ fügt einen externen Benutzer zur Organisation hinzu.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 92bf3929fa4f736be3c6956f20aff6965291a876
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528858"
---
# <a name="create-invitation"></a><span data-ttu-id="159ba-104">Einladung erstellen</span><span class="sxs-lookup"><span data-stu-id="159ba-104">Create invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="159ba-p102">Verwenden Sie diese API zum Erstellen einer neuen [Einladung](../resources/invitation.md). „Invitation“ fügt einen externen Benutzer zur Organisation hinzu.</span><span class="sxs-lookup"><span data-stu-id="159ba-p102">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="159ba-107">Wenn Sie eine neue Einladung erstellen, stehen Ihnen mehrere Optionen zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="159ba-107">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="159ba-p103">Bei der Erstellung der Einladung, kann Microsoft Graph automatisch eine Einladungs-E-Mail direkt an die eingeladenen Benutzer senden, oder Ihre App kann die in der Erstellungsantwort zurückgegebene *inviteRedeemUrl* verwenden, um eine eigene Einladung (über den gewünschten Kommunikationsmechanismus) an den eingeladenen Benutzer zu erstellen. Wenn Sie sich entscheiden, dass Microsoft Graph automatisch eine Einladungs-E-Mail senden soll, können Sie den Inhalt und die Sprache der E-Mail mithilfe von [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md) steuern.</span><span class="sxs-lookup"><span data-stu-id="159ba-p103">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="159ba-p104">Wenn der Benutzer eingeladen wird, wird eine Benutzerentität (userTyp Guest) erstellt, die nun zum Steuern des Zugriffs auf Ressourcen verwendet werden kann. Der eingeladene Benutzer muss den Einlösevorgang durchlaufen, um auf Ressourcen zuzugreifen, zu denen er eingeladen wurde.</span><span class="sxs-lookup"><span data-stu-id="159ba-p104">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="159ba-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="159ba-112">Permissions</span></span>
<span data-ttu-id="159ba-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="159ba-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="159ba-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="159ba-115">Permission type</span></span>      | <span data-ttu-id="159ba-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="159ba-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="159ba-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="159ba-117">Delegated (work or school account)</span></span> | <span data-ttu-id="159ba-118">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="159ba-118">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="159ba-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="159ba-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="159ba-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="159ba-120">Not supported.</span></span>    |
|<span data-ttu-id="159ba-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="159ba-121">Application</span></span> | <span data-ttu-id="159ba-122">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="159ba-122">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="159ba-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="159ba-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="159ba-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="159ba-124">Request headers</span></span>
| <span data-ttu-id="159ba-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="159ba-125">Header</span></span>       | <span data-ttu-id="159ba-126">Wert</span><span class="sxs-lookup"><span data-stu-id="159ba-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="159ba-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="159ba-127">Authorization</span></span>  | <span data-ttu-id="159ba-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="159ba-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="159ba-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="159ba-130">Content-Type</span></span>  | <span data-ttu-id="159ba-131">application/json</span><span class="sxs-lookup"><span data-stu-id="159ba-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="159ba-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="159ba-132">Request body</span></span>
<span data-ttu-id="159ba-133">Geben Sie im Anforderungstext eine JSON-Darstellung eines [invitation](../resources/invitation.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="159ba-133">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="159ba-134">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen einer Einladung erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="159ba-134">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="159ba-135">Parameter</span><span class="sxs-lookup"><span data-stu-id="159ba-135">Parameter</span></span> | <span data-ttu-id="159ba-136">Typ</span><span class="sxs-lookup"><span data-stu-id="159ba-136">Type</span></span> | <span data-ttu-id="159ba-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="159ba-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="159ba-138">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="159ba-138">invitedUserEmailAddress</span></span> |<span data-ttu-id="159ba-139">string</span><span class="sxs-lookup"><span data-stu-id="159ba-139">string</span></span> | <span data-ttu-id="159ba-140">Die E-Mail-Adresse des Benutzers, den Sie einladen.</span><span class="sxs-lookup"><span data-stu-id="159ba-140">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="159ba-141">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="159ba-141">inviteRedirectUrl</span></span> |<span data-ttu-id="159ba-142">string</span><span class="sxs-lookup"><span data-stu-id="159ba-142">string</span></span> |<span data-ttu-id="159ba-143">Die URL, zu der der Benutzer nach der Einlösung umgeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="159ba-143">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="159ba-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="159ba-144">Response</span></span>

<span data-ttu-id="159ba-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [invitation](../resources/invitation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="159ba-145">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="159ba-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="159ba-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="159ba-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="159ba-147">Request</span></span>
<span data-ttu-id="159ba-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="159ba-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="159ba-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="159ba-149">Response</span></span>
<span data-ttu-id="159ba-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="159ba-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/invitation-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
