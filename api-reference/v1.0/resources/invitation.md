---
title: Einladungs-Manager
description: 'Verwenden Sie den Einladungs-Manager, um eine Einladung zum Hinzufügen eines externen Benutzers zu der Organisation zu erstellen. '
localization_priority: Priority
ms.openlocfilehash: 4e47131fd7e3128366d482c314c059d833c8e101
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867438"
---
# <a name="invitation-manager"></a><span data-ttu-id="e686b-103">Einladungs-Manager</span><span class="sxs-lookup"><span data-stu-id="e686b-103">invitation manager</span></span>

<span data-ttu-id="e686b-104">Verwenden Sie den Einladungs-Manager, um eine Einladung zum Hinzufügen eines externen Benutzers zu der Organisation zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="e686b-104">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="e686b-105">Der Einladungsprozess verwendet den folgenden Ablauf:</span><span class="sxs-lookup"><span data-stu-id="e686b-105">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="e686b-106">Eine Einladung wird erstellt.</span><span class="sxs-lookup"><span data-stu-id="e686b-106">An invitation is created</span></span>
* <span data-ttu-id="e686b-107">Eine Einladung (mit einem Einladungs-Link) wird an den eingeladenen Benutzer gesendet.</span><span class="sxs-lookup"><span data-stu-id="e686b-107">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="e686b-108">Der eingeladene Benutzer klickt auf den Einladungs-Link, meldet sich an und löst die Einladung und die Erstellung der Benutzerentität ein, die den eingeladenen Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="e686b-108">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="e686b-109">Der Benutzer wird nach Abschluss der Einlösung zu einer bestimmten Seite umgeleitet.</span><span class="sxs-lookup"><span data-stu-id="e686b-109">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="e686b-p101">Durch Erstellen einer Einladung wird eine URL für die Einlösung in der Antwort zurückgegeben (*InviteRedeemUrl*). Die API zum Erstellen der Einladung kann automatisch eine E-Mail mit der Einlösungs-URL an den eingeladenen Benutzer senden, indem *sendInvitationMessage* auf „true“ festgelegt wird. Sie können die Nachricht, die an den eingeladenen Benutzer gesendet wird, auch anpassen. Wenn Sie die Einlösungs-URL anderweitig versenden möchten, können Sie die *sendInvitationMessage* auf „false“ festlegen und die Einlösungs-URL aus der Antwort verwenden, um Ihre eigene Mitteilung zu erstellen. Derzeit gibt es keine API, die den Einlösungsprozess durchführt. Der eingeladene Benutzer muss auf den Link *inviteRedeemUrl* klicken, der in der Mitteilung im Schritt oben versendet wurde, und den interaktiven Einlösungsprozess in einem Browser durchführen. Nach Abschluss wird der eingeladene Benutzer ein externer Benutzer in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="e686b-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="e686b-117">Methoden</span><span class="sxs-lookup"><span data-stu-id="e686b-117">Methods</span></span>
| <span data-ttu-id="e686b-118">Methode</span><span class="sxs-lookup"><span data-stu-id="e686b-118">Method</span></span>       | <span data-ttu-id="e686b-119">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e686b-119">Return Type</span></span>  |<span data-ttu-id="e686b-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e686b-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e686b-121">Einladung erstellen</span><span class="sxs-lookup"><span data-stu-id="e686b-121">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="e686b-122">invitation</span><span class="sxs-lookup"><span data-stu-id="e686b-122">invitation</span></span> | <span data-ttu-id="e686b-123">Dient zum Schreiben der Eigenschaften und der Beziehungen des Einladungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="e686b-123">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e686b-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e686b-124">Properties</span></span>
| <span data-ttu-id="e686b-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e686b-125">Property</span></span>     | <span data-ttu-id="e686b-126">Typ</span><span class="sxs-lookup"><span data-stu-id="e686b-126">Type</span></span>   |<span data-ttu-id="e686b-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e686b-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e686b-128">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="e686b-128">invitedUserDisplayName</span></span>|<span data-ttu-id="e686b-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e686b-129">String</span></span>|<span data-ttu-id="e686b-130">Der Anzeigename des eingeladenen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e686b-130">The display name of the user being invited.</span></span>|
|<span data-ttu-id="e686b-131">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e686b-131">invitedUserEmailAddress</span></span>|<span data-ttu-id="e686b-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e686b-132">String</span></span>|<span data-ttu-id="e686b-p102">Die E-Mail-Adresse des eingeladenen Benutzers. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e686b-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="e686b-135">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="e686b-135">invitedUserMessageInfo</span></span>|[<span data-ttu-id="e686b-136">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="e686b-136">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="e686b-137">Zusätzliche Konfiguration für die an den eingeladenen Benutzer gesendete Nachricht, einschließlich des Anpassens des Nachrichtentexts, der Sprache und der Empfängerliste in CC.</span><span class="sxs-lookup"><span data-stu-id="e686b-137">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="e686b-138">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="e686b-138">sendInvitationMessage</span></span>|<span data-ttu-id="e686b-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e686b-139">Boolean</span></span>|<span data-ttu-id="e686b-p103">Gibt an, ob eine E-Mail-Nachricht an den eingeladenen Benutzer gesendet werden soll oder nicht. Der Standardwert ist „false“.</span><span class="sxs-lookup"><span data-stu-id="e686b-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="e686b-142">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="e686b-142">inviteRedirectUrl</span></span>|<span data-ttu-id="e686b-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e686b-143">String</span></span>|<span data-ttu-id="e686b-p104">Die URL, an die der eingeladene Benutzer umgeleitet werden sollte, nachdem die Einladung eingelöst wurde. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e686b-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="e686b-146">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="e686b-146">inviteRedeemUrl</span></span>|<span data-ttu-id="e686b-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e686b-147">String</span></span>|<span data-ttu-id="e686b-p105">Die URL, die der Benutzer zum Einlösen seiner Einladung verwenden kann. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="e686b-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="e686b-150">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="e686b-150">invitedUserType</span></span>|<span data-ttu-id="e686b-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e686b-151">String</span></span>|<span data-ttu-id="e686b-152">Der userType des eingeladenen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e686b-152">The userType of the user being invited.</span></span> <span data-ttu-id="e686b-153">Standardmäßig ist dieser Wert auf „Gast“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e686b-153">By default, this is Guest.</span></span> <span data-ttu-id="e686b-154">Wenn Sie der Unternehmensadministrator sind, können Sie ihn als „Mitglied“ einladen.</span><span class="sxs-lookup"><span data-stu-id="e686b-154">You can invite as Member if you are a company administrator.</span></span> |
|<span data-ttu-id="e686b-155">status</span><span class="sxs-lookup"><span data-stu-id="e686b-155">status</span></span>|<span data-ttu-id="e686b-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e686b-156">String</span></span>|<span data-ttu-id="e686b-p107">Der Status der Einladung. Mögliche Werte: PendingAcceptance, Completed, InProgress und Error</span><span class="sxs-lookup"><span data-stu-id="e686b-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="e686b-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e686b-159">Relationships</span></span>
| <span data-ttu-id="e686b-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e686b-160">Relationship</span></span> | <span data-ttu-id="e686b-161">Typ</span><span class="sxs-lookup"><span data-stu-id="e686b-161">Type</span></span>   |<span data-ttu-id="e686b-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e686b-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e686b-163">invitedUser</span><span class="sxs-lookup"><span data-stu-id="e686b-163">invitedUser</span></span>|[<span data-ttu-id="e686b-164">Benutzer</span><span class="sxs-lookup"><span data-stu-id="e686b-164">User</span></span>](user.md)|<span data-ttu-id="e686b-p108">Der Benutzer, der im Rahmen der Einladungserstellung erstellt wurde. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="e686b-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e686b-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e686b-167">JSON representation</span></span>
<span data-ttu-id="e686b-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e686b-168">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "baseType": "microsoft.graph.entity", "@odata.type": "microsoft.graph.invitation" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
