---
title: Einladungs-Manager
description: 'Verwenden Sie den Einladungs-Manager, um eine Einladung zum Hinzufügen eines externen Benutzers zu der Organisation zu erstellen. '
localization_priority: Normal
ms.openlocfilehash: ffe09e5043b60b01728d497b88034b289bdc5131
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811242"
---
# <a name="invitation-manager"></a><span data-ttu-id="70459-103">Einladungs-Manager</span><span class="sxs-lookup"><span data-stu-id="70459-103">invitation manager</span></span>

> <span data-ttu-id="70459-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="70459-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70459-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70459-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70459-106">Verwenden Sie den Einladungs-Manager, um eine Einladung zum Hinzufügen eines externen Benutzers zu der Organisation zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="70459-106">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="70459-107">Der Einladungsprozess verwendet den folgenden Ablauf:</span><span class="sxs-lookup"><span data-stu-id="70459-107">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="70459-108">Eine Einladung wird erstellt.</span><span class="sxs-lookup"><span data-stu-id="70459-108">An invitation is created</span></span>
* <span data-ttu-id="70459-109">Eine Einladung (mit einem Einladungs-Link) wird an den eingeladenen Benutzer gesendet.</span><span class="sxs-lookup"><span data-stu-id="70459-109">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="70459-110">Der eingeladene Benutzer klickt auf den Einladungs-Link, meldet sich an und löst die Einladung und die Erstellung der Benutzerentität ein, die den eingeladenen Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="70459-110">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="70459-111">Der Benutzer wird nach Abschluss der Einlösung zu einer bestimmten Seite umgeleitet.</span><span class="sxs-lookup"><span data-stu-id="70459-111">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="70459-p102">Durch Erstellen einer Einladung wird eine URL für die Einlösung in der Antwort zurückgegeben (*InviteRedeemUrl*). Die API zum Erstellen der Einladung kann automatisch eine E-Mail mit der Einlösungs-URL an den eingeladenen Benutzer senden, indem *sendInvitationMessage* auf „true“ festgelegt wird. Sie können die Nachricht, die an den eingeladenen Benutzer gesendet wird, auch anpassen. Wenn Sie die Einlösungs-URL anderweitig versenden möchten, können Sie die *sendInvitationMessage* auf „false“ festlegen und die Einlösungs-URL aus der Antwort verwenden, um Ihre eigene Mitteilung zu erstellen. Derzeit gibt es keine API, die den Einlösungsprozess durchführt. Der eingeladene Benutzer muss auf den Link *inviteRedeemUrl* klicken, der in der Mitteilung im Schritt oben versendet wurde, und den interaktiven Einlösungsprozess in einem Browser durchführen. Nach Abschluss wird der eingeladene Benutzer ein externer Benutzer in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="70459-p102">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="70459-119">Methoden</span><span class="sxs-lookup"><span data-stu-id="70459-119">Methods</span></span>
| <span data-ttu-id="70459-120">Methode</span><span class="sxs-lookup"><span data-stu-id="70459-120">Method</span></span>       | <span data-ttu-id="70459-121">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="70459-121">Return Type</span></span>  |<span data-ttu-id="70459-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70459-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70459-123">Einladung erstellen</span><span class="sxs-lookup"><span data-stu-id="70459-123">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="70459-124">invitation</span><span class="sxs-lookup"><span data-stu-id="70459-124">invitation</span></span> | <span data-ttu-id="70459-125">Dient zum Schreiben der Eigenschaften und der Beziehungen des Einladungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="70459-125">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="70459-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70459-126">Properties</span></span>
| <span data-ttu-id="70459-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70459-127">Property</span></span>     | <span data-ttu-id="70459-128">Typ</span><span class="sxs-lookup"><span data-stu-id="70459-128">Type</span></span>   |<span data-ttu-id="70459-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70459-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70459-130">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="70459-130">invitedUserDisplayName</span></span>|<span data-ttu-id="70459-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70459-131">String</span></span>|<span data-ttu-id="70459-132">Der Anzeigename des eingeladenen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="70459-132">The display name of the user being invited.</span></span>|
|<span data-ttu-id="70459-133">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="70459-133">invitedUserEmailAddress</span></span>|<span data-ttu-id="70459-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70459-134">String</span></span>|<span data-ttu-id="70459-p103">Die E-Mail-Adresse des eingeladenen Benutzers. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="70459-p103">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="70459-137">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="70459-137">invitedUserMessageInfo</span></span>|[<span data-ttu-id="70459-138">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="70459-138">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="70459-139">Zusätzliche Konfiguration für die an den eingeladenen Benutzer gesendete Nachricht, einschließlich des Anpassens des Nachrichtentexts, der Sprache und der Empfängerliste in CC.</span><span class="sxs-lookup"><span data-stu-id="70459-139">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="70459-140">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="70459-140">sendInvitationMessage</span></span>|<span data-ttu-id="70459-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="70459-141">Boolean</span></span>|<span data-ttu-id="70459-p104">Gibt an, ob eine E-Mail-Nachricht an den eingeladenen Benutzer gesendet werden soll oder nicht. Der Standardwert ist „false“.</span><span class="sxs-lookup"><span data-stu-id="70459-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="70459-144">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="70459-144">inviteRedirectUrl</span></span>|<span data-ttu-id="70459-145">String</span><span class="sxs-lookup"><span data-stu-id="70459-145">String</span></span>|<span data-ttu-id="70459-p105">Die URL, an die der eingeladene Benutzer umgeleitet werden sollte, nachdem die Einladung eingelöst wurde. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="70459-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="70459-148">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="70459-148">inviteRedeemUrl</span></span>|<span data-ttu-id="70459-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70459-149">String</span></span>|<span data-ttu-id="70459-p106">Die URL, die der Benutzer zum Einlösen seiner Einladung verwenden kann. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="70459-p106">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="70459-152">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="70459-152">invitedUserType</span></span>|<span data-ttu-id="70459-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70459-153">String</span></span>|<span data-ttu-id="70459-p107">Der userType des eingeladenen Benutzers. Standardmäßig ist dieser Wert auf „Gast“ festgelegt. Wenn Sie der Unternehmensadministrator sind, können Sie ihn als „Mitglied“ einladen.</span><span class="sxs-lookup"><span data-stu-id="70459-p107">The userType of the user being invited. By default, this is Guest. You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="70459-157">status</span><span class="sxs-lookup"><span data-stu-id="70459-157">status</span></span>|<span data-ttu-id="70459-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70459-158">String</span></span>|<span data-ttu-id="70459-p108">Der Status der Einladung. Mögliche Werte: PendingAcceptance, Completed, InProgress und Error</span><span class="sxs-lookup"><span data-stu-id="70459-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="70459-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="70459-161">Relationships</span></span>
| <span data-ttu-id="70459-162">Beziehung</span><span class="sxs-lookup"><span data-stu-id="70459-162">Relationship</span></span> | <span data-ttu-id="70459-163">Typ</span><span class="sxs-lookup"><span data-stu-id="70459-163">Type</span></span>   |<span data-ttu-id="70459-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70459-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70459-165">invitedUser</span><span class="sxs-lookup"><span data-stu-id="70459-165">invitedUser</span></span>|[<span data-ttu-id="70459-166">Benutzer</span><span class="sxs-lookup"><span data-stu-id="70459-166">User</span></span>](user.md)|<span data-ttu-id="70459-p109">Der Benutzer, der im Rahmen der Einladungserstellung erstellt wurde. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="70459-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70459-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70459-169">JSON representation</span></span>
<span data-ttu-id="70459-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70459-170">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
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
