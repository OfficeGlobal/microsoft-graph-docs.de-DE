---
title: Arbeiten mit Gruppen in Microsoft Graph
description: Gruppen sind Auflistungen von Benutzern und anderen Hauptbenutzern, die den Zugriff auf Ressourcen in Microsoft-Diensten oder in Ihrer App gemeinsam nutzen. Microsoft Graph enthält APIs, die Sie zum Erstellen und Verwalten von verschiedenen Typen von Gruppen und Gruppenfunktionalitäten entsprechend Ihrem Szenario verwenden können. Für alle gruppenbezogenen Vorgänge in Microsoft Graph ist die Zustimmung durch einen Administrator erforderlich.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 46d8f1db9a2c3c12add07787d62fe02c588cd6ae
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642268"
---
# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="ee8ed-105">Arbeiten mit Gruppen in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ee8ed-105">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="ee8ed-106">Gruppen sind Auflistungen von [Benutzern](user.md) und anderen Hauptbenutzern, die den Zugriff auf Ressourcen in Microsoft-Diensten oder in Ihrer App gemeinsam nutzen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-106">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="ee8ed-107">Microsoft Graph enthält APIs, die Sie zum Erstellen und Verwalten von verschiedenen Typen von Gruppen und Gruppenfunktionalitäten entsprechend Ihrem Szenario verwenden können.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-107">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="ee8ed-108">Für alle gruppenbezogenen Vorgänge in Microsoft Graph ist die Zustimmung durch einen Administrator erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-108">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="ee8ed-109">**Hinweis**: Gruppen können nur über Geschäfts- oder Schulkonten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-109">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="ee8ed-110">Persönliche Microsoft-Konten unterstützen keine Gruppen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-110">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="ee8ed-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ee8ed-111">Type</span></span>              | <span data-ttu-id="ee8ed-112">Anwendungsfall</span><span class="sxs-lookup"><span data-stu-id="ee8ed-112">Use case</span></span> | <span data-ttu-id="ee8ed-113">groupType</span><span class="sxs-lookup"><span data-stu-id="ee8ed-113">groupType</span></span> | <span data-ttu-id="ee8ed-114">E-Mail-aktiviert</span><span class="sxs-lookup"><span data-stu-id="ee8ed-114">mail-enabled</span></span> | <span data-ttu-id="ee8ed-115">Mit aktivierter Sicherheit</span><span class="sxs-lookup"><span data-stu-id="ee8ed-115">security-enabled</span></span> | <span data-ttu-id="ee8ed-116">Erstellung über API möglich?</span><span class="sxs-lookup"><span data-stu-id="ee8ed-116">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="ee8ed-117">Office 365-Gruppen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-117">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="ee8ed-118">Ermöglicht die Zusammenarbeit von Benutzern mit freigegebenen Microsoft-Onlineressourcen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-118">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="ee8ed-119">Ja</span><span class="sxs-lookup"><span data-stu-id="ee8ed-119">Yes</span></span> |
| [<span data-ttu-id="ee8ed-120">Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-120">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="ee8ed-121">Steuern des Benutzerzugriffs auf Ressourcen innerhalb der App.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-121">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="ee8ed-122">Ja</span><span class="sxs-lookup"><span data-stu-id="ee8ed-122">Yes</span></span> |
| [<span data-ttu-id="ee8ed-123">E-Mail-aktivierte Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-123">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="ee8ed-124">Steuern des Benutzerzugriffs auf Ressourcen innerhalb der App mit einem freigegebenen Gruppenpostfach.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-124">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="ee8ed-125">Nein</span><span class="sxs-lookup"><span data-stu-id="ee8ed-125">No</span></span> |
| <span data-ttu-id="ee8ed-126">Verteilergruppen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-126">Distribution groups</span></span> | <span data-ttu-id="ee8ed-127">Verteilen von E-Mail-Nachrichten an die Mitglieder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-127">Distributing mail to the members of the group.</span></span> <span data-ttu-id="ee8ed-128">Es wird empfohlen, dass Sie aufgrund der vielfältigeren Ressourcen Office 365-Gruppen verwenden.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-128">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="ee8ed-129">Nein</span><span class="sxs-lookup"><span data-stu-id="ee8ed-129">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="ee8ed-130">Office 365-Gruppen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-130">Office 365 groups</span></span>
<span data-ttu-id="ee8ed-131">Die Leistungsfähigkeit von Office 365-Gruppen liegt an der Zusammenarbeitsfunktion, die ideal für Personen geeignet ist, die an einem Projekt oder in einem Team zusammenarbeiten.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-131">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="ee8ed-132">Diese werden mit Ressourcen erstellt, die Mitglieder der Gruppe gemeinsam verwenden, darunter:</span><span class="sxs-lookup"><span data-stu-id="ee8ed-132">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="ee8ed-133">Outlook-Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="ee8ed-133">Outlook conversations</span></span>
- <span data-ttu-id="ee8ed-134">Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="ee8ed-134">Outlook calendar</span></span>
- <span data-ttu-id="ee8ed-135">SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="ee8ed-135">SharePoint files</span></span>
- <span data-ttu-id="ee8ed-136">OneNote-Notizbuch</span><span class="sxs-lookup"><span data-stu-id="ee8ed-136">OneNote notebook</span></span>
- <span data-ttu-id="ee8ed-137">SharePoint-Teamwebsite</span><span class="sxs-lookup"><span data-stu-id="ee8ed-137">SharePoint team site</span></span>
- <span data-ttu-id="ee8ed-138">Planner-Pläne</span><span class="sxs-lookup"><span data-stu-id="ee8ed-138">Planner plans</span></span>
- <span data-ttu-id="ee8ed-139">Intune-Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="ee8ed-139">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="ee8ed-140">Beispiel einer Gruppe in Outlook</span><span class="sxs-lookup"><span data-stu-id="ee8ed-140">Group in Outlook example</span></span>

<span data-ttu-id="ee8ed-141">Es folgt eine JSON-Darstellung von Gruppen in Outlook.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-141">The following is a JSON representation of groups in Outlook.</span></span> 

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
<span data-ttu-id="ee8ed-142">Weitere Informationen zu Office 365-Gruppen und der Administratorerfahrung finden Sie unter [Weitere Informationen zu Gruppen in Office 365](https://support.office.com/de-DE/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="ee8ed-142">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/de-DE/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="ee8ed-143">Sicherheitsgruppen und E-Mail-aktivierte Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-143">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="ee8ed-144">Sicherheitsgruppen sind für das Steuern des Benutzerzugriffs auf Ressourcen gedacht.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-144">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="ee8ed-145">Durch Überprüfen, ob ein Benutzer ein Mitglied einer Sicherheitsgruppe ist, kann Ihre App Autorisierungsentscheidungen treffen, wenn dieser Benutzer versucht, auf sichere Ressourcen in Ihrer App zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-145">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="ee8ed-146">Sicherheitsgruppen können Benutzer und andere Sicherheitsgruppen als Mitglieder haben.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-146">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="ee8ed-147">E-Mail-aktivierte Sicherheitsgruppen werden auf die gleiche Weise wie Sicherheitsgruppen verwendet, weisen jedoch das zusätzliche Feature eines freigegebenen Postfachs für die Gruppen auf.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-147">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="ee8ed-148">E-Mail-aktivierte Sicherheitsgruppen können nicht über die API erstellt werden, aber andere Gruppenvorgänge funktionieren weiterhin.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-148">Mail-enabled security groups can't be created through the API, but other group operations work.</span></span>  <span data-ttu-id="ee8ed-149">E-Mail-aktivierte Sicherheitsgruppen sind schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-149">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="ee8ed-150">Weitere Informationen finden Sie im Exchange-Artikel  [Verwalten von E-Mail-aktivierten Sicherheitsgruppen](https://technet.microsoft.com/de-DE/library/bb123521%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ee8ed-150">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/de-DE/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="ee8ed-151">Beispiel für eine Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="ee8ed-151">Security group example</span></span>

<span data-ttu-id="ee8ed-152">Es folgt eine JSON-Darstellung einer Sicherheitsgruppe.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-152">The following is a JSON representation of a security group.</span></span> 

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
## <a name="dynamic-membership"></a><span data-ttu-id="ee8ed-153">Dynamische Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="ee8ed-153">Dynamic membership</span></span> 

<span data-ttu-id="ee8ed-154">Alle Typen von Gruppen können Regeln für dynamische Mitgliedschaft aufweisen, die automatisch Mitglieder zu der Gruppe basierend auf den Benutzereigenschaften hinzufügen oder darauf entfernen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-154">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="ee8ed-155">Die Gruppe „Marketing-Mitarbeiter“ würde beispielsweise jeden Benutzer einschließen, für den die department-Eigenschaft auf „Marketing“ festgelegt ist, sodass neue Marketing-Mitarbeiter automatisch zu der Gruppe hinzugefügt werden, und Mitarbeiter, die die Abteilung verlassen, automatisch aus der Gruppe entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-155">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="ee8ed-156">Diese Regel kann im Feld „membershipRule“ während der Erstellung von Gruppen als `"membershipRule": 'user.department -eq "Marketing"'` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-156">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="ee8ed-157">GroupType muss auch `"DynamicMembership"` umfassen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-157">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="ee8ed-158">Die folgende Anforderung erstellt eine neue Office 365-Gruppe für die Marketing-Mitarbeiter:</span><span class="sxs-lookup"><span data-stu-id="ee8ed-158">The following request creates a new Office 365 group for the marketing employees:</span></span> 

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

<span data-ttu-id="ee8ed-159">Weitere Informationen zum Verfassen von membershipRules finden Sie unter [Erstellen von attributbasierten Regeln für dynamische Gruppenmitgliedschaft in Azure Active Directory](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="ee8ed-159">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="ee8ed-160">**Hinweis**: Regeln für dynamische Mitgliedschaft erfordern eine Lizenz vom Mandanten auf der Ebene [Azure Active Directory Premium P1](https://azure.microsoft.com/de-DE/pricing/details/active-directory/) oder höher.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-160">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/de-DE/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="ee8ed-161">Andere Arten von Gruppen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-161">Other types of groups</span></span>

<span data-ttu-id="ee8ed-162">Office 365-Gruppen in Yammer werden verwendet, um die Zusammenarbeit von Benutzern über Yammer-Beiträge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-162">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="ee8ed-163">Diese Art von Gruppe kann über eine Leseanforderung zurückgegeben werden, auf die Beiträge kann jedoch nicht über die API zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-163">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="ee8ed-164">Wenn Yammer-Beiträge und Unterhaltungs-Feeds für eine Gruppe aktiviert sind, werden standardmäßige Office 365-Gruppenunterhaltungen deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-164">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="ee8ed-165">Weitere Informationen finden Sie in den [Yammer-Entwickler-API-Dokumenten](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="ee8ed-165">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="group-based-licensing"></a><span data-ttu-id="ee8ed-166">Gruppenbasierte Lizenzierung</span><span class="sxs-lookup"><span data-stu-id="ee8ed-166">Group-based licensing</span></span> 

<span data-ttu-id="ee8ed-167">Sie können die gruppenbasierte Lizenzierung verwenden, um eine oder mehrere Produktlizenzen einer Azure AD-Gruppe zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-167">You can use group-based licensing to assign one or more product licenses to an Azure AD group.</span></span> <span data-ttu-id="ee8ed-168">Azure AD stellt sicher, dass die Lizenzen allen Mitgliedern der Gruppe zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-168">Azure AD ensures that the licenses are assigned to all members of the group.</span></span> <span data-ttu-id="ee8ed-169">Allen neuen Mitgliedern, die der Gruppe beitreten, werden die entsprechenden Lizenzen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-169">Any new members who join the group are assigned the appropriate licenses.</span></span> <span data-ttu-id="ee8ed-170">Wenn sie die Gruppe verlassen, werden diese Lizenzen entfernt.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-170">When they leave the group, those licenses are removed.</span></span> <span data-ttu-id="ee8ed-171">Das Feature kann nur in Sicherheitsgruppen und in Office 365-Gruppen mit `securityEnabled=TRUE` verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-171">The feature can only be used with security groups and Office 365 groups that have `securityEnabled=TRUE`.</span></span> <span data-ttu-id="ee8ed-172">Weitere Informationen zur gruppenbasierten Lizenzierung finden Sie unter [Was ist die gruppenbasierte Lizenzierung in Azure Active Directory?](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="ee8ed-172">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory?](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="ee8ed-173">Allgemeine Anwendungsfälle</span><span class="sxs-lookup"><span data-stu-id="ee8ed-173">Common use cases</span></span>

<span data-ttu-id="ee8ed-174">Mit Microsoft Graph können Sie die folgenden allgemeinen Vorgänge ausführen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-174">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="ee8ed-175">**Anwendungsfälle**</span><span class="sxs-lookup"><span data-stu-id="ee8ed-175">**Use cases**</span></span>  | <span data-ttu-id="ee8ed-176">**REST-Ressourcen**</span><span class="sxs-lookup"><span data-stu-id="ee8ed-176">**REST resources**</span></span> | <span data-ttu-id="ee8ed-177">**Siehe auch**</span><span class="sxs-lookup"><span data-stu-id="ee8ed-177">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="ee8ed-178">**Gruppenobjekt und Methoden**</span><span class="sxs-lookup"><span data-stu-id="ee8ed-178">**Group object and methods**</span></span> | | |
| <span data-ttu-id="ee8ed-179">Neue Gruppen erstellen, vorhandene Gruppen abrufen, die Eigenschaften für Gruppe aktualisieren und Gruppen löschen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-179">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="ee8ed-180">Derzeit können nur Sicherheitsgruppen und Gruppen in Outlook über die API erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-180">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="ee8ed-181">Gruppe</span><span class="sxs-lookup"><span data-stu-id="ee8ed-181">group</span></span>](group.md) | [<span data-ttu-id="ee8ed-182">Neue Gruppen erstellen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-182">Create new groups</span></span>](../api/group-post-groups.md) <br/> [<span data-ttu-id="ee8ed-183">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="ee8ed-183">List groups</span></span>](../api/group-list.md) <br/> [<span data-ttu-id="ee8ed-184">Gruppen aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ee8ed-184">Update groups</span></span>](../api/group-update.md) <br/> [<span data-ttu-id="ee8ed-185">Gruppen löschen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-185">Delete groups</span></span>](../api/group-delete.md) |
| <span data-ttu-id="ee8ed-186">**Methoden für Gruppenmitgliedschaft**</span><span class="sxs-lookup"><span data-stu-id="ee8ed-186">**Group membership methods**</span></span> | | |
| <span data-ttu-id="ee8ed-187">Mitglieder einer Gruppe auflisten und Mitglieder hinzufügen oder entfernen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-187">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="ee8ed-188">user</span><span class="sxs-lookup"><span data-stu-id="ee8ed-188">user</span></span>](user.md) <br/> [<span data-ttu-id="ee8ed-189">Gruppe</span><span class="sxs-lookup"><span data-stu-id="ee8ed-189">group</span></span>](group.md)| [<span data-ttu-id="ee8ed-190">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="ee8ed-190">List members</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="ee8ed-191">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-191">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="ee8ed-192">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-192">Remove member</span></span>](../api/group-delete-members.md)|
| <span data-ttu-id="ee8ed-193">Bestimmen, ob ein Benutzer Mitglied einer Gruppe ist, alle Gruppen abrufen, bei denen der Benutzer Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-193">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="ee8ed-194">user</span><span class="sxs-lookup"><span data-stu-id="ee8ed-194">user</span></span>](user.md) <br/> [<span data-ttu-id="ee8ed-195">Gruppe</span><span class="sxs-lookup"><span data-stu-id="ee8ed-195">group</span></span>](group.md)| [<span data-ttu-id="ee8ed-196">Mitgliedergruppen prüfen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-196">Check member groups</span></span>](../api/group-checkmembergroups.md) <br/> [<span data-ttu-id="ee8ed-197">Mitgliedergruppen abrufen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-197">Get member groups</span></span>](../api/group-getmembergroups.md)|
| <span data-ttu-id="ee8ed-198">Besitzer einer Gruppe auflisten und Besitzer hinzufügen oder entfernen.</span><span class="sxs-lookup"><span data-stu-id="ee8ed-198">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="ee8ed-199">Benutzer</span><span class="sxs-lookup"><span data-stu-id="ee8ed-199">user</span></span>](user.md) <br/> [<span data-ttu-id="ee8ed-200">Gruppe</span><span class="sxs-lookup"><span data-stu-id="ee8ed-200">group</span></span>](group.md)| [<span data-ttu-id="ee8ed-201">Besitzer auflisten</span><span class="sxs-lookup"><span data-stu-id="ee8ed-201">List owners</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="ee8ed-202">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-202">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="ee8ed-203">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="ee8ed-203">Remove member</span></span>](../api/group-delete-members.md)|
