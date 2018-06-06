# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="2a9c3-101">Bekannte Probleme in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a9c3-101">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="2a9c3-p101">Dieser Artikel beschreibt bekannte Probleme in Microsoft Graph. Informationen zu den neuesten Updates finden Sie im [Microsoft Graph-Änderungsprotokoll](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p101">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="2a9c3-104">Benutzer</span><span class="sxs-lookup"><span data-stu-id="2a9c3-104">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="2a9c3-105">Kein direkter Zugriff nach der Erstellung</span><span class="sxs-lookup"><span data-stu-id="2a9c3-105">No instant access after creation</span></span>

<span data-ttu-id="2a9c3-p102">Benutzer können direkt über POST in der Benutzerentität erstellt werden. Eine Office 365-Lizenz muss zunächst einem Benutzer zugewiesen werden, damit dieser Zugriff auf Office 365-Dienste erhält. Aufgrund der verteilten Art des Diensts kann es bis zu 15 Minuten dauern, bis Dateien-, Nachrichten- und Ereignisentitäten für diesen Benutzer über die Microsoft Graph-API zur Verfügung stehen. In dieser Zeit erhalten Apps als Antwort den HTTP-Fehler 404.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p102">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="2a9c3-110">Fotoeinschränkungen</span><span class="sxs-lookup"><span data-stu-id="2a9c3-110">Photo restrictions</span></span>

<span data-ttu-id="2a9c3-p103">Benutzerprofilfotos können nur gelesen und aktualisiert werden, wenn der Benutzer über ein Postfach verfügt. Darüber hinaus kann auf Fotos, die *ggf.* zuvor mithilfe der **thumbnailPhoto**-Eigenschaft (unter Verwendung der Office 365 Unified-API-Vorschau oder Azure AD Graph oder über die AD Connect-Synchronisierung) gespeichert wurden, nicht mehr über die Microsoft Graph-Eigenschaft **photo** der [user](../api-reference/v1.0/resources/user.md)-Ressource zugegriffen werden. Beim Auftreten eines Fehlers beim Lesen oder Aktualisieren eines Fotos wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p103">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](../api-reference/v1.0/resources/user.md) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```


### <a name="using-delta-query"></a><span data-ttu-id="2a9c3-114">Verwenden der Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="2a9c3-114">Using delta query</span></span>

<span data-ttu-id="2a9c3-115">Bekannte Probleme bei der Verwendung der Delta-Abfrage finden Sie im Abschnitt [Delta-Abfrage](#delta-query) in diesem Artikel.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-115">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="groups-and-microsoft-teams"></a><span data-ttu-id="2a9c3-116">Gruppen und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2a9c3-116">Groups and Microsoft Teams</span></span>

><span data-ttu-id="2a9c3-117">**Hinweis** Microsoft Teams ist derzeit nur im Beta-Endpunkt von Microsoft Graph als Vorschauversion verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-117">**Note** Microsoft Teams is currently in preview and is available only in the Microsoft Graph beta endpoint.</span></span>

### <a name="policy"></a><span data-ttu-id="2a9c3-118">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2a9c3-118">Policy</span></span>

<span data-ttu-id="2a9c3-119">Beim Erstellen und Benennen einer Office 365-Gruppe mit Microsoft Graph werden Office 365-Gruppenrichtlinien umgangen, die über Outlook Web App konfiguriert werden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-119">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="2a9c3-120">Berechtigungen für Gruppen und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2a9c3-120">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="2a9c3-p104">Microsoft Graph stellt zwei Berechtigungen (*Group.Read.All* und *Group.ReadWrite.All*) für den Zugriff auf Gruppen und Microsoft Teams zur Verfügung. Diesen Berechtigungen muss ein Administrator seine Zustimmung erteilen (anders als in der Vorschauversion).  In Zukunft sollen neue Berechtigungen für Gruppen und Teams hinzugefügt werden, für die Benutzer ihre Zustimmung erteilen können.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p104">Microsoft Graph exposes two permissions (*Group.Read.All* and *Group.ReadWrite.All*) for access to the APIs for groups and Microsoft Teams. These permissions must be consented to by an administrator (which is a change from preview).  In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="2a9c3-p105">Außerdem unterstützt nur die API für die Hauptgruppenadministration und -verwaltung den Zugriff mithilfe delegierter oder Nur-App-Berechtigungen. Alle anderen Features der Gruppen-API unterstützen nur delegierte Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p105">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="2a9c3-126">Beispiele für Gruppenfeatures, die delegierte und Nur-App-Berechtigungen unterstützen:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-126">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="2a9c3-127">Erstellen und Löschen von Gruppen</span><span class="sxs-lookup"><span data-stu-id="2a9c3-127">Creating and deleting groups</span></span>
* <span data-ttu-id="2a9c3-128">Abrufen und Aktualisieren von Gruppeneigenschaften, die zur Gruppenadministration oder -verwaltung gehören</span><span class="sxs-lookup"><span data-stu-id="2a9c3-128">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="2a9c3-129">[Verzeichniseinstellungen](../api-reference/v1.0/resources/directoryobject.md) für Gruppen, Typ und Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="2a9c3-129">Group [directory settings](../api-reference/v1.0/resources/directoryobject.md), type, and synchronization</span></span>
* <span data-ttu-id="2a9c3-130">Gruppenbesitzer und Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="2a9c3-130">Group owners and membership</span></span>

<span data-ttu-id="2a9c3-131">Beispiele für Gruppenfeatures, die nur delegierte Berechtigungen unterstützen:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-131">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="2a9c3-132">Gruppenunterhaltungen, Ereignisse, Fotos</span><span class="sxs-lookup"><span data-stu-id="2a9c3-132">Group conversations, events, photo</span></span>
* <span data-ttu-id="2a9c3-133">Externe Absender, akzeptierte oder abgelehnte Absender, Gruppenabonnement</span><span class="sxs-lookup"><span data-stu-id="2a9c3-133">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="2a9c3-134">Benutzerfavoriten und Anzahl ungesehener Elemente</span><span class="sxs-lookup"><span data-stu-id="2a9c3-134">User favorites and unseen count</span></span>
* <span data-ttu-id="2a9c3-135">Microsoft Teams-Kanäle und -Chats.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-135">Microsoft Teams channels and chats</span></span>

### <a name="teams-in-microsoft-teams-preview"></a><span data-ttu-id="2a9c3-136">Teams in Microsoft Teams (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="2a9c3-136">Teams in Microsoft Teams (preview)</span></span>

<span data-ttu-id="2a9c3-p106">Microsoft Teams und Office 365-Gruppen [haben eine ähnliche Funktionalität](../api-reference/beta/resources/teams_api_overview.md). Alle Gruppen-APIs können für Teams verwendet werden, mit der Ausnahme, dass mit der API „Gruppe erstellen“ derzeit kein Team erstellt werden kann.  In zukünftigen API-Versionen wird dies unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p106">Microsoft Teams and Office 365 groups [share similar functionality](../api-reference/beta/resources/teams_api_overview.md). All group APIs can be used with teams, with the exception that the Create group API does not currently allow you to create a team.  Future API releases will support this.</span></span>

### <a name="microsoft-teams-channels-preview"></a><span data-ttu-id="2a9c3-140">Microsoft Teams-Kanäle (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="2a9c3-140">Microsoft Teams channels (preview)</span></span>

<span data-ttu-id="2a9c3-p107">Zurzeit können Sie Kanäle lesen und erstellen, aber nicht aktualisieren oder löschen.  In zukünftigen API-Versionen wird dies unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p107">Currently, you can read and create channels, but you cannot update or delete them.  Future API releases will support this.</span></span>

### <a name="microsoft-teams-chat-threads-and-chat-messages-preview"></a><span data-ttu-id="2a9c3-143">Microsoft Teams-Chatthreads und -Chatnachrichten (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="2a9c3-143">Microsoft Teams chat threads and chat messages (preview)</span></span>

<span data-ttu-id="2a9c3-p108">Zurzeit können Sie Chatthreads in Kanälen erstellen, aber keine vorhandenen Chatthreads lesen und keine Antworten auf diese hinzufügen. Außerdem können Sie keine direkten Chats zwischen Benutzern lesen oder schreiben, die sich außerhalb des Bereichs eines Teams oder Kanals befinden.  Zukünftige API-Versionen werden über zusätzliche Funktionen in diesem Bereich verfügen.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p108">Currently, you can create chat threads in channels, but you cannot read existing chat threads or add replies to them. Also, you cannot read or write direct chats between users that are outside the scope of a team or channel.  Future API releases will add additional capabilities in this area.</span></span>

### <a name="microsoft-teams-users-list-of-joined-teams-preview"></a><span data-ttu-id="2a9c3-147">Liste der Teams, denen ein Microsoft Teams-Benutzer beigetreten ist (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="2a9c3-147">Microsoft Teams user's list of joined teams (preview)</span></span>

<span data-ttu-id="2a9c3-p109">Aktuell funktioniert das [Auflisten der Teams, denen ein Benutzer beigetreten ist](../api-reference/beta/api/user_list_joinedteams.md), nur für den Benutzer „Ich“, für den der Anrufer über [delegierte Berechtigungen](permissions_reference.md) verfügt.  In zukünftigen Versionen wird dieser Vorgang für alle angegebenen Benutzer-IDs unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p109">Currrently, [listing the teams a user has joined](../api-reference/beta/api/user_list_joinedteams.md) only works for the 'me' user for which the caller has [delegated permissions](permissions_reference.md).  Future releases will support this operation for any specified user ID.</span></span>

### <a name="adding-and-getting-attachments-of-group-posts"></a><span data-ttu-id="2a9c3-150">Hinzufügen und Abrufen von Anlagen von Gruppenbeiträgen</span><span class="sxs-lookup"><span data-stu-id="2a9c3-150">Adding and getting attachments of group posts</span></span>

<span data-ttu-id="2a9c3-p110">Durch das [Hinzufügen](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/post_post_attachments) von Anlagen zu Gruppenbeiträgen, das [Auflisten](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/post_list_attachments) und das Abrufen von Anlagen von Gruppenbeiträgen wird aktuell die Fehlermeldung „Die OData-Anforderung wird nicht unterstützt“ zurückgegeben. Für die `/v1.0`- und `/beta`-Versionen wurde eine Problemlösung entwickelt, die bis Ende Januar 2016 allgemein verfügbar sein sollte.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p110">[Adding](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/post_post_attachments) attachments to group posts, [listing](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/post_list_attachments) and getting attachments of group posts currently return the error message "The OData request is not supported." A fix has been rolled out for both the `/v1.0` and `/beta` versions, and is expected to be widely available by the end of January 2016.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="2a9c3-153">Festlegen der allowExternalSenders-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a9c3-153">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="2a9c3-154">Aktuell liegt ein Problem vor, aufgrund dessen sich die Eigenschaft **allowExternalSenders** einer Gruppe in POST- oder PATCH-Operationen nicht festlegen lässt. Das Problem tritt sowohl in `/v1.0` als auch in `/beta` auf.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-154">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="2a9c3-155">Verwenden der Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="2a9c3-155">Using delta query</span></span>

<span data-ttu-id="2a9c3-156">Bekannte Probleme bei der Verwendung der Delta-Abfrage finden Sie im Abschnitt [ Delta-Abfrage](#delta-query) in diesem Artikel.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-156">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>


## <a name="calendars"></a><span data-ttu-id="2a9c3-157">Kalender</span><span class="sxs-lookup"><span data-stu-id="2a9c3-157">Calendars</span></span>

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="2a9c3-158">Hinzufügen von und Zugreifen auf ICS-basierte Kalender im Postfach des Benutzers</span><span class="sxs-lookup"><span data-stu-id="2a9c3-158">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="2a9c3-159">Derzeit gibt es eine teilweise Unterstützung für einen Kalender, der auf einem Internet-Kalenderabonnement (ICS) basiert:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-159">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="2a9c3-160">Sie können einen ICS-basierten Kalender einem Benutzerpostfach über die Benutzeroberfläche, jedoch nicht über die Microsoft Graph-API hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-160">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="2a9c3-p111">[Das Auflisten der Kalender des Benutzers](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/user_list_calendars) ermöglicht Ihnen, die Eigenschaften **name**, **color** und **id** jedes [Kalenders](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/calendar) in der Standardkalendergruppe des Benutzers oder einer bestimmten Kalendergruppe abzurufen, einschließlich ICS-basierte Kalender. Sie können die ICS-URL in der Kalenderressource nicht speichern und nicht darauf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p111">[Listing the user's calendars](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/user_list_calendars) lets you get the **name**, **color** and **id** properties of each [calendar](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/calendar) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="2a9c3-163">Sie haben auch die Möglichkeit zum [Auflisten der Ereignisse](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/calendar_list_events) eines ICS-basierten Kalenders.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-163">You can also [list the events](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/calendar_list_events) of an ICS-based calendar.</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="2a9c3-164">Zugreifen auf einen freigegebenen Kalender</span><span class="sxs-lookup"><span data-stu-id="2a9c3-164">Accessing a shared calendar</span></span>

<span data-ttu-id="2a9c3-165">Beim Versuch, auf Ereignisse in einem Kalender zuzugreifen, der von einem anderen Benutzer mithilfe des folgenden Vorgangs freigegeben wurde:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-165">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="2a9c3-p112">Möglicherweise wird HTTP 500 mit dem Fehlercode `ErrorInternalServerTransientError` angezeigt. Der Fehler tritt aus folgendem Grund auf:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p112">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="2a9c3-168">Bisher gibt es zwei Methoden zur Implementierung der Kalenderfreigabe, die zur Unterscheidung einmal als der „alte“ Implementierungsansatz und einmal als der „neue“ Implementierungsansatz bezeichnet werden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-168">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="2a9c3-169">Der neue Ansatz ist derzeit für die Kalenderfreigabe mit Berechtigungen zum Anzeigen oder Bearbeiten verfügbar, jedoch nicht mit  aber nicht mit Berechtigungen der Stellvertretung.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-169">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="2a9c3-170">Sie können die Kalender-REST-API verwenden, um freigegebene Kalender anzuzeigen oder freizugeben, aber nur, wenn die Kalender auf die **neue** Weise freigegebenen wurden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-170">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="2a9c3-171">Sie können die Kalender-REST-API nicht verwenden, um freigegebene Kalender (oder deren Ereignisse) anzuzeigen oder freizugeben, wenn die Kalender auf die **alte** Weise freigegebenen wurden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-171">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="2a9c3-172">Wenn ein Kalender mit Berechtigungen zum Anzeigen oder Bearbeiten auf die alte Weise freigegeben wurde, können Sie dieses Problem umgehen und die Kalenderfreigabe für die Verwendung des neuen Ansatzes aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-172">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="2a9c3-173">Im Laufe der Zeit werden alle freigegebenen Kalender für die Verwendung des neuen Ansatzes automatisch in Outlook aktualisiert, einschließlich mit Berechtigungen der Stellvertretung freigegebener Kalender.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-173">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="2a9c3-174">Gehen Sie folgendermaßen vor, um einen freigegebenen Kalender für die Verwendung des neuen Ansatzes manuell zu aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-174">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="2a9c3-175">Der Empfänger entfernt den Kalender, der zuvor für diesen freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-175">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="2a9c3-176">Der Besitzer des Kalenders gibt den Kalender erneut in Outlook im Web, Outlook für iOS oder Outlook für Android frei.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-176">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="2a9c3-p114">Der Empfänger akzeptiert den freigegebenen Kalender mithilfe von Outlook im Web erneut. (Zukünftig können auch andere Outlook-Clients verwendet werden.)</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p114">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="2a9c3-179">Der Empfänger überprüft, ob der Kalender auf die neue Weise erfolgreich erneut freigegeben wurde und in Outlook für iOS oder in Outlook für Android angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-179">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="2a9c3-p115">Ein für Sie mit dem neuen Ansatz freigegebener Kalender wird genau wie jeder andere Kalender in Ihrem Postfach angezeigt. Sie können die Kalender-REST-API verwenden, um Ereignisse im freigegebenen Kalender so anzuzeigen oder zu bearbeiten, als wäre es Ihr eigener Kalender. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p115">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```


## <a name="contacts"></a><span data-ttu-id="2a9c3-183">Kontakte</span><span class="sxs-lookup"><span data-stu-id="2a9c3-183">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="2a9c3-184">Organisationskontakte nur in Betaversion verfügbar</span><span class="sxs-lookup"><span data-stu-id="2a9c3-184">Organization contacts available in only beta</span></span>

<span data-ttu-id="2a9c3-p116">Derzeit werden nur persönliche Kontakten unterstützt. Organisationskontakte werden derzeit nicht in `/v1.0` unterstützt, sind jedoch in `/beta` vorhanden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p116">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="2a9c3-187">Standardordner für Kontakte</span><span class="sxs-lookup"><span data-stu-id="2a9c3-187">Default contacts folder</span></span>

<span data-ttu-id="2a9c3-188">In der `/v1.0`-Version enthält `GET /me/contactFolders` keinen Standardordner für Kontakte des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-188">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="2a9c3-p117">Es wird ein Update zur Verfügung gestellt. In der Zwischenzeit können Sie die folgende [list contacts](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/user_list_contacts)-Abfrage und die **parentFolderId**-Eigenschaft als Problemumgehung verwenden, um die ID des Standardordners für Kontakte abzurufen:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p117">A fix will be made available. Meanwhile, you can use the following [list contacts](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/user_list_contacts) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="2a9c3-191">In der obigen Abfrage gilt Folgendes:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-191">In the above query:</span></span>

1. <span data-ttu-id="2a9c3-192">`/me/contacts?$top=1` ruft die Eigenschaften eines [Kontakts](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/contact) im Standardordner für Kontakte ab.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-192">`/me/contacts?$top=1` gets the properties of a [contact](http://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/contact) in the default contacts folder.</span></span>
2. <span data-ttu-id="2a9c3-193">Das Anfügen von `&$select=parentFolderId` gibt nur die **parentFolderId**-Eigenschaft des Kontakts zurück, also die ID des Standardordners für Kontakte.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-193">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="2a9c3-194">Zugreifen auf Kontakte über einen Kontakteordner in der Betaversion</span><span class="sxs-lookup"><span data-stu-id="2a9c3-194">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="2a9c3-195">In der Version `/beta` liegt aktuell ein Problem vor, aufgrund dessen der Zugriff auf einen [Kontakt](../api-reference/beta/resources/contact.md) über die Angabe seines übergeordneten Ordners in der REST-Anforderungs-URL in den folgenden 2 Szenarien nicht möglich ist:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-195">In the `/beta` version, there is currently an issue that prevents accessing a [contact](../api-reference/beta/resources/contact.md) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="2a9c3-196">Zugreifen auf einen Kontakt über ein [contactFolder](../api-reference/beta/resources/contactfolder.md)-Objekt höchster Ebene des Benutzers</span><span class="sxs-lookup"><span data-stu-id="2a9c3-196">Accessing a contact from a top level [contactFolder](../api-reference/beta/resources/contactfolder.md) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="2a9c3-p118">Zugreifen auf einen Kontakt in einem untergeordneten Ordner eines **contactFolder**-Objekts  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p118">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="2a9c3-199">Alternativ können Sie den Kontakt ganz einfach [per GET-Befehl abrufen](../api-reference/beta/api/contact_get.md), indem Sie seine ID wie unten gezeigt angeben. Das funktioniert, weil der Befehl „GET /contacts“ in der Version `/beta` auf alle Kontakte im Postfach des Benutzers angewendet wird:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-199">As an alternative, you can simply [get](../api-reference/beta/api/contact_get.md) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="2a9c3-200">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2a9c3-200">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="2a9c3-201">Der comment-Parameter für das Erstellen eines Entwurfs</span><span class="sxs-lookup"><span data-stu-id="2a9c3-201">The comment parameter for creating a draft</span></span>

<span data-ttu-id="2a9c3-202">Der comment-Parameter für das Erstellen eines Antwort- oder Weiterleitungsentwurfs ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) wird nicht Teil des Textkörpers des resultierenden Nachrichtenentwurfs.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-202">The **comment** parameter for creating a reply or forward draft ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) does not become part of the body of the resultant message draft.</span></span>

## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="2a9c3-203">Laufwerke, Dateien und Streamen von Inhalten</span><span class="sxs-lookup"><span data-stu-id="2a9c3-203">Drives, files and content streaming</span></span>

* <span data-ttu-id="2a9c3-204">Beim ersten Zugriff auf ein persönliches Benutzerlaufwerk über Microsoft Graph tritt ein 401-Fehler auf, wenn der Benutzer seine persönliche Website noch nicht in einem Browser aufgerufen hat.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-204">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="2a9c3-205">Einschränkungen für Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2a9c3-205">Query parameter limitations</span></span>

* <span data-ttu-id="2a9c3-206">Mehrere Namespaces werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-206">Multiple namespaces are not supported</span></span>
* <span data-ttu-id="2a9c3-207">GET-Anforderungen für `$ref` und Umwandlung wird für Benutzer, Gruppen, Geräte, Dienstprinzipale und Anwendungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-207">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="2a9c3-p119">`@odata.bind` wird nicht unterstützt.  Ein Entwickler kann daher `Accepted` oder `RejectedSenders` für eine Gruppe nicht ordnungsgemäß festlegen.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p119">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the `Accepted` or `RejectedSenders` on a group.</span></span>
* <span data-ttu-id="2a9c3-210">`@odata.id` ist bei Nicht-Aufnahmenavigationen (z. B. Nachrichten) nicht vorhanden, wenn minimale Metadaten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-210">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata</span></span>
* <span data-ttu-id="2a9c3-211">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-211"></span></span>
  * <span data-ttu-id="2a9c3-212">Keine Unterstützung für `nextLink`.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-212">No support for `nextLink`</span></span>
  * <span data-ttu-id="2a9c3-213">Keine Unterstützung für mehr als eine Erweiterungsebene.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-213">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="2a9c3-214">Keine Unterstützung mit zusätzlichen Parametern (`$filter`, `$select`).</span><span class="sxs-lookup"><span data-stu-id="2a9c3-214">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="2a9c3-215">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-215"></span></span>
  * <span data-ttu-id="2a9c3-216">Filter werden vom `/attachments`-Endpunkt nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-216">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="2a9c3-217">Falls vorhanden, wird der `$filter`-Parameter ignoriert.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-217">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="2a9c3-218">Arbeitsauslastungsübergreifende Filter werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-218">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="2a9c3-219">`$search`:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-219"></span></span>
  * <span data-ttu-id="2a9c3-220">Volltextsuche ist nur für einige Entitäten wie Nachrichten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-220">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="2a9c3-221">Arbeitsauslastungsübergreifende Suche wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-221">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="2a9c3-222">Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="2a9c3-222">Delta query</span></span>

* <span data-ttu-id="2a9c3-223">OData-Kontext wird beim Nachverfolgen von Änderungen an Beziehungen manchmal falsch zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-223">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="2a9c3-224">Schemaerweiterungen (Legacy) werden nicht mit $select-Anweisung, sondern ohne $select zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-224">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="2a9c3-225">Clients können keine Änderungen an offenen Erweiterungen oder registrierten Schemaerweiterungen nachverfolgen.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-225">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="2a9c3-226">Änderungen an der application- und servicePrincipal-API</span><span class="sxs-lookup"><span data-stu-id="2a9c3-226">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="2a9c3-p121">Es gibt Änderungen an den [application](../api-reference/beta/resources/application.md)- und [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md)-Entitäten, die derzeit entwickelt werden. Nachfolgend finden Sie eine Zusammenfassung aktueller Einschränkungen und API-Features, die derzeit entwickelt werden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p121">There are changes to the [application](../api-reference/beta/resources/application.md) and [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="2a9c3-229">Aktuelle Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-229">Current limitations:</span></span>

* <span data-ttu-id="2a9c3-230">Einige Anwendungseigenschaften (z. B. appRoles und addIns) sind erst verfügbar, wenn alle Änderungen abgeschlossen sind.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-230">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="2a9c3-231">Es können nur Apps mit mehreren Mandanten registriert werden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-231">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="2a9c3-232">Das Aktualisieren von Apps ist auf Apps beschränkt, die nach dem anfänglichen Beta-Update registriert wurden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-232">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="2a9c3-233">Azure Active Directory-Benutzer können Apps registrieren und weitere Besitzer hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-233">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="2a9c3-234">Unterstützung für OpenID Connect und OAuth-Protokolle.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-234">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="2a9c3-235">Richtlinienzuweisungen zu einer App schlagen fehl.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-235">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="2a9c3-236">Vorgänge mit ownedObjects, die die appId erfordern, schlagen fehl (z. B. users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="2a9c3-236">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="2a9c3-237">In der Entwicklung:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-237">In development:</span></span>

* <span data-ttu-id="2a9c3-238">Die Möglichkeit, Apps mit nur einem Mandanten zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-238">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="2a9c3-239">Updates für servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-239">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="2a9c3-240">Migration von vorhandenen Azure AD-Apps zum aktualisierten Modell.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-240">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="2a9c3-241">Unterstützung für appRoles, vorab autorisierte Clients, optionale Ansprüche, Gruppenmitgliedschaftsansprüche und Branding</span><span class="sxs-lookup"><span data-stu-id="2a9c3-241">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="2a9c3-242">Benutzer eines Microsoft-Kontos (MSA-Benutzer) können Apps registrieren.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-242">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="2a9c3-243">Unterstützung für SAML und WsFed-Protokolle.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-243">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="2a9c3-244">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="2a9c3-244">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="2a9c3-245">Die Änderungsnachverfolgung wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-245">Change tracking is not supported</span></span>

<span data-ttu-id="2a9c3-246">Die Änderungsnachverfolgung (Delta-Abfrage) wird für Eigenschaften von offenen Erweiterungen oder Schemaerweiterungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-246">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="2a9c3-247">Gleichzeitiges Erstellen einer Ressource und einer offenen Erweiterung</span><span class="sxs-lookup"><span data-stu-id="2a9c3-247">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="2a9c3-p122">Wenn Sie eine Instanz von Ressourcen des Typs **administrativeUnit**, **device**, **group**, **organization** oder **user** erstellen, können Sie nicht gleichzeitig eine offene Erweiterung angeben. Sie müssen zuerst die Instanz erstellen und dann eine ``POST``-Anforderung auf diese Instanz anwenden, in der Sie die Daten der offenen Erweiterung angeben.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p122">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="2a9c3-250">Erstellen einer Ressourceninstanz und Hinzufügen von Schemaerweiterungsdaten zur gleichen Zeit</span><span class="sxs-lookup"><span data-stu-id="2a9c3-250">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="2a9c3-251">Sie können während des Vorgangs zum Erstellen einer **contact**-, **event**-, **message**- oder **post**-Instanz nicht gleichzeitig eine Schemaerweiterung festlegen.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-251">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="2a9c3-252">Sie müssen zuerst die Ressourceninstanz erstellen und dann einen `PATCH` für die betreffende Instanz durchführen, um eine Schemaerweiterung und benutzerdefinierte Daten hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-252">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="2a9c3-253">Grenzwert von 100 zulässigen Werten für Schemaerweiterungseigenschaften pro Ressourceninstanz.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-253">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="2a9c3-254">Für Verzeichnisressourcen wie **device**, **group** und **user** gilt aktuell: Für eine Ressourceninstanz dürfen maximal 100 Eigenschaftswerte von Schemaerweiterungen festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-254">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

## <a name="json-batching"></a><span data-ttu-id="2a9c3-255">JSON-Batchverarbeitung</span><span class="sxs-lookup"><span data-stu-id="2a9c3-255">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="2a9c3-256">Keine geschachtelter Batch</span><span class="sxs-lookup"><span data-stu-id="2a9c3-256">No nested batch</span></span>

<span data-ttu-id="2a9c3-257">JSON-Batchanforderungen dürfen keine geschachtelten Batchanforderungen enthalten.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-257">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="2a9c3-258">Alle einzelnen Anforderungen müssen synchron sein.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-258">All individual requests must be synchronous</span></span>

<span data-ttu-id="2a9c3-p124">Alle in einer Batchanforderung enthaltenen Anforderungen müssen synchron ausgeführt werden. Falls vorhanden, wird die `respond-async`-Präferenz ignoriert.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p124">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="2a9c3-261">Keine Transaktionen</span><span class="sxs-lookup"><span data-stu-id="2a9c3-261">No transactions</span></span>

<span data-ttu-id="2a9c3-p125">Microsoft Graph unterstützt derzeit keine Transaktionsverarbeitung von einzelnen Anforderungen. Die `atomicityGroup`-Eigenschaft von einzelnen Anforderungen wird ignoriert.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p125">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="2a9c3-264">URIs müssen relativ sein</span><span class="sxs-lookup"><span data-stu-id="2a9c3-264">URIs must be relative</span></span>

<span data-ttu-id="2a9c3-p126">Geben Sie in Batchanforderungen immer relative URIs an. Microsoft Graph macht daraus dann mithilfe des in der Batch-URL enthaltenen Versionsendpunkts absolute URLs.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p126">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="2a9c3-267">Beschränkung der Batchgröße</span><span class="sxs-lookup"><span data-stu-id="2a9c3-267">Limit on batch size</span></span>

<span data-ttu-id="2a9c3-268">JSON-Batchanforderungen sind derzeit auf 20 einzelne Anforderungen beschränkt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-268">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="2a9c3-269">Vereinfachte Abhängigkeiten</span><span class="sxs-lookup"><span data-stu-id="2a9c3-269">Simplified dependencies</span></span>

<span data-ttu-id="2a9c3-p127">Einzelne Anforderungen können von anderen einzelnen Anforderungen abhängen. Derzeit können Anforderungen nur von einer einzigen anderen Anforderung abhängen und müssen einem der folgenden drei Muster entsprechen:</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p127">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="2a9c3-272">Parallel: Eine einzelne Anforderung gibt eine Abhängigkeit in der `dependsOn`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-272">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="2a9c3-273">Seriell: Alle einzelnen Anforderungen hängen von der vorherigen einzelnen Anforderung ab.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-273">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="2a9c3-274">Gleich: Alle einzelnen Anforderungen, die eine Abhängigkeit in der `dependsOn`-Eigenschaft angeben, geben die gleiche Abhängigkeit an.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-274">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="2a9c3-275">In der weiteren Entwicklung der JSON-Batchverarbeitung werden diese Einschränkungen entfernt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-275">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="2a9c3-276">Apps vom Cloudlösungsanbieter</span><span class="sxs-lookup"><span data-stu-id="2a9c3-276">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="2a9c3-277">Apps vom Cloudlösungsanbieter müssen den Azure AD-Endpunkt verwenden</span><span class="sxs-lookup"><span data-stu-id="2a9c3-277">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="2a9c3-p128">CSP-Apps (Cloud-Lösungsanbieter) müssen Token von den Azure AD (v1)-Endpunkten erwerben, um Microsoft Graph erfolgreich in ihren partnerverwalteten Kunden aufrufen zu können. Derzeit wird der Erwerb eines Tokens über den neueren Azure AD v2.0-Endpunkt nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p128">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="2a9c3-280">Eine Vorabgenehmigung für Apps vom Cloudlösungsanbieter funktioniert bei einigen Kundenmandanten nicht</span><span class="sxs-lookup"><span data-stu-id="2a9c3-280">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="2a9c3-281">Unter bestimmten Umständen funktioniert die Vorabgenehmigung für Apps vom Cloudlösungsanbieter bei einigen Kundenmandanten nicht.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-281">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="2a9c3-282">Für Apps, die delegierte Berechtigungen verwenden, wird bei der ersten Verwendung der App mit einem neuen Kundenmandanten möglicherweise der folgende Fehler nach der Anmeldung angezeigt: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-282">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="2a9c3-283">Für Apps, die Anwendungsberechtigungen verwenden, kann Ihre App ein Token erfassen, beim Aufrufen von Microsoft Graph wird jedoch unerwartet die Meldung angezeigt, dass der Zugriff verweigert wurde.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-283">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="2a9c3-284">Wir arbeiten daran, dieses Problem so schnell wie möglich zu lösen, damit die Vorabgenehmigung für alle Kundenmandanten funktioniert.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-284">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="2a9c3-285">In der Zwischenzeit können Sie die folgende Problemumgehung verwenden, um die Entwicklung und das Testen nicht zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-285">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="2a9c3-p129">**HINWEIS:** Dies ist keine dauerhafte Lösung und soll nur dazu dienen, die Entwicklung nicht zu blockieren.  Diese Problemumgehung ist nicht mehr erforderlich, nachdem das zuvor erwähnte Problem behoben wurde.  Diese Problemumgehung muss nicht rückgängig gemacht werden, nachdem die Korrektur vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p129">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="2a9c3-p130">Öffnen Sie eine Azure AD v2-PowerShell-Sitzung, und stellen Sie eine Verbindung mit Ihrem `customer`-Mandanten her, indem Sie Ihre Administrator-Anmeldeinformationen in das Anmeldefenster eingeben. Sie können Azure AD PowerShell V2 [hier](https://www.powershellgallery.com/packages/AzureAD) herunterladen und installieren.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p130">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="2a9c3-291">Erstellen Sie den Microsoft Graph-Dienstprinzipal.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-291">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="2a9c3-292">Nur in Office 365-REST- oder Azure AD-Graph-APIs verfügbare Funktionen</span><span class="sxs-lookup"><span data-stu-id="2a9c3-292">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="2a9c3-p131">Einige Funktionen sind in Microsoft Graph noch nicht verfügbar. Wenn Sie die gesuchte Funktion nicht finden, können Sie die endpunktspezifischen [Office 365-REST-APIs](https://msdn.microsoft.com/de-DE/office/office365/api/api-catalog) verwenden. Für Azure Active Directory finden Sie im Blogbeitrag [Microsoft Graph oder Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) Informationen über die Features, die nur über die Azure AD-Graph-API verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p131">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/de-DE/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

## <a name="feedback"></a><span data-ttu-id="2a9c3-296">Feedback</span><span class="sxs-lookup"><span data-stu-id="2a9c3-296">Feedback</span></span>

> <span data-ttu-id="2a9c3-p132">Ihr Feedback ist uns wichtig. Nehmen Sie unter [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph) Kontakt mit uns auf.</span><span class="sxs-lookup"><span data-stu-id="2a9c3-p132">Your feedback is important to us. Connect with us on [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph).</span></span>
