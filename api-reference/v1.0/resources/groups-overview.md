# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="a253c-101">Arbeiten mit Gruppen in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a253c-101">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="a253c-102">Gruppen sind Auflistungen von [Benutzern](user.md) und anderen Hauptbenutzern, die den Zugriff auf Ressourcen in Microsoft-Diensten oder in Ihrer App gemeinsam nutzen.</span><span class="sxs-lookup"><span data-stu-id="a253c-102">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="a253c-103">Microsoft Graph enthält APIs, die Sie zum Erstellen und Verwalten von verschiedenen Typen von Gruppen und Gruppenfunktionalitäten entsprechend Ihrem Szenario verwenden können.</span><span class="sxs-lookup"><span data-stu-id="a253c-103">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="a253c-104">Für alle gruppenbezogenen Vorgänge in Microsoft Graph ist die Zustimmung durch einen Administrator erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a253c-104">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="a253c-105">**Hinweis**: Gruppen können nur über Geschäfts- oder Schulkonten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="a253c-105">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="a253c-106">Persönliche Microsoft-Konten unterstützen keine Gruppen.</span><span class="sxs-lookup"><span data-stu-id="a253c-106">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="a253c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="a253c-107">Type</span></span>              | <span data-ttu-id="a253c-108">Anwendungsfall</span><span class="sxs-lookup"><span data-stu-id="a253c-108">Use case</span></span> | <span data-ttu-id="a253c-109">groupType</span><span class="sxs-lookup"><span data-stu-id="a253c-109">groupType</span></span> | <span data-ttu-id="a253c-110">E-Mail-aktiviert</span><span class="sxs-lookup"><span data-stu-id="a253c-110">mail-enabled</span></span> | <span data-ttu-id="a253c-111">Mit aktivierter Sicherheit</span><span class="sxs-lookup"><span data-stu-id="a253c-111">security-enabled</span></span> | <span data-ttu-id="a253c-112">Erstellung über API möglich?</span><span class="sxs-lookup"><span data-stu-id="a253c-112">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="a253c-113">Office 365-Gruppen</span><span class="sxs-lookup"><span data-stu-id="a253c-113">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="a253c-114">Ermöglicht die Zusammenarbeit von Benutzern mit freigegebenen Microsoft-Onlineressourcen.</span><span class="sxs-lookup"><span data-stu-id="a253c-114">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="a253c-115">Ja</span><span class="sxs-lookup"><span data-stu-id="a253c-115">Yes</span></span> |
| [<span data-ttu-id="a253c-116">Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="a253c-116">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="a253c-117">Steuern des Benutzerzugriffs auf Ressourcen innerhalb der App.</span><span class="sxs-lookup"><span data-stu-id="a253c-117">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="a253c-118">Ja</span><span class="sxs-lookup"><span data-stu-id="a253c-118">Yes</span></span> |
| [<span data-ttu-id="a253c-119">E-Mail-aktivierte Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="a253c-119">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="a253c-120">Steuern des Benutzerzugriffs auf Ressourcen innerhalb der App mit einem freigegebenen Gruppenpostfach.</span><span class="sxs-lookup"><span data-stu-id="a253c-120">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="a253c-121">Nein</span><span class="sxs-lookup"><span data-stu-id="a253c-121">No</span></span> |
| <span data-ttu-id="a253c-122">Verteilergruppen</span><span class="sxs-lookup"><span data-stu-id="a253c-122">Distribution groups</span></span> | <span data-ttu-id="a253c-123">Verteilen von E-Mail-Nachrichten an die Mitglieder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="a253c-123">Distributing mail to the members of the group.</span></span> <span data-ttu-id="a253c-124">Es wird empfohlen, dass Sie aufgrund der vielfältigeren Ressourcen Office 365-Gruppen verwenden.</span><span class="sxs-lookup"><span data-stu-id="a253c-124">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="a253c-125">Nein</span><span class="sxs-lookup"><span data-stu-id="a253c-125">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="a253c-126">Office 365-Gruppen</span><span class="sxs-lookup"><span data-stu-id="a253c-126">Office 365 groups</span></span>
<span data-ttu-id="a253c-127">Die Leistungsfähigkeit von Office 365-Gruppen liegt an der Zusammenarbeitsfunktion, die ideal für Personen geeignet ist, die an einem Projekt oder in einem Team zusammenarbeiten.</span><span class="sxs-lookup"><span data-stu-id="a253c-127">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="a253c-128">Diese werden mit Ressourcen erstellt, die Mitglieder der Gruppe gemeinsam verwenden, darunter:</span><span class="sxs-lookup"><span data-stu-id="a253c-128">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="a253c-129">Outlook-Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="a253c-129">Outlook conversations</span></span>
- <span data-ttu-id="a253c-130">Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="a253c-130">Outlook calendar</span></span>
- <span data-ttu-id="a253c-131">SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="a253c-131">SharePoint files</span></span>
- <span data-ttu-id="a253c-132">OneNote-Notizbuch</span><span class="sxs-lookup"><span data-stu-id="a253c-132">OneNote notebook</span></span>
- <span data-ttu-id="a253c-133">SharePoint-Teamwebsite</span><span class="sxs-lookup"><span data-stu-id="a253c-133">SharePoint team site</span></span>
- <span data-ttu-id="a253c-134">Planner-Pläne</span><span class="sxs-lookup"><span data-stu-id="a253c-134">Planner plans</span></span>
- <span data-ttu-id="a253c-135">Intune-Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="a253c-135">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="a253c-136">Beispiel einer Gruppe in Outlook</span><span class="sxs-lookup"><span data-stu-id="a253c-136">Group in Outlook example</span></span>

<span data-ttu-id="a253c-137">Es folgt eine JSON-Darstellung von Gruppen in Outlook.</span><span class="sxs-lookup"><span data-stu-id="a253c-137">The following is a JSON representation of groups in Outlook.</span></span> 

```http

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "4c5ee71b-e6a5-4343-9e2c-4244bc7e0938",
    "deletedDateTime": null,
    "classification": "MBI",
    "createdDateTime": "2016-08-23T14:46:56Z",
    "description": "This is a group in Outlook",
    "displayName": "OutlookGroup101",
    "groupTypes": [
        "Unified"
    ],
    "mail": "outlookgroup101@service.microsoft.com",
    "mailEnabled": true,
    "mailNickname": "outlookgroup101",
    "preferredLanguage": null,
    "proxyAddresses": [
        "smtp:outlookgroup101@microsoft.onmicrosoft.com",
        "SMTP:outlookgroup101@service.microsoft.com"
    ],
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```
<span data-ttu-id="a253c-138">Weitere Informationen zu Office 365-Gruppen und der Administratorerfahrung finden Sie unter [Weitere Informationen zu Gruppen in Office 365](https://support.office.com/de-DE/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="a253c-138">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/de-DE/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="a253c-139">Sicherheitsgruppen und E-Mail-aktivierte Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="a253c-139">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="a253c-140">Sicherheitsgruppen sind für das Steuern des Benutzerzugriffs auf Ressourcen gedacht.</span><span class="sxs-lookup"><span data-stu-id="a253c-140">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="a253c-141">Durch Überprüfen, ob ein Benutzer ein Mitglied einer Sicherheitsgruppe ist, kann Ihre App Autorisierungsentscheidungen treffen, wenn dieser Benutzer versucht, auf sichere Ressourcen in Ihrer App zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="a253c-141">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="a253c-142">Sicherheitsgruppen können Benutzer und andere Sicherheitsgruppen als Mitglieder haben.</span><span class="sxs-lookup"><span data-stu-id="a253c-142">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="a253c-143">E-Mail-aktivierte Sicherheitsgruppen werden auf die gleiche Weise wie Sicherheitsgruppen verwendet, weisen jedoch das zusätzliche Feature eines freigegebenen Postfachs für die Gruppen auf.</span><span class="sxs-lookup"><span data-stu-id="a253c-143">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="a253c-144">E-Mail-aktivierte Sicherheitsgruppen können nicht über die API erstellt werden, aber andere Gruppenvorgänge funktionieren weiterhin.</span><span class="sxs-lookup"><span data-stu-id="a253c-144">Mail-enabled security groups can't be created through the API, but other group operations will still work here.</span></span>  <span data-ttu-id="a253c-145">E-Mail-aktivierte Sicherheitsgruppen sind schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a253c-145">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="a253c-146">Weitere Informationen finden Sie im Exchange-Artikel  [Verwalten von E-Mail-aktivierten Sicherheitsgruppen](https://technet.microsoft.com/de-DE/library/bb123521%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a253c-146">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/de-DE/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="a253c-147">Beispiel für eine Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="a253c-147">Security group example</span></span>

<span data-ttu-id="a253c-148">Es folgt eine JSON-Darstellung einer Sicherheitsgruppe.</span><span class="sxs-lookup"><span data-stu-id="a253c-148">The following is a JSON representation of a security group.</span></span> 

```http
{
    "@odata.type": "#microsoft.graph.group",
    "id": "f87faa71-57a8-4c14-91f0-517f54645106",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2016-07-20T09:21:23Z",
    "description": "This group is a Security Group",
    "displayName": "SecurityGroup101",
    "groupTypes": [],
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "",
    "preferredLanguage": null,
    "proxyAddresses": [],
    "securityEnabled": true
}
```
## <a name="dynamic-membership"></a><span data-ttu-id="a253c-149">Dynamische Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="a253c-149">Dynamic membership</span></span> 

<span data-ttu-id="a253c-150">Alle Typen von Gruppen können Regeln für dynamische Mitgliedschaft aufweisen, die automatisch Mitglieder zu der Gruppe basierend auf den Benutzereigenschaften hinzufügen oder darauf entfernen.</span><span class="sxs-lookup"><span data-stu-id="a253c-150">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="a253c-151">Die Gruppe „Marketing-Mitarbeiter“ würde beispielsweise jeden Benutzer einschließen, für den die department-Eigenschaft auf „Marketing“ festgelegt ist, sodass neue Marketing-Mitarbeiter automatisch zu der Gruppe hinzugefügt werden, und Mitarbeiter, die die Abteilung verlassen, automatisch aus der Gruppe entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="a253c-151">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="a253c-152">Diese Regel kann im Feld „membershipRule“ während der Erstellung von Gruppen als `"membershipRule": 'user.department -eq "Marketing"'` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="a253c-152">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="a253c-153">GroupType muss auch `"DynamicMembership"` umfassen.</span><span class="sxs-lookup"><span data-stu-id="a253c-153">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="a253c-154">Die folgende Anforderung erstellt eine neue Office 365-Gruppe für die Marketing-Mitarbeiter:</span><span class="sxs-lookup"><span data-stu-id="a253c-154">The following request creates a new Office 365 group for the marketing employees:</span></span> 

```http
POST https://graph.microsoft.com/beta/groups
{
    "description": "Marketing department folks",
    "displayName": "Marketing department",
    "groupTypes": [
        "Unified",
        "DynamicMembership"
    ],
    "mailEnabled": true,
    "mailNickname": "marketing",
    "securityEnabled": false,
    "membershipRule": 'user.department -eq "Marketing"',
    "membershipRuleProcessingState": "on"
}
```

<span data-ttu-id="a253c-155">Weitere Informationen zum Verfassen von membershipRules finden Sie unter [Erstellen von attributbasierten Regeln für dynamische Gruppenmitgliedschaft in Azure Active Directory](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="a253c-155">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="a253c-156">**Hinweis**: Regeln für dynamische Mitgliedschaft erfordern eine Lizenz vom Mandanten auf der Ebene [Azure Active Directory Premium P1](https://azure.microsoft.com/de-DE/pricing/details/active-directory/) oder höher.</span><span class="sxs-lookup"><span data-stu-id="a253c-156">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/de-DE/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="a253c-157">Andere Arten von Gruppen</span><span class="sxs-lookup"><span data-stu-id="a253c-157">Other types of groups</span></span>

<span data-ttu-id="a253c-158">Office 365-Gruppen in Yammer werden verwendet, um die Zusammenarbeit von Benutzern über Yammer-Beiträge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="a253c-158">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="a253c-159">Diese Art von Gruppe kann über eine Leseanforderung zurückgegeben werden, auf die Beiträge kann jedoch nicht über die API zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="a253c-159">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="a253c-160">Wenn Yammer-Beiträge und Unterhaltungs-Feeds für eine Gruppe aktiviert sind, werden standardmäßige Office 365-Gruppenunterhaltungen deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="a253c-160">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="a253c-161">Weitere Informationen finden Sie unter [Yammer-Entwickler-API Dokumente](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="a253c-161">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="a253c-162">Allgemeine Anwendungsfälle</span><span class="sxs-lookup"><span data-stu-id="a253c-162">Common use cases</span></span>

<span data-ttu-id="a253c-163">Mit Microsoft Graph können Sie die folgenden allgemeinen Vorgänge ausführen.</span><span class="sxs-lookup"><span data-stu-id="a253c-163">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="a253c-164">**Anwendungsfälle**</span><span class="sxs-lookup"><span data-stu-id="a253c-164">**Use cases**</span></span>  | <span data-ttu-id="a253c-165">**REST-Ressourcen**</span><span class="sxs-lookup"><span data-stu-id="a253c-165">**REST resources**</span></span> | <span data-ttu-id="a253c-166">**Siehe auch**</span><span class="sxs-lookup"><span data-stu-id="a253c-166">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="a253c-167">**Gruppenobjekt und Methoden**</span><span class="sxs-lookup"><span data-stu-id="a253c-167">**Group object and methods**</span></span> | | |
| <span data-ttu-id="a253c-168">Neue Gruppen erstellen, vorhandene Gruppen abrufen, die Eigenschaften für Gruppe aktualisieren und Gruppen löschen.</span><span class="sxs-lookup"><span data-stu-id="a253c-168">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="a253c-169">Derzeit können nur Sicherheitsgruppen und Gruppen in Outlook über die API erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="a253c-169">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="a253c-170">Gruppe</span><span class="sxs-lookup"><span data-stu-id="a253c-170">group</span></span>](group.md) | [<span data-ttu-id="a253c-171">Neue Gruppen erstellen</span><span class="sxs-lookup"><span data-stu-id="a253c-171">Create new groups</span></span>](../api/group_post_groups.md) <br/> [<span data-ttu-id="a253c-172">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="a253c-172">List groups</span></span>](../api/group_list.md) <br/> [<span data-ttu-id="a253c-173">Gruppen aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a253c-173">Update groups</span></span>](../api/group_update.md) <br/> [<span data-ttu-id="a253c-174">Gruppen löschen</span><span class="sxs-lookup"><span data-stu-id="a253c-174">Delete groups</span></span>](../api/group_delete.md) |
| <span data-ttu-id="a253c-175">**Methoden für Gruppenmitgliedschaft**</span><span class="sxs-lookup"><span data-stu-id="a253c-175">**Group membership methods**</span></span> | | |
| <span data-ttu-id="a253c-176">Mitglieder einer Gruppe auflisten und Mitglieder hinzufügen oder entfernen.</span><span class="sxs-lookup"><span data-stu-id="a253c-176">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="a253c-177">user</span><span class="sxs-lookup"><span data-stu-id="a253c-177">user</span></span>](user.md) <br/> [<span data-ttu-id="a253c-178">Gruppe</span><span class="sxs-lookup"><span data-stu-id="a253c-178">group</span></span>](group.md)| [<span data-ttu-id="a253c-179">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="a253c-179">List members</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="a253c-180">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="a253c-180">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="a253c-181">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="a253c-181">Remove member</span></span>](../api/group_delete_members.md)|
| <span data-ttu-id="a253c-182">Bestimmen, ob ein Benutzer Mitglied einer Gruppe ist, alle Gruppen abrufen, bei denen der Benutzer Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="a253c-182">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="a253c-183">user</span><span class="sxs-lookup"><span data-stu-id="a253c-183">user</span></span>](user.md) <br/> [<span data-ttu-id="a253c-184">Gruppe</span><span class="sxs-lookup"><span data-stu-id="a253c-184">group</span></span>](group.md)| [<span data-ttu-id="a253c-185">Mitgliedergruppen prüfen</span><span class="sxs-lookup"><span data-stu-id="a253c-185">Check member groups</span></span>](../api/group_checkmembergroups.md) <br/> [<span data-ttu-id="a253c-186">Mitgliedergruppen abrufen</span><span class="sxs-lookup"><span data-stu-id="a253c-186">Get member groups</span></span>](../api/group_getmembergroups.md)|
| <span data-ttu-id="a253c-187">Besitzer einer Gruppe auflisten und Besitzer hinzufügen oder entfernen.</span><span class="sxs-lookup"><span data-stu-id="a253c-187">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="a253c-188">Benutzer</span><span class="sxs-lookup"><span data-stu-id="a253c-188">user</span></span>](user.md) <br/> [<span data-ttu-id="a253c-189">Gruppe</span><span class="sxs-lookup"><span data-stu-id="a253c-189">group</span></span>](group.md)| [<span data-ttu-id="a253c-190">Besitzer auflisten</span><span class="sxs-lookup"><span data-stu-id="a253c-190">List owners</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="a253c-191">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="a253c-191">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="a253c-192">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="a253c-192">Remove member</span></span>](../api/group_delete_members.md)|
