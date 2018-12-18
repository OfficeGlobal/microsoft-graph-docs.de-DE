---
title: Arbeiten mit Gruppen in Microsoft Graph
description: Gruppen sind Auflistungen von Benutzern und anderen Hauptbenutzern, die den Zugriff auf Ressourcen in Microsoft-Diensten oder in Ihrer App gemeinsam nutzen. Microsoft Graph enthält APIs, die Sie zum Erstellen und Verwalten von verschiedenen Typen von Gruppen und Gruppenfunktionalitäten entsprechend Ihrem Szenario verwenden können. Für alle gruppenbezogenen Vorgänge in Microsoft Graph ist die Zustimmung durch einen Administrator erforderlich.
author: dkershaw10
ms.openlocfilehash: f3d18fd2ebf579c878e50bfae66e3987b6ef1a84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301687"
---
# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="8a575-105">Arbeiten mit Gruppen in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a575-105">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="8a575-106">Gruppen sind Auflistungen von [Benutzern](user.md) und anderen Hauptbenutzern, die den Zugriff auf Ressourcen in Microsoft-Diensten oder in Ihrer App gemeinsam nutzen.</span><span class="sxs-lookup"><span data-stu-id="8a575-106">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="8a575-107">Microsoft Graph enthält APIs, die Sie zum Erstellen und Verwalten von verschiedenen Typen von Gruppen und Gruppenfunktionalitäten entsprechend Ihrem Szenario verwenden können.</span><span class="sxs-lookup"><span data-stu-id="8a575-107">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="8a575-108">Für alle gruppenbezogenen Vorgänge in Microsoft Graph ist die Zustimmung durch einen Administrator erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a575-108">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="8a575-109">**Hinweis**: Gruppen können nur über Geschäfts- oder Schulkonten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="8a575-109">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="8a575-110">Persönliche Microsoft-Konten unterstützen keine Gruppen.</span><span class="sxs-lookup"><span data-stu-id="8a575-110">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="8a575-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8a575-111">Type</span></span>              | <span data-ttu-id="8a575-112">Anwendungsfall</span><span class="sxs-lookup"><span data-stu-id="8a575-112">Use case</span></span> | <span data-ttu-id="8a575-113">groupType</span><span class="sxs-lookup"><span data-stu-id="8a575-113">groupType</span></span> | <span data-ttu-id="8a575-114">E-Mail-aktiviert</span><span class="sxs-lookup"><span data-stu-id="8a575-114">mail-enabled</span></span> | <span data-ttu-id="8a575-115">Mit aktivierter Sicherheit</span><span class="sxs-lookup"><span data-stu-id="8a575-115">security-enabled</span></span> | <span data-ttu-id="8a575-116">Erstellung über API möglich?</span><span class="sxs-lookup"><span data-stu-id="8a575-116">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="8a575-117">Office 365-Gruppen</span><span class="sxs-lookup"><span data-stu-id="8a575-117">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="8a575-118">Ermöglicht die Zusammenarbeit von Benutzern mit freigegebenen Microsoft-Onlineressourcen.</span><span class="sxs-lookup"><span data-stu-id="8a575-118">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="8a575-119">Ja</span><span class="sxs-lookup"><span data-stu-id="8a575-119">Yes</span></span> |
| [<span data-ttu-id="8a575-120">Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="8a575-120">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="8a575-121">Steuern des Benutzerzugriffs auf Ressourcen innerhalb der App.</span><span class="sxs-lookup"><span data-stu-id="8a575-121">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="8a575-122">Ja</span><span class="sxs-lookup"><span data-stu-id="8a575-122">Yes</span></span> |
| [<span data-ttu-id="8a575-123">E-Mail-aktivierte Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="8a575-123">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="8a575-124">Steuern des Benutzerzugriffs auf Ressourcen innerhalb der App mit einem freigegebenen Gruppenpostfach.</span><span class="sxs-lookup"><span data-stu-id="8a575-124">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="8a575-125">Nein</span><span class="sxs-lookup"><span data-stu-id="8a575-125">No</span></span> |
| <span data-ttu-id="8a575-126">Verteilergruppen</span><span class="sxs-lookup"><span data-stu-id="8a575-126">Distribution groups</span></span> | <span data-ttu-id="8a575-127">Verteilen von E-Mail-Nachrichten an die Mitglieder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="8a575-127">Distributing mail to the members of the group.</span></span> <span data-ttu-id="8a575-128">Es wird empfohlen, dass Sie aufgrund der vielfältigeren Ressourcen Office 365-Gruppen verwenden.</span><span class="sxs-lookup"><span data-stu-id="8a575-128">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="8a575-129">Nein</span><span class="sxs-lookup"><span data-stu-id="8a575-129">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="8a575-130">Office 365-Gruppen</span><span class="sxs-lookup"><span data-stu-id="8a575-130">Office 365 groups</span></span>
<span data-ttu-id="8a575-131">Die Leistungsfähigkeit von Office 365-Gruppen liegt an der Zusammenarbeitsfunktion, die ideal für Personen geeignet ist, die an einem Projekt oder in einem Team zusammenarbeiten.</span><span class="sxs-lookup"><span data-stu-id="8a575-131">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="8a575-132">Diese werden mit Ressourcen erstellt, die Mitglieder der Gruppe gemeinsam verwenden, darunter:</span><span class="sxs-lookup"><span data-stu-id="8a575-132">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="8a575-133">Outlook-Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="8a575-133">Outlook conversations</span></span>
- <span data-ttu-id="8a575-134">Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="8a575-134">Outlook calendar</span></span>
- <span data-ttu-id="8a575-135">SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="8a575-135">SharePoint files</span></span>
- <span data-ttu-id="8a575-136">OneNote-Notizbuch</span><span class="sxs-lookup"><span data-stu-id="8a575-136">OneNote notebook</span></span>
- <span data-ttu-id="8a575-137">SharePoint-Teamwebsite</span><span class="sxs-lookup"><span data-stu-id="8a575-137">SharePoint team site</span></span>
- <span data-ttu-id="8a575-138">Planner-Pläne</span><span class="sxs-lookup"><span data-stu-id="8a575-138">Planner plans</span></span>
- <span data-ttu-id="8a575-139">Intune-Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="8a575-139">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="8a575-140">Beispiel einer Gruppe in Outlook</span><span class="sxs-lookup"><span data-stu-id="8a575-140">Group in Outlook example</span></span>

<span data-ttu-id="8a575-141">Es folgt eine JSON-Darstellung von Gruppen in Outlook.</span><span class="sxs-lookup"><span data-stu-id="8a575-141">The following is a JSON representation of groups in Outlook.</span></span> 

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
<span data-ttu-id="8a575-142">Weitere Informationen zu Office 365-Gruppen und der Administratorerfahrung finden Sie unter [Weitere Informationen zu Gruppen in Office 365](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="8a575-142">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="8a575-143">Sicherheitsgruppen und E-Mail-aktivierte Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="8a575-143">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="8a575-144">Sicherheitsgruppen sind für das Steuern des Benutzerzugriffs auf Ressourcen gedacht.</span><span class="sxs-lookup"><span data-stu-id="8a575-144">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="8a575-145">Durch Überprüfen, ob ein Benutzer ein Mitglied einer Sicherheitsgruppe ist, kann Ihre App Autorisierungsentscheidungen treffen, wenn dieser Benutzer versucht, auf sichere Ressourcen in Ihrer App zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="8a575-145">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="8a575-146">Sicherheitsgruppen können Benutzer und andere Sicherheitsgruppen als Mitglieder haben.</span><span class="sxs-lookup"><span data-stu-id="8a575-146">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="8a575-147">E-Mail-aktivierte Sicherheitsgruppen werden auf die gleiche Weise wie Sicherheitsgruppen verwendet, weisen jedoch das zusätzliche Feature eines freigegebenen Postfachs für die Gruppen auf.</span><span class="sxs-lookup"><span data-stu-id="8a575-147">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="8a575-148">E-Mail-aktivierte Sicherheitsgruppen können nicht über die API erstellt werden, aber andere Gruppenvorgänge funktionieren weiterhin.</span><span class="sxs-lookup"><span data-stu-id="8a575-148">Mail-enabled security groups can't be created through the API, but other group operations work.</span></span>  <span data-ttu-id="8a575-149">E-Mail-aktivierte Sicherheitsgruppen sind schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8a575-149">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="8a575-150">Weitere Informationen finden Sie im Exchange-Artikel  [Verwalten von E-Mail-aktivierten Sicherheitsgruppen](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8a575-150">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="8a575-151">Beispiel für eine Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="8a575-151">Security group example</span></span>

<span data-ttu-id="8a575-152">Es folgt eine JSON-Darstellung einer Sicherheitsgruppe.</span><span class="sxs-lookup"><span data-stu-id="8a575-152">The following is a JSON representation of a security group.</span></span> 

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
## <a name="dynamic-membership"></a><span data-ttu-id="8a575-153">Dynamische Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="8a575-153">Dynamic membership</span></span> 

<span data-ttu-id="8a575-154">Alle Typen von Gruppen können Regeln für dynamische Mitgliedschaft aufweisen, die automatisch Mitglieder zu der Gruppe basierend auf den Benutzereigenschaften hinzufügen oder darauf entfernen.</span><span class="sxs-lookup"><span data-stu-id="8a575-154">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="8a575-155">Die Gruppe „Marketing-Mitarbeiter“ würde beispielsweise jeden Benutzer einschließen, für den die department-Eigenschaft auf „Marketing“ festgelegt ist, sodass neue Marketing-Mitarbeiter automatisch zu der Gruppe hinzugefügt werden, und Mitarbeiter, die die Abteilung verlassen, automatisch aus der Gruppe entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="8a575-155">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="8a575-156">Diese Regel kann im Feld „membershipRule“ während der Erstellung von Gruppen als `"membershipRule": 'user.department -eq "Marketing"'` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="8a575-156">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="8a575-157">GroupType muss auch `"DynamicMembership"` umfassen.</span><span class="sxs-lookup"><span data-stu-id="8a575-157">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="8a575-158">Die folgende Anforderung erstellt eine neue Office 365-Gruppe für die Marketing-Mitarbeiter:</span><span class="sxs-lookup"><span data-stu-id="8a575-158">The following request creates a new Office 365 group for the marketing employees:</span></span> 

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

<span data-ttu-id="8a575-159">Weitere Informationen zum Verfassen von membershipRules finden Sie unter [Erstellen von attributbasierten Regeln für dynamische Gruppenmitgliedschaft in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="8a575-159">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="8a575-160">**Hinweis**: Regeln für dynamische Mitgliedschaft erfordern eine Lizenz vom Mandanten auf der Ebene [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) oder höher.</span><span class="sxs-lookup"><span data-stu-id="8a575-160">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="8a575-161">Andere Arten von Gruppen</span><span class="sxs-lookup"><span data-stu-id="8a575-161">Other types of groups</span></span>

<span data-ttu-id="8a575-162">Office 365-Gruppen in Yammer werden verwendet, um die Zusammenarbeit von Benutzern über Yammer-Beiträge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="8a575-162">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="8a575-163">Diese Art von Gruppe kann über eine Leseanforderung zurückgegeben werden, auf die Beiträge kann jedoch nicht über die API zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="8a575-163">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="8a575-164">Wenn Yammer-Beiträge und Unterhaltungs-Feeds für eine Gruppe aktiviert sind, werden standardmäßige Office 365-Gruppenunterhaltungen deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="8a575-164">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="8a575-165">Weitere Informationen finden Sie unter [Yammer-Entwickler-API Dokumente](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="8a575-165">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="8a575-166">Allgemeine Anwendungsfälle</span><span class="sxs-lookup"><span data-stu-id="8a575-166">Common use cases</span></span>

<span data-ttu-id="8a575-167">Mit Microsoft Graph können Sie die folgenden allgemeinen Vorgänge ausführen.</span><span class="sxs-lookup"><span data-stu-id="8a575-167">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="8a575-168">**Anwendungsfälle**</span><span class="sxs-lookup"><span data-stu-id="8a575-168">**Use cases**</span></span>  | <span data-ttu-id="8a575-169">**REST-Ressourcen**</span><span class="sxs-lookup"><span data-stu-id="8a575-169">**REST resources**</span></span> | <span data-ttu-id="8a575-170">**Siehe auch**</span><span class="sxs-lookup"><span data-stu-id="8a575-170">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="8a575-171">**Gruppenobjekt und Methoden**</span><span class="sxs-lookup"><span data-stu-id="8a575-171">**Group object and methods**</span></span> | | |
| <span data-ttu-id="8a575-172">Neue Gruppen erstellen, vorhandene Gruppen abrufen, die Eigenschaften für Gruppe aktualisieren und Gruppen löschen.</span><span class="sxs-lookup"><span data-stu-id="8a575-172">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="8a575-173">Derzeit können nur Sicherheitsgruppen und Gruppen in Outlook über die API erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="8a575-173">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="8a575-174">Gruppe</span><span class="sxs-lookup"><span data-stu-id="8a575-174">group</span></span>](group.md) | [<span data-ttu-id="8a575-175">Neue Gruppen erstellen</span><span class="sxs-lookup"><span data-stu-id="8a575-175">Create new groups</span></span>](../api/group-post-groups.md) <br/> [<span data-ttu-id="8a575-176">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="8a575-176">List groups</span></span>](../api/group-list.md) <br/> [<span data-ttu-id="8a575-177">Gruppen aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8a575-177">Update groups</span></span>](../api/group-update.md) <br/> [<span data-ttu-id="8a575-178">Gruppen löschen</span><span class="sxs-lookup"><span data-stu-id="8a575-178">Delete groups</span></span>](../api/group-delete.md) |
| <span data-ttu-id="8a575-179">**Methoden für Gruppenmitgliedschaft**</span><span class="sxs-lookup"><span data-stu-id="8a575-179">**Group membership methods**</span></span> | | |
| <span data-ttu-id="8a575-180">Mitglieder einer Gruppe auflisten und Mitglieder hinzufügen oder entfernen.</span><span class="sxs-lookup"><span data-stu-id="8a575-180">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="8a575-181">user</span><span class="sxs-lookup"><span data-stu-id="8a575-181">user</span></span>](user.md) <br/> [<span data-ttu-id="8a575-182">Gruppe</span><span class="sxs-lookup"><span data-stu-id="8a575-182">group</span></span>](group.md)| [<span data-ttu-id="8a575-183">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="8a575-183">List members</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="8a575-184">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8a575-184">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="8a575-185">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="8a575-185">Remove member</span></span>](../api/group-delete-members.md)|
| <span data-ttu-id="8a575-186">Bestimmen, ob ein Benutzer Mitglied einer Gruppe ist, alle Gruppen abrufen, bei denen der Benutzer Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="8a575-186">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="8a575-187">user</span><span class="sxs-lookup"><span data-stu-id="8a575-187">user</span></span>](user.md) <br/> [<span data-ttu-id="8a575-188">Gruppe</span><span class="sxs-lookup"><span data-stu-id="8a575-188">group</span></span>](group.md)| [<span data-ttu-id="8a575-189">Mitgliedergruppen prüfen</span><span class="sxs-lookup"><span data-stu-id="8a575-189">Check member groups</span></span>](../api/group-checkmembergroups.md) <br/> [<span data-ttu-id="8a575-190">Mitgliedergruppen abrufen</span><span class="sxs-lookup"><span data-stu-id="8a575-190">Get member groups</span></span>](../api/group-getmembergroups.md)|
| <span data-ttu-id="8a575-191">Besitzer einer Gruppe auflisten und Besitzer hinzufügen oder entfernen.</span><span class="sxs-lookup"><span data-stu-id="8a575-191">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="8a575-192">Benutzer</span><span class="sxs-lookup"><span data-stu-id="8a575-192">user</span></span>](user.md) <br/> [<span data-ttu-id="8a575-193">Gruppe</span><span class="sxs-lookup"><span data-stu-id="8a575-193">group</span></span>](group.md)| [<span data-ttu-id="8a575-194">Besitzer auflisten</span><span class="sxs-lookup"><span data-stu-id="8a575-194">List owners</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="8a575-195">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8a575-195">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="8a575-196">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="8a575-196">Remove member</span></span>](../api/group-delete-members.md)|
