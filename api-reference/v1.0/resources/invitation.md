# <a name="invitation-manager"></a><span data-ttu-id="844d4-101">Einladungs-Manager</span><span class="sxs-lookup"><span data-stu-id="844d4-101">invitation manager</span></span>

<span data-ttu-id="844d4-102">Verwenden Sie den Einladungs-Manager, um eine Einladung zum Hinzufügen eines externen Benutzers zu der Organisation zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="844d4-102">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="844d4-103">Der Einladungsprozess verwendet den folgenden Ablauf:</span><span class="sxs-lookup"><span data-stu-id="844d4-103">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="844d4-104">Eine Einladung wird erstellt.</span><span class="sxs-lookup"><span data-stu-id="844d4-104">An invitation is created</span></span>
* <span data-ttu-id="844d4-105">Eine Einladung (mit einem Einladungs-Link) wird an den eingeladenen Benutzer gesendet.</span><span class="sxs-lookup"><span data-stu-id="844d4-105">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="844d4-106">Der eingeladene Benutzer klickt auf den Einladungs-Link, meldet sich an und löst die Einladung und die Erstellung der Benutzerentität ein, die den eingeladenen Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="844d4-106">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="844d4-107">Der Benutzer wird nach Abschluss der Einlösung zu einer bestimmten Seite umgeleitet.</span><span class="sxs-lookup"><span data-stu-id="844d4-107">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="844d4-p101">Durch Erstellen einer Einladung wird eine URL für die Einlösung in der Antwort zurückgegeben (*InviteRedeemUrl*). Die API zum Erstellen der Einladung kann automatisch eine E-Mail mit der Einlösungs-URL an den eingeladenen Benutzer senden, indem *sendInvitationMessage* auf „true“ festgelegt wird. Sie können die Nachricht, die an den eingeladenen Benutzer gesendet wird, auch anpassen. Wenn Sie die Einlösungs-URL anderweitig versenden möchten, können Sie die *sendInvitationMessage* auf „false“ festlegen und die Einlösungs-URL aus der Antwort verwenden, um Ihre eigene Mitteilung zu erstellen. Derzeit gibt es keine API, die den Einlösungsprozess durchführt. Der eingeladene Benutzer muss auf den Link *inviteRedeemUrl* klicken, der in der Mitteilung im Schritt oben versendet wurde, und den interaktiven Einlösungsprozess in einem Browser durchführen. Nach Abschluss wird der eingeladene Benutzer ein externer Benutzer in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="844d4-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="844d4-115">Methoden</span><span class="sxs-lookup"><span data-stu-id="844d4-115">Methods</span></span>
| <span data-ttu-id="844d4-116">Methode</span><span class="sxs-lookup"><span data-stu-id="844d4-116">Method</span></span>       | <span data-ttu-id="844d4-117">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="844d4-117">Return Type</span></span>  |<span data-ttu-id="844d4-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="844d4-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="844d4-119">Einladung erstellen</span><span class="sxs-lookup"><span data-stu-id="844d4-119">Create invitation</span></span>](../api/invitation_post.md) | <span data-ttu-id="844d4-120">invitation</span><span class="sxs-lookup"><span data-stu-id="844d4-120">invitation</span></span> | <span data-ttu-id="844d4-121">Dient zum Schreiben der Eigenschaften und der Beziehungen des Einladungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="844d4-121">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="844d4-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="844d4-122">Properties</span></span>
| <span data-ttu-id="844d4-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="844d4-123">Property</span></span>     | <span data-ttu-id="844d4-124">Typ</span><span class="sxs-lookup"><span data-stu-id="844d4-124">Type</span></span>   |<span data-ttu-id="844d4-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="844d4-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="844d4-126">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="844d4-126">invitedUserDisplayName</span></span>|<span data-ttu-id="844d4-127">String</span><span class="sxs-lookup"><span data-stu-id="844d4-127">String</span></span>|<span data-ttu-id="844d4-128">Der Anzeigename des eingeladenen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="844d4-128">The display name of the user being invited.</span></span>|
|<span data-ttu-id="844d4-129">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="844d4-129">invitedUserEmailAddress</span></span>|<span data-ttu-id="844d4-130">String</span><span class="sxs-lookup"><span data-stu-id="844d4-130">String</span></span>|<span data-ttu-id="844d4-p102">Die E-Mail-Adresse des eingeladenen Benutzers. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="844d4-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="844d4-133">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="844d4-133">invitedUserMessageInfo</span></span>|[<span data-ttu-id="844d4-134">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="844d4-134">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="844d4-135">Zusätzliche Konfiguration für die an den eingeladenen Benutzer gesendete Nachricht, einschließlich des Anpassens des Nachrichtentexts, der Sprache und der Empfängerliste in CC.</span><span class="sxs-lookup"><span data-stu-id="844d4-135">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="844d4-136">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="844d4-136">sendInvitationMessage</span></span>|<span data-ttu-id="844d4-137">Boolesch</span><span class="sxs-lookup"><span data-stu-id="844d4-137">Boolean</span></span>|<span data-ttu-id="844d4-p103">Gibt an, ob eine E-Mail-Nachricht an den eingeladenen Benutzer gesendet werden soll oder nicht. Der Standardwert ist „false“.</span><span class="sxs-lookup"><span data-stu-id="844d4-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="844d4-140">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="844d4-140">inviteRedirectUrl</span></span>|<span data-ttu-id="844d4-141">String</span><span class="sxs-lookup"><span data-stu-id="844d4-141">String</span></span>|<span data-ttu-id="844d4-p104">Die URL, an die der eingeladene Benutzer umgeleitet werden sollte, nachdem die Einladung eingelöst wurde. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="844d4-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="844d4-144">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="844d4-144">inviteRedeemUrl</span></span>|<span data-ttu-id="844d4-145">String</span><span class="sxs-lookup"><span data-stu-id="844d4-145">String</span></span>|<span data-ttu-id="844d4-p105">Die URL, die der Benutzer zum Einlösen seiner Einladung verwenden kann. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="844d4-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="844d4-148">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="844d4-148">invitedUserType</span></span>|<span data-ttu-id="844d4-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="844d4-149">String</span></span>|<span data-ttu-id="844d4-150">Der userType des eingeladenen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="844d4-150">The userType of the user being invited.</span></span> <span data-ttu-id="844d4-151">Standardmäßig ist dieser Wert auf „Gast“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="844d4-151">By default, this is Guest.</span></span> <span data-ttu-id="844d4-152">Wenn Sie der Unternehmensadministrator sind, können Sie ihn als „Mitglied“ einladen.</span><span class="sxs-lookup"><span data-stu-id="844d4-152">You can invite as Member if you are a company administrator.</span></span> |
|<span data-ttu-id="844d4-153">status</span><span class="sxs-lookup"><span data-stu-id="844d4-153">status</span></span>|<span data-ttu-id="844d4-154">String</span><span class="sxs-lookup"><span data-stu-id="844d4-154">String</span></span>|<span data-ttu-id="844d4-p107">Der Status der Einladung. Mögliche Werte: PendingAcceptance, Completed, InProgress und Error</span><span class="sxs-lookup"><span data-stu-id="844d4-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="844d4-157">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="844d4-157">Relationships</span></span>
| <span data-ttu-id="844d4-158">Beziehung</span><span class="sxs-lookup"><span data-stu-id="844d4-158">Relationship</span></span> | <span data-ttu-id="844d4-159">Typ</span><span class="sxs-lookup"><span data-stu-id="844d4-159">Type</span></span>   |<span data-ttu-id="844d4-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="844d4-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="844d4-161">invitedUser</span><span class="sxs-lookup"><span data-stu-id="844d4-161">invitedUser</span></span>|[<span data-ttu-id="844d4-162">Benutzer</span><span class="sxs-lookup"><span data-stu-id="844d4-162">User</span></span>](user.md)|<span data-ttu-id="844d4-p108">Der Benutzer, der im Rahmen der Einladungserstellung erstellt wurde. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="844d4-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="844d4-165">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="844d4-165">JSON representation</span></span>
<span data-ttu-id="844d4-166">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="844d4-166">Here is a JSON representation of the resource</span></span>

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
