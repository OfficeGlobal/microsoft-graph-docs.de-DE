---
title: Bekannte Probleme in Microsoft Graph
description: Dieser Artikel beschreibt bekannte Probleme in Microsoft Graph. Informationen zu den neuesten Updates finden Sie im Microsoft Graph-Änderungsprotokoll.
ms.openlocfilehash: 254e40fa9a249ba0a23308b0c40a732b567eb6a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092223"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="40192-104">Bekannte Probleme in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="40192-104">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="40192-p102">Dieser Artikel beschreibt bekannte Probleme in Microsoft Graph. Informationen zu den neuesten Updates finden Sie im [Microsoft Graph-Änderungsprotokoll](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="40192-p102">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="40192-107">Benutzer</span><span class="sxs-lookup"><span data-stu-id="40192-107">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="40192-108">Kein direkter Zugriff nach der Erstellung</span><span class="sxs-lookup"><span data-stu-id="40192-108">No instant access after creation</span></span>

<span data-ttu-id="40192-p103">Benutzer können direkt über POST in der Benutzerentität erstellt werden. Eine Office 365-Lizenz muss zunächst einem Benutzer zugewiesen werden, damit dieser Zugriff auf Office 365-Dienste erhält. Aufgrund der verteilten Art des Diensts kann es bis zu 15 Minuten dauern, bis Dateien-, Nachrichten- und Ereignisentitäten für diesen Benutzer über die Microsoft Graph-API zur Verfügung stehen. In dieser Zeit erhalten Apps als Antwort den HTTP-Fehler 404.</span><span class="sxs-lookup"><span data-stu-id="40192-p103">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="40192-113">Fotoeinschränkungen</span><span class="sxs-lookup"><span data-stu-id="40192-113">Photo restrictions</span></span>

<span data-ttu-id="40192-p104">Benutzerprofilfotos können nur gelesen und aktualisiert werden, wenn der Benutzer über ein Postfach verfügt. Darüber hinaus kann auf Fotos, die *ggf.* zuvor mithilfe der **thumbnailPhoto**-Eigenschaft (unter Verwendung der Office 365 Unified-API-Vorschau oder Azure AD Graph oder über die AD Connect-Synchronisierung) gespeichert wurden, nicht mehr über die Microsoft Graph-Eigenschaft **photo** der [user](/graph/api/resources/user?view=graph-rest-1.0)-Ressource zugegriffen werden. Beim Auftreten eines Fehlers beim Lesen oder Aktualisieren eines Fotos wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="40192-p104">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

### <a name="using-delta-query"></a><span data-ttu-id="40192-117">Verwenden der Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="40192-117">Using delta query</span></span>

<span data-ttu-id="40192-118">Bekannte Probleme bei der Verwendung der Delta-Abfrage finden Sie im Abschnitt [ Delta-Abfrage](#delta-query) in diesem Artikel.</span><span class="sxs-lookup"><span data-stu-id="40192-118">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="microsoft-teams"></a><span data-ttu-id="40192-119">Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="40192-119">Microsoft Teams</span></span>

### <a name="application-permissions"></a><span data-ttu-id="40192-120">Anwendungsberechtigungen</span><span class="sxs-lookup"><span data-stu-id="40192-120">Application permissions</span></span>

<span data-ttu-id="40192-121">Beim Vornehmen von Änderungen an Teams und Kanälen mithilfe von Anwendungsberechtigungen rendert Microsoft Teams die im Kanal "Allgemein" veröffentlichte Steuerungsnachricht mit leerem Namen anstelle des Anwendungsnamens.</span><span class="sxs-lookup"><span data-stu-id="40192-121">When making changes to teams and channels using application permissions, Microsoft Teams renders the control message posted to the General channel with a blank name instead of the application name.</span></span> <span data-ttu-id="40192-122">Dieses Problem wird in einem zukünftigen Update behoben.</span><span class="sxs-lookup"><span data-stu-id="40192-122">This will be addressed in a future update.</span></span> <span data-ttu-id="40192-123">Durch den Fix werden bereits veröffentlichte Steuerungsnachrichten rückwirkend aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="40192-123">The fix will retroactively update control messages that are already posted.</span></span>

### <a name="create-chat-thread-api"></a><span data-ttu-id="40192-124">Chatthread-API erstellen</span><span class="sxs-lookup"><span data-stu-id="40192-124">Create chat thread API</span></span>

<span data-ttu-id="40192-125">Die aktuelle API zum [Erstellen eines Chatthreads](/graph/api/channel-post-chatthreads?view=graph-rest-beta) wird durch eine funktionsreichere API ersetzt, die mit dem Schema zum [Auflisten von Kanalnachrichten](/graph/api/channel-list-messages?view=graph-rest-beta) konsistent ist.</span><span class="sxs-lookup"><span data-stu-id="40192-125">The current API to [create a chat thread](/graph/api/channel-post-chatthreads?view=graph-rest-beta) will be replaced with a richer API that is consistent with the schema for [listing channel messages](/graph/api/channel-list-messages?view=graph-rest-beta).</span></span>

### <a name="graph-explorer-and-v10"></a><span data-ttu-id="40192-126">Graph Explorer und v1.0</span><span class="sxs-lookup"><span data-stu-id="40192-126">Graph Explorer and v1.0</span></span>

<span data-ttu-id="40192-127">Die Beispielabfragen für Graph Explorer wurden noch nicht für v1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="40192-127">Graph Explorer sample queries have not been updated for v1.0 yet.</span></span>
<span data-ttu-id="40192-128">Sie können trotzdem Abfragen für Version 1.0 in das Textfeld oben eingeben.</span><span class="sxs-lookup"><span data-stu-id="40192-128">You can still type v1.0 queries into the text box on the top.</span></span>
<span data-ttu-id="40192-129">Achten Sie darauf, dass Graph Explorer mit den entsprechenden Berechtigungen eingerichtet ist, wie etwa "Group.ReadWrite.All" und "User.Read.All".</span><span class="sxs-lookup"><span data-stu-id="40192-129">Make sure you have set up Graph Explorer with the appropriate permissions, such as Group.ReadWrite.All and User.Read.All.</span></span>

### <a name="graph-explorer-and-global-admins"></a><span data-ttu-id="40192-130">Graph-Explorer und globale Administratoren</span><span class="sxs-lookup"><span data-stu-id="40192-130">Graph Explorer and Global Admins</span></span>

<span data-ttu-id="40192-131">Derzeit lässt Graph Explorer die Bearbeitung von Teams durch globale Administratoren zu, die weder Besitzer noch Mitglied dieser Teams sind, bei den gleichen API-Aufrufen durch andere Apps tritt jedoch ein Fehler auf, wenn der aktuelle Benutzer kein Mitglied oder Besitzer des Teams ist.</span><span class="sxs-lookup"><span data-stu-id="40192-131">Currently, Graph Explorer allows global admins to manipulate teams they are not an owner or member of, but other apps attempting to make the same API calls will fail if the current user is not a member or owner of the team.</span></span>

### <a name="get-teams-and-post-teams-are-not-supported"></a><span data-ttu-id="40192-132">"GET /teams" und "POST /teams" werden nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40192-132">GET /teams and POST /teams are not supported</span></span>

<span data-ttu-id="40192-133">Informationen zum Auflisten aller Teams finden Sie unter [Alle Teams auflisten](teams-list-all-teams.md) und [Ihre Teams auflisten](/graph/api/user-list-joinedteams?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="40192-133">See [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) to get a list of teams.</span></span>
<span data-ttu-id="40192-134">Informationen zum Erstellen von Teams finden Sie unter [Teams erstellen](/graph/api/team-put-teams?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="40192-134">See [create team](/graph/api/team-put-teams?view=graph-rest-1.0) for creating teams.</span></span>

### <a name="missing-teams-in-list-all-teams"></a><span data-ttu-id="40192-135">Fehlende Teams in "Alle Teams auflisten"</span><span class="sxs-lookup"><span data-stu-id="40192-135">Missing teams in list all teams</span></span>

<span data-ttu-id="40192-136">Einige Teams, die früher erstellt, in letzter Zeit aber nicht von einem Microsoft Teams-Benutzer verwendet wurden, werden von [Alle Teams auflisten](teams-list-all-teams.md) nicht aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="40192-136">Some teams that were created in the past but haven't been used recently by a Microsoft Teams user aren't listed by [list all teams](teams-list-all-teams.md).</span></span>
<span data-ttu-id="40192-137">Neue Teams werden aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="40192-137">New teams will be listed.</span></span>
<span data-ttu-id="40192-138">Bestimmte alte Teams weisen keine Eigenschaft **resourceProvisioningOptions** auf, die "Team" enthält und bei neu erstellten Teams und in Microsoft Teams besuchten Teams festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="40192-138">Certain old teams don't have a **resourceProvisioningOptions** property that contains "Team", which is set on newly created teams and teams that are visited in Microsoft Teams.</span></span>
<span data-ttu-id="40192-139">Wir legen **resourceProvisioningOptions** zukünftig für vorhandene Teams fest, die nicht in Microsoft Teams geöffnet wurden.</span><span class="sxs-lookup"><span data-stu-id="40192-139">In the future, we will set **resourceProvisioningOptions** on existing teams that have not been opened in Microsoft Teams.</span></span>

## <a name="groups"></a><span data-ttu-id="40192-140">Gruppen</span><span class="sxs-lookup"><span data-stu-id="40192-140">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="40192-141">Berechtigungen für Gruppen und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="40192-141">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="40192-142">Microsoft Graph stellt zwei Berechtigungen ([*Group.Read.All*](permissions-reference.md#group-permissions) und [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) für den Zugriff auf Gruppen und Microsoft Teams zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="40192-142">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="40192-143">Diesen Berechtigungen muss von einem Administrator zugestimmt werden.</span><span class="sxs-lookup"><span data-stu-id="40192-143">App permissions must be consented to by an Office 365 tenant administrator.</span></span>
<span data-ttu-id="40192-144">Zukünftig sollen neue Berechtigungen für Gruppen und Teams hinzugefügt werden, für die Benutzer ihre Zustimmung erteilen können.</span><span class="sxs-lookup"><span data-stu-id="40192-144">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="40192-p110">Außerdem unterstützt nur die API für die Hauptgruppenadministration und -verwaltung den Zugriff mithilfe delegierter oder Nur-App-Berechtigungen. Alle anderen Features der Gruppen-API unterstützen nur delegierte Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="40192-p110">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="40192-147">Beispiele für Gruppenfeatures, die delegierte und Nur-App-Berechtigungen unterstützen:</span><span class="sxs-lookup"><span data-stu-id="40192-147">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="40192-148">Erstellen und Löschen von Gruppen</span><span class="sxs-lookup"><span data-stu-id="40192-148">Creating and deleting groups</span></span>
* <span data-ttu-id="40192-149">Abrufen und Aktualisieren von Gruppeneigenschaften, die zur Gruppenadministration oder -verwaltung gehören</span><span class="sxs-lookup"><span data-stu-id="40192-149">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="40192-150">[Verzeichniseinstellungen](/graph/api/resources/directoryobject?view=graph-rest-1.0) für Gruppen, Typ und Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="40192-150">Group [directory settings](/graph/api/resources/directoryobject?view=graph-rest-1.0), type, and synchronization</span></span>
* <span data-ttu-id="40192-151">Gruppenbesitzer und Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="40192-151">Group owners and membership</span></span>

<span data-ttu-id="40192-152">Beispiele für Gruppenfeatures, die nur delegierte Berechtigungen unterstützen:</span><span class="sxs-lookup"><span data-stu-id="40192-152">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="40192-153">Gruppenunterhaltungen, Ereignisse, Fotos</span><span class="sxs-lookup"><span data-stu-id="40192-153">Group conversations, events, photo</span></span>
* <span data-ttu-id="40192-154">Externe Absender, akzeptierte oder abgelehnte Absender, Gruppenabonnement</span><span class="sxs-lookup"><span data-stu-id="40192-154">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="40192-155">Benutzerfavoriten und Anzahl ungesehener Elemente</span><span class="sxs-lookup"><span data-stu-id="40192-155">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="40192-156">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="40192-156">Policy</span></span>

<span data-ttu-id="40192-157">Beim Erstellen und Benennen einer Office 365-Gruppe mit Microsoft Graph werden Office 365-Gruppenrichtlinien umgangen, die über Outlook Web App konfiguriert werden.</span><span class="sxs-lookup"><span data-stu-id="40192-157">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="adding-and-getting-attachments-of-group-posts"></a><span data-ttu-id="40192-158">Hinzufügen und Abrufen von Anlagen von Gruppenbeiträgen</span><span class="sxs-lookup"><span data-stu-id="40192-158">Adding and getting attachments of group posts</span></span>

<span data-ttu-id="40192-p111">Durch das [Hinzufügen](/graph/api/post-post-attachments?view=graph-rest-1.0) von Anlagen zu Gruppenbeiträgen, das [Auflisten](/graph/api/post-list-attachments?view=graph-rest-1.0) und das Abrufen von Anlagen von Gruppenbeiträgen wird aktuell die Fehlermeldung „Die OData-Anforderung wird nicht unterstützt“ zurückgegeben. Für die `/v1.0`- und `/beta`-Versionen wurde eine Problemlösung entwickelt, die bis Ende Januar 2016 allgemein verfügbar sein sollte.</span><span class="sxs-lookup"><span data-stu-id="40192-p111">[Adding](/graph/api/post-post-attachments?view=graph-rest-1.0) attachments to group posts, [listing](/graph/api/post-list-attachments?view=graph-rest-1.0) and getting attachments of group posts currently return the error message "The OData request is not supported." A fix has been rolled out for both the `/v1.0` and `/beta` versions, and is expected to be widely available by the end of January 2016.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="40192-161">Festlegen der allowExternalSenders-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40192-161">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="40192-162">Aktuell liegt ein Problem vor, aufgrund dessen sich die Eigenschaft **allowExternalSenders** einer Gruppe in POST- oder PATCH-Operationen nicht festlegen lässt. Das Problem tritt sowohl in `/v1.0` als auch in `/beta` auf.</span><span class="sxs-lookup"><span data-stu-id="40192-162">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="40192-163">Verwenden der Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="40192-163">Using delta query</span></span>

<span data-ttu-id="40192-164">Bekannte Probleme bei der Verwendung der Delta-Abfrage finden Sie im Abschnitt [ Delta-Abfrage](#delta-query) in diesem Artikel.</span><span class="sxs-lookup"><span data-stu-id="40192-164">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="bookings"></a><span data-ttu-id="40192-165">Bookings</span><span class="sxs-lookup"><span data-stu-id="40192-165">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="40192-166">„ErrorExceededFindCountLimit“ bei Abfrage von „bookingBusinesses“</span><span class="sxs-lookup"><span data-stu-id="40192-166">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="40192-167">Beim Abrufen der Liste mit `bookingBusinesses` tritt ein Fehler mit dem folgenden Fehlercode auf, wenn eine Organisation über mehrere Buchungsunternehmen verfügt und das Konto, das die Anforderung stellt, kein Administratorkonto ist:</span><span class="sxs-lookup"><span data-stu-id="40192-167">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="40192-168">Schränken Sie zur Umgehung dieses Problems den Satz von Unternehmen ein, der von der Anforderung zurückgegeben wird, indem Sie einen `query`-Parameter einbeziehen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="40192-168">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```


## <a name="calendars"></a><span data-ttu-id="40192-169">Kalender</span><span class="sxs-lookup"><span data-stu-id="40192-169">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="40192-170">Zugreifen auf einen freigegebenen Kalender</span><span class="sxs-lookup"><span data-stu-id="40192-170">Accessing a shared calendar</span></span>

<span data-ttu-id="40192-171">Beim Versuch, auf Ereignisse in einem Kalender zuzugreifen, der von einem anderen Benutzer mithilfe des folgenden Vorgangs freigegeben wurde:</span><span class="sxs-lookup"><span data-stu-id="40192-171">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="40192-p112">Möglicherweise wird HTTP 500 mit dem Fehlercode `ErrorInternalServerTransientError` angezeigt. Der Fehler tritt aus folgendem Grund auf:</span><span class="sxs-lookup"><span data-stu-id="40192-p112">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="40192-174">Bisher gibt es zwei Methoden zur Implementierung der Kalenderfreigabe, die zur Unterscheidung einmal als der „alte“ Implementierungsansatz und einmal als der „neue“ Implementierungsansatz bezeichnet werden.</span><span class="sxs-lookup"><span data-stu-id="40192-174">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="40192-175">Der neue Ansatz ist derzeit für die Kalenderfreigabe mit Berechtigungen zum Anzeigen oder Bearbeiten verfügbar, jedoch nicht mit  aber nicht mit Berechtigungen der Stellvertretung.</span><span class="sxs-lookup"><span data-stu-id="40192-175">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="40192-176">Sie können die Kalender-REST-API verwenden, um freigegebene Kalender anzuzeigen oder freizugeben, aber nur, wenn die Kalender auf die **neue** Weise freigegebenen wurden.</span><span class="sxs-lookup"><span data-stu-id="40192-176">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="40192-177">Sie können die Kalender-REST-API nicht verwenden, um freigegebene Kalender (oder deren Ereignisse) anzuzeigen oder freizugeben, wenn die Kalender auf die **alte** Weise freigegebenen wurden.</span><span class="sxs-lookup"><span data-stu-id="40192-177">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="40192-178">Wenn ein Kalender mit Berechtigungen zum Anzeigen oder Bearbeiten auf die alte Weise freigegeben wurde, können Sie dieses Problem umgehen und die Kalenderfreigabe für die Verwendung des neuen Ansatzes aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="40192-178">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="40192-179">Im Laufe der Zeit werden alle freigegebenen Kalender für die Verwendung des neuen Ansatzes automatisch in Outlook aktualisiert, einschließlich mit Berechtigungen der Stellvertretung freigegebener Kalender.</span><span class="sxs-lookup"><span data-stu-id="40192-179">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="40192-180">Gehen Sie folgendermaßen vor, um einen freigegebenen Kalender für die Verwendung des neuen Ansatzes manuell zu aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="40192-180">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="40192-181">Der Empfänger entfernt den Kalender, der zuvor für diesen freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="40192-181">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="40192-182">Der Besitzer des Kalenders gibt den Kalender erneut in Outlook im Web, Outlook für iOS oder Outlook für Android frei.</span><span class="sxs-lookup"><span data-stu-id="40192-182">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="40192-p114">Der Empfänger akzeptiert den freigegebenen Kalender mithilfe von Outlook im Web erneut. (Zukünftig können auch andere Outlook-Clients verwendet werden.)</span><span class="sxs-lookup"><span data-stu-id="40192-p114">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="40192-185">Der Empfänger überprüft, ob der Kalender auf die neue Weise erfolgreich erneut freigegeben wurde und in Outlook für iOS oder in Outlook für Android angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="40192-185">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="40192-p115">Ein für Sie mit dem neuen Ansatz freigegebener Kalender wird genau wie jeder andere Kalender in Ihrem Postfach angezeigt. Sie können die Kalender-REST-API verwenden, um Ereignisse im freigegebenen Kalender so anzuzeigen oder zu bearbeiten, als wäre es Ihr eigener Kalender. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="40192-p115">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="40192-189">Hinzufügen von und Zugreifen auf ICS-basierte Kalender im Postfach des Benutzers</span><span class="sxs-lookup"><span data-stu-id="40192-189">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="40192-190">Derzeit gibt es eine teilweise Unterstützung für einen Kalender, der auf einem Internet-Kalenderabonnement (ICS) basiert:</span><span class="sxs-lookup"><span data-stu-id="40192-190">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="40192-191">Sie können einen ICS-basierten Kalender einem Benutzerpostfach über die Benutzeroberfläche, jedoch nicht über die Microsoft Graph-API hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="40192-191">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="40192-p116">[Das Auflisten der Kalender des Benutzers](/graph/api/user-list-calendars?view=graph-rest-1.0) ermöglicht Ihnen, die Eigenschaften **name**, **color** und **id** jedes [Kalenders](/graph/api/resources/calendar?view=graph-rest-1.0) in der Standardkalendergruppe des Benutzers oder einer bestimmten Kalendergruppe abzurufen, einschließlich ICS-basierte Kalender. Sie können die ICS-URL in der Kalenderressource nicht speichern und nicht darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="40192-p116">[Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="40192-194">Sie haben auch die Möglichkeit zum [Auflisten der Ereignisse](/graph/api/calendar-list-events?view=graph-rest-1.0) eines ICS-basierten Kalenders.</span><span class="sxs-lookup"><span data-stu-id="40192-194">You can also [list the events](/graph/api/calendar-list-events?view=graph-rest-1.0) of an ICS-based calendar.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="40192-195">Unterstützung für die onlineMeetingUrl-Eigenschaft in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="40192-195">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="40192-196">Derzeit gibt die **onlineMeetingUrl**-Eigenschaft einer Skype-Besprechung [event](/graph/api/resources/event?view=graph-rest-1.0) die URL der Online-Besprechung angeben.</span><span class="sxs-lookup"><span data-stu-id="40192-196">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event?view=graph-rest-1.0) would indicate the online meeting URL.</span></span> <span data-ttu-id="40192-197">Allerdings wird diese Eigenschaft für eine Microsoft Teams-Besprechung auf Null festgelegt.</span><span class="sxs-lookup"><span data-stu-id="40192-197">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

## <a name="calls-and-online-meetings"></a><span data-ttu-id="40192-198">Anrufe und Onlinebesprechungen</span><span class="sxs-lookup"><span data-stu-id="40192-198">Calls and online meetings</span></span>

> <span data-ttu-id="40192-199">**Hinweis** Anrufe und Onlinebesprechungen befinden sich aktuell im Vorschaustadium und sind nur am Beta-Endpunkt von Microsoft Graph verfügbar.</span><span class="sxs-lookup"><span data-stu-id="40192-199">**Note** Calling and online meetings are currently in preview and are available only in the Microsoft Graph beta endpoint.</span></span>

- <span data-ttu-id="40192-200">Der Navigationspfad `/applications/{id}` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-200">Navigation path `/applications/{id}` is not supported.</span></span> <span data-ttu-id="40192-201">Das Navigieren zur Anwendung über den globalen Anwendungsknoten ist nicht zulässig, selbst, wenn es sich um den eigenen handelt.</span><span class="sxs-lookup"><span data-stu-id="40192-201">Navigating through the global applications node to the application, even your own, is not allowed.</span></span> <span data-ttu-id="40192-202">Verwenden Sie nur die `/app`-Navigation.</span><span class="sxs-lookup"><span data-stu-id="40192-202">Please use the `/app` navigation only.</span></span>

## <a name="contacts"></a><span data-ttu-id="40192-203">Kontakte</span><span class="sxs-lookup"><span data-stu-id="40192-203">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="40192-204">Organisationskontakte nur in Betaversion verfügbar</span><span class="sxs-lookup"><span data-stu-id="40192-204">Organization contacts available in only beta</span></span>

<span data-ttu-id="40192-p119">Derzeit werden nur persönliche Kontakten unterstützt. Organisationskontakte werden derzeit nicht in `/v1.0` unterstützt, sind jedoch in `/beta` vorhanden.</span><span class="sxs-lookup"><span data-stu-id="40192-p119">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="40192-207">Standardordner für Kontakte</span><span class="sxs-lookup"><span data-stu-id="40192-207">Default contacts folder</span></span>

<span data-ttu-id="40192-208">In der `/v1.0`-Version enthält `GET /me/contactFolders` keinen Standardordner für Kontakte des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="40192-208">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="40192-p120">Es wird ein Update zur Verfügung gestellt. In der Zwischenzeit können Sie die folgende [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0)-Abfrage und die **parentFolderId**-Eigenschaft als Problemumgehung verwenden, um die ID des Standardordners für Kontakte abzurufen:</span><span class="sxs-lookup"><span data-stu-id="40192-p120">A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="40192-211">In der obigen Abfrage gilt Folgendes:</span><span class="sxs-lookup"><span data-stu-id="40192-211">In the above query:</span></span>

1. <span data-ttu-id="40192-212">`/me/contacts?$top=1` ruft die Eigenschaften eines [Kontakts](/graph/api/resources/contact?view=graph-rest-1.0) im Standardordner für Kontakte ab.</span><span class="sxs-lookup"><span data-stu-id="40192-212">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact?view=graph-rest-1.0) in the default contacts folder.</span></span>
2. <span data-ttu-id="40192-213">Das Anfügen von `&$select=parentFolderId` gibt nur die **parentFolderId**-Eigenschaft des Kontakts zurück, also die ID des Standardordners für Kontakte.</span><span class="sxs-lookup"><span data-stu-id="40192-213">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="40192-214">Zugreifen auf Kontakte über einen Kontakteordner in der Betaversion</span><span class="sxs-lookup"><span data-stu-id="40192-214">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="40192-215">In der Version `/beta` liegt aktuell ein Problem vor, aufgrund dessen der Zugriff auf einen [Kontakt](/graph/api/resources/contact?view=graph-rest-beta) über die Angabe seines übergeordneten Ordners in der REST-Anforderungs-URL in den folgenden 2 Szenarien nicht möglich ist:</span><span class="sxs-lookup"><span data-stu-id="40192-215">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="40192-216">Zugreifen auf einen Kontakt über ein [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta)-Objekt höchster Ebene des Benutzers</span><span class="sxs-lookup"><span data-stu-id="40192-216">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="40192-p121">Zugreifen auf einen Kontakt in einem untergeordneten Ordner eines **contactFolder**-Objekts  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="40192-p121">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="40192-219">Alternativ können Sie den Kontakt ganz einfach [per GET-Befehl abrufen](/graph/api/contact-get?view=graph-rest-beta), indem Sie seine ID wie unten gezeigt angeben. Das funktioniert, weil der Befehl „GET /contacts“ in der Version `/beta` auf alle Kontakte im Postfach des Benutzers angewendet wird:</span><span class="sxs-lookup"><span data-stu-id="40192-219">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="40192-220">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="40192-220">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="40192-221">Der comment-Parameter für das Erstellen eines Entwurfs</span><span class="sxs-lookup"><span data-stu-id="40192-221">The comment parameter for creating a draft</span></span>

<span data-ttu-id="40192-222">Der comment-Parameter für das Erstellen eines Antwort- oder Weiterleitungsentwurfs ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) wird nicht Teil des Textkörpers des resultierenden Nachrichtenentwurfs.</span><span class="sxs-lookup"><span data-stu-id="40192-222">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="40192-223">Nachrichten abrufen gibt Chats in Microsoft Teams zurück</span><span class="sxs-lookup"><span data-stu-id="40192-223">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="40192-224">In den v1- und Beta-Endpunkten beinhaltet die Antwort von `GET /users/id/messages` die Chats des Benutzers aus Microsoft Teams, die außerhalb des Bereichs eines Teams oder Kanal erfolgt sind.</span><span class="sxs-lookup"><span data-stu-id="40192-224">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="40192-225">Diese Chatnachrichten haben „Chat“ als Betreff.</span><span class="sxs-lookup"><span data-stu-id="40192-225">These chat messages have "IM" as their subject.</span></span>


## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="40192-226">Laufwerke, Dateien und Streamen von Inhalten</span><span class="sxs-lookup"><span data-stu-id="40192-226">Drives, files and content streaming</span></span>

* <span data-ttu-id="40192-227">Beim ersten Zugriff auf ein persönliches Benutzerlaufwerk über Microsoft Graph tritt ein 401-Fehler auf, wenn der Benutzer seine persönliche Website noch nicht in einem Browser aufgerufen hat.</span><span class="sxs-lookup"><span data-stu-id="40192-227">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="40192-228">Einschränkungen für Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="40192-228">Query parameter limitations</span></span>

* <span data-ttu-id="40192-229">Mehrere Namespaces werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-229">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="40192-230">GET-Anforderungen für `$ref` und Umwandlung wird für Benutzer, Gruppen, Geräte, Dienstprinzipale und Anwendungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-230">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="40192-p123">`@odata.bind` wird nicht unterstützt.  Ein Entwickler kann daher `Accepted` oder `RejectedSenders` für eine Gruppe nicht ordnungsgemäß festlegen.</span><span class="sxs-lookup"><span data-stu-id="40192-p123">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the `Accepted` or `RejectedSenders` on a group.</span></span>
* <span data-ttu-id="40192-233">`@odata.id` ist bei Nicht-Aufnahmenavigationen (z. B. Nachrichten) nicht vorhanden, wenn minimale Metadaten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="40192-233">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="40192-234">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="40192-234"></span></span>
  * <span data-ttu-id="40192-235">Keine Unterstützung für `nextLink`.</span><span class="sxs-lookup"><span data-stu-id="40192-235">No support for `nextLink`</span></span>
  * <span data-ttu-id="40192-236">Keine Unterstützung für mehr als eine Erweiterungsebene.</span><span class="sxs-lookup"><span data-stu-id="40192-236">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="40192-237">Keine Unterstützung mit zusätzlichen Parametern (`$filter`, `$select`).</span><span class="sxs-lookup"><span data-stu-id="40192-237">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="40192-238">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="40192-238"></span></span>
  * <span data-ttu-id="40192-239">Filter werden vom `/attachments`-Endpunkt nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-239">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="40192-240">Falls vorhanden, wird der `$filter`-Parameter ignoriert.</span><span class="sxs-lookup"><span data-stu-id="40192-240">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="40192-241">Arbeitsauslastungsübergreifende Filter werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-241">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="40192-242">`$search`:</span><span class="sxs-lookup"><span data-stu-id="40192-242"></span></span>
  * <span data-ttu-id="40192-243">Volltextsuche ist nur für einige Entitäten wie Nachrichten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="40192-243">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="40192-244">Arbeitsauslastungsübergreifende Suche wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-244">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="40192-245">Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="40192-245">Delta query</span></span>

* <span data-ttu-id="40192-246">OData-Kontext wird beim Nachverfolgen von Änderungen an Beziehungen manchmal falsch zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40192-246">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="40192-247">Schemaerweiterungen (Legacy) werden nicht mit $select-Anweisung, sondern ohne $select zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40192-247">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="40192-248">Clients können keine Änderungen an offenen Erweiterungen oder registrierten Schemaerweiterungen nachverfolgen.</span><span class="sxs-lookup"><span data-stu-id="40192-248">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="40192-249">Änderungen an der application- und servicePrincipal-API</span><span class="sxs-lookup"><span data-stu-id="40192-249">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="40192-p125">Es gibt Änderungen an den [application](/graph/api/resources/application?view=graph-rest-beta)- und [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta)-Entitäten, die derzeit entwickelt werden. Nachfolgend finden Sie eine Zusammenfassung aktueller Einschränkungen und API-Features, die derzeit entwickelt werden.</span><span class="sxs-lookup"><span data-stu-id="40192-p125">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="40192-252">Aktuelle Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="40192-252">Current limitations:</span></span>

* <span data-ttu-id="40192-253">Einige Anwendungseigenschaften (z. B. appRoles und addIns) sind erst verfügbar, wenn alle Änderungen abgeschlossen sind.</span><span class="sxs-lookup"><span data-stu-id="40192-253">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="40192-254">Es können nur Apps mit mehreren Mandanten registriert werden.</span><span class="sxs-lookup"><span data-stu-id="40192-254">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="40192-255">Das Aktualisieren von Apps ist auf Apps beschränkt, die nach dem anfänglichen Beta-Update registriert wurden.</span><span class="sxs-lookup"><span data-stu-id="40192-255">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="40192-256">Azure Active Directory-Benutzer können Apps registrieren und weitere Besitzer hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="40192-256">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="40192-257">Unterstützung für OpenID Connect und OAuth-Protokolle.</span><span class="sxs-lookup"><span data-stu-id="40192-257">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="40192-258">Richtlinienzuweisungen zu einer App schlagen fehl.</span><span class="sxs-lookup"><span data-stu-id="40192-258">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="40192-259">Vorgänge mit ownedObjects, die die appId erfordern, schlagen fehl (z. B. users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="40192-259">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="40192-260">In der Entwicklung:</span><span class="sxs-lookup"><span data-stu-id="40192-260">In development:</span></span>

* <span data-ttu-id="40192-261">Die Möglichkeit, Apps mit nur einem Mandanten zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="40192-261">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="40192-262">Updates für servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="40192-262">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="40192-263">Migration von vorhandenen Azure AD-Apps zum aktualisierten Modell.</span><span class="sxs-lookup"><span data-stu-id="40192-263">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="40192-264">Unterstützung für appRoles, vorab autorisierte Clients, optionale Ansprüche, Gruppenmitgliedschaftsansprüche und Branding</span><span class="sxs-lookup"><span data-stu-id="40192-264">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="40192-265">Benutzer eines Microsoft-Kontos (MSA-Benutzer) können Apps registrieren.</span><span class="sxs-lookup"><span data-stu-id="40192-265">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="40192-266">Unterstützung für SAML und WsFed-Protokolle.</span><span class="sxs-lookup"><span data-stu-id="40192-266">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="40192-267">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="40192-267">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="40192-268">Die Änderungsnachverfolgung wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-268">Change tracking is not supported</span></span>

<span data-ttu-id="40192-269">Die Änderungsnachverfolgung (Delta-Abfrage) wird für Eigenschaften von offenen Erweiterungen oder Schemaerweiterungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-269">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="40192-270">Gleichzeitiges Erstellen einer Ressource und einer offenen Erweiterung</span><span class="sxs-lookup"><span data-stu-id="40192-270">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="40192-p126">Wenn Sie eine Instanz von Ressourcen des Typs **administrativeUnit**, **device**, **group**, **organization** oder **user** erstellen, können Sie nicht gleichzeitig eine offene Erweiterung angeben. Sie müssen zuerst die Instanz erstellen und dann eine ``POST``-Anforderung auf diese Instanz anwenden, in der Sie die Daten der offenen Erweiterung angeben.</span><span class="sxs-lookup"><span data-stu-id="40192-p126">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="40192-273">Erstellen einer Ressourceninstanz und Hinzufügen von Schemaerweiterungsdaten zur gleichen Zeit</span><span class="sxs-lookup"><span data-stu-id="40192-273">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="40192-274">Sie können während des Vorgangs zum Erstellen einer **contact**-, **event**-, **message**- oder **post**-Instanz nicht gleichzeitig eine Schemaerweiterung festlegen.</span><span class="sxs-lookup"><span data-stu-id="40192-274">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="40192-275">Sie müssen zuerst die Ressourceninstanz erstellen und dann einen `PATCH` für die betreffende Instanz durchführen, um eine Schemaerweiterung und benutzerdefinierte Daten hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="40192-275">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="40192-276">Grenzwert von 100 zulässigen Werten für Schemaerweiterungseigenschaften pro Ressourceninstanz.</span><span class="sxs-lookup"><span data-stu-id="40192-276">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="40192-277">Für Verzeichnisressourcen wie **device**, **group** und **user** gilt aktuell: Für eine Ressourceninstanz dürfen maximal 100 Eigenschaftswerte von Schemaerweiterungen festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="40192-277">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="40192-278">Filtern von Schemaerweiterungseigenschaften wird nicht für alle Entitätstypen unterstützt</span><span class="sxs-lookup"><span data-stu-id="40192-278">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="40192-279">Das Filtern von Schemaerweiterungseigenschaften (mit dem Ausdruck `$filter`) wird für Outlook-Entitätstypen – **contact**, **event**, **message** oder **post**, nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-279">Filtering on schema extension properties (using the `$filter` expresssion) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="json-batching"></a><span data-ttu-id="40192-280">JSON-Batchverarbeitung</span><span class="sxs-lookup"><span data-stu-id="40192-280">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="40192-281">Keine geschachtelter Batch</span><span class="sxs-lookup"><span data-stu-id="40192-281">No nested batch</span></span>

<span data-ttu-id="40192-282">JSON-Batchanforderungen dürfen keine geschachtelten Batchanforderungen enthalten.</span><span class="sxs-lookup"><span data-stu-id="40192-282">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="40192-283">Alle einzelnen Anforderungen müssen synchron sein.</span><span class="sxs-lookup"><span data-stu-id="40192-283">All individual requests must be synchronous</span></span>

<span data-ttu-id="40192-p128">Alle in einer Batchanforderung enthaltenen Anforderungen müssen synchron ausgeführt werden. Falls vorhanden, wird die `respond-async`-Präferenz ignoriert.</span><span class="sxs-lookup"><span data-stu-id="40192-p128">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="40192-286">Keine Transaktionen</span><span class="sxs-lookup"><span data-stu-id="40192-286">No transactions</span></span>

<span data-ttu-id="40192-p129">Microsoft Graph unterstützt derzeit keine Transaktionsverarbeitung von einzelnen Anforderungen. Die `atomicityGroup`-Eigenschaft von einzelnen Anforderungen wird ignoriert.</span><span class="sxs-lookup"><span data-stu-id="40192-p129">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="40192-289">URIs müssen relativ sein</span><span class="sxs-lookup"><span data-stu-id="40192-289">URIs must be relative</span></span>

<span data-ttu-id="40192-p130">Geben Sie in Batchanforderungen immer relative URIs an. Microsoft Graph macht daraus dann mithilfe des in der Batch-URL enthaltenen Versionsendpunkts absolute URLs.</span><span class="sxs-lookup"><span data-stu-id="40192-p130">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="40192-292">Beschränkung der Batchgröße</span><span class="sxs-lookup"><span data-stu-id="40192-292">Limit on batch size</span></span>

<span data-ttu-id="40192-293">JSON-Batchanforderungen sind derzeit auf 20 einzelne Anforderungen beschränkt.</span><span class="sxs-lookup"><span data-stu-id="40192-293">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="40192-294">Vereinfachte Abhängigkeiten</span><span class="sxs-lookup"><span data-stu-id="40192-294">Simplified dependencies</span></span>

<span data-ttu-id="40192-p131">Einzelne Anforderungen können von anderen einzelnen Anforderungen abhängen. Derzeit können Anforderungen nur von einer einzigen anderen Anforderung abhängen und müssen einem der folgenden drei Muster entsprechen:</span><span class="sxs-lookup"><span data-stu-id="40192-p131">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="40192-297">Parallel: Eine einzelne Anforderung gibt eine Abhängigkeit in der `dependsOn`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="40192-297">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="40192-298">Seriell: Alle einzelnen Anforderungen hängen von der vorherigen einzelnen Anforderung ab.</span><span class="sxs-lookup"><span data-stu-id="40192-298">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="40192-299">Gleich: Alle einzelnen Anforderungen, die eine Abhängigkeit in der `dependsOn`-Eigenschaft angeben, geben die gleiche Abhängigkeit an.</span><span class="sxs-lookup"><span data-stu-id="40192-299">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="40192-300">In der weiteren Entwicklung der JSON-Batchverarbeitung werden diese Einschränkungen entfernt.</span><span class="sxs-lookup"><span data-stu-id="40192-300">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="40192-301">Apps vom Cloudlösungsanbieter</span><span class="sxs-lookup"><span data-stu-id="40192-301">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="40192-302">Apps vom Cloudlösungsanbieter müssen den Azure AD-Endpunkt verwenden</span><span class="sxs-lookup"><span data-stu-id="40192-302">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="40192-p132">CSP-Apps (Cloud-Lösungsanbieter) müssen Token von den Azure AD (v1)-Endpunkten erwerben, um Microsoft Graph erfolgreich in ihren partnerverwalteten Kunden aufrufen zu können. Derzeit wird der Erwerb eines Tokens über den neueren Azure AD v2.0-Endpunkt nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40192-p132">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="40192-305">Eine Vorabgenehmigung für Apps vom Cloudlösungsanbieter funktioniert bei einigen Kundenmandanten nicht</span><span class="sxs-lookup"><span data-stu-id="40192-305">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="40192-306">Unter bestimmten Umständen funktioniert die Vorabgenehmigung für Apps vom Cloudlösungsanbieter bei einigen Kundenmandanten nicht.</span><span class="sxs-lookup"><span data-stu-id="40192-306">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="40192-307">Für Apps, die delegierte Berechtigungen verwenden, wird bei der ersten Verwendung der App mit einem neuen Kundenmandanten möglicherweise der folgende Fehler nach der Anmeldung angezeigt: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="40192-307">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="40192-308">Für Apps, die Anwendungsberechtigungen verwenden, kann Ihre App ein Token erfassen, beim Aufrufen von Microsoft Graph wird jedoch unerwartet die Meldung angezeigt, dass der Zugriff verweigert wurde.</span><span class="sxs-lookup"><span data-stu-id="40192-308">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="40192-309">Wir arbeiten daran, dieses Problem so schnell wie möglich zu lösen, damit die Vorabgenehmigung für alle Kundenmandanten funktioniert.</span><span class="sxs-lookup"><span data-stu-id="40192-309">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="40192-310">In der Zwischenzeit können Sie die folgende Problemumgehung verwenden, um die Entwicklung und das Testen nicht zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="40192-310">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="40192-p133">**HINWEIS:** Dies ist keine dauerhafte Lösung und soll nur dazu dienen, die Entwicklung nicht zu blockieren.  Diese Problemumgehung ist nicht mehr erforderlich, nachdem das zuvor erwähnte Problem behoben wurde.  Diese Problemumgehung muss nicht rückgängig gemacht werden, nachdem die Korrektur vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="40192-p133">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="40192-p134">Öffnen Sie eine Azure AD v2-PowerShell-Sitzung, und stellen Sie eine Verbindung mit Ihrem `customer`-Mandanten her, indem Sie Ihre Administrator-Anmeldeinformationen in das Anmeldefenster eingeben. Sie können Azure AD PowerShell V2 [hier](https://www.powershellgallery.com/packages/AzureAD) herunterladen und installieren.</span><span class="sxs-lookup"><span data-stu-id="40192-p134">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="40192-316">Erstellen Sie den Microsoft Graph-Dienstprinzipal.</span><span class="sxs-lookup"><span data-stu-id="40192-316">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="40192-317">Nur in Office 365-REST- oder Azure AD-Graph-APIs verfügbare Funktionen</span><span class="sxs-lookup"><span data-stu-id="40192-317">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="40192-p135">Einige Funktionen sind in Microsoft Graph noch nicht verfügbar. Wenn Sie die gesuchte Funktion nicht finden, können Sie die endpunktspezifischen [Office 365-REST-APIs](https://msdn.microsoft.com/office/office365/api/api-catalog) verwenden. Für Azure Active Directory finden Sie im Blogbeitrag [Microsoft Graph oder Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) Informationen über die Features, die nur über die Azure AD-Graph-API verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="40192-p135">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

## <a name="feedback"></a><span data-ttu-id="40192-321">Feedback</span><span class="sxs-lookup"><span data-stu-id="40192-321">Feedback</span></span>

> <span data-ttu-id="40192-p136">Ihr Feedback ist uns wichtig. Nehmen Sie unter [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoftgraph) Kontakt mit uns auf.</span><span class="sxs-lookup"><span data-stu-id="40192-p136">Your feedback is important to us. Connect with us on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoftgraph).</span></span>
