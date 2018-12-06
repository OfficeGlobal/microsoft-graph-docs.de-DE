---
title: Überblick über Benutzer in Microsoft Graph
description: Benutzer stehen für ein Geschäfts- oder Schul- bzw. Unikonto von Azure Active Directory (Azure AD) oder ein Microsoft-Konto in Microsoft Graph. Die **Benutzer**-Ressource in Microsoft Graph ist ein Hub, von dem aus Sie auf die Beziehungen und Ressourcen, die für Ihre Benutzer relevant sind, zugreifen können.
ms.openlocfilehash: 2f07cdea940a7fe09b034f8fb21f443447ec67d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092283"
---
# <a name="overview-of-users-in-microsoft-graph"></a><span data-ttu-id="7b5bd-104">Überblick über Benutzer in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7b5bd-104">Overview of users in Microsoft Graph</span></span>

<span data-ttu-id="7b5bd-105">Benutzer stehen für ein Geschäfts- oder Schul- bzw. Unikonto von Azure Active Directory (Azure AD) oder ein Microsoft-Konto in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-105">Users are the representation of an Azure Active Directory (Azure AD) work or school user account or a Microsoft account in Microsoft Graph.</span></span> <span data-ttu-id="7b5bd-106">Die **Benutzer**-Ressource in Microsoft Graph ist ein Hub, von dem aus Sie auf die Beziehungen und Ressourcen, die für Ihre Benutzer relevant sind, zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-106">The **user** resource in Microsoft Graph is a hub from which you can access the relationships and resources that are relevant to your users.</span></span>

![Diagramm mit einem Benutzer, der mit Kalender, E-Mail, Kontakten, Besprechungen, Aufgaben, Websites und Dokumenten verbunden ist](images/users.png)

## <a name="develop-user-centric-applications"></a><span data-ttu-id="7b5bd-108">Entwickeln von auf Benutzer ausgerichteten Anwendungen</span><span class="sxs-lookup"><span data-stu-id="7b5bd-108">Develop user-centric applications</span></span>

<span data-ttu-id="7b5bd-109">Sie können mit Microsoft Graph auf die Beziehungen, Dokumente, Kontakte und Einstellungen zugreifen, die im Kontext des angemeldeten Benutzers relevant sind.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-109">You can use Microsoft Graph to access the relationships, documents, contacts, and preferences that are contextually relevant to the signed-in user.</span></span> <span data-ttu-id="7b5bd-110">Die **Benutzer**-Ressource bietet eine einfache Möglichkeit zum Zugreifen und Bearbeiten von Benutzerressourcen ohne zusätzliche Aufrufe, ohne Suche nach bestimmten Authentifizierungsinformationen und die direkte Ausgabe von Abfragen für Microsoft Graph-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-110">The **user** resource provides straightforward way for you to access and manipulate user resources without having to perform additional calls, look up specific authentication information, and directly issue queries against other Microsoft Graph resources.</span></span>

<span data-ttu-id="7b5bd-111">Um auf die Informationen oder Daten eines Benutzers zuzugreifen, müssen Sie [den Zugriff im Namen dieses Benutzers erhalten](auth-v2-user.md).</span><span class="sxs-lookup"><span data-stu-id="7b5bd-111">To access a user's information and data, you'll need to [get access on their behalf](auth-v2-user.md).</span></span> <span data-ttu-id="7b5bd-112">Das Authentifizieren Ihrer Anwendung mit [Admin Zustimmung](permissions-reference.md) ermöglicht Ihnen, eine umfassendere Palette von Entitäten, die einem Benutzer zugeordnet sind, zu verwenden und zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-112">Authenticating your application with [admin consent](permissions-reference.md) enables you to work with and update a wider range of entities associated with a user.</span></span>

### <a name="manage-your-organization"></a><span data-ttu-id="7b5bd-113">Verwalten Ihrer Organisation</span><span class="sxs-lookup"><span data-stu-id="7b5bd-113">Manage your organization</span></span>

<span data-ttu-id="7b5bd-114">Erstellen Sie in Ihrer Organisation neue Benutzer, oder aktualisieren Sie die Ressourcen und Beziehungen vorhandener Benutzer.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-114">Create new users in your organization or update the resources and relationships for existing users.</span></span> <span data-ttu-id="7b5bd-115">Mit Microsoft Graph können Sie die folgenden Aufgaben für die Benutzerverwaltung ausführen:</span><span class="sxs-lookup"><span data-stu-id="7b5bd-115">You can use Microsoft Graph to perform the following user management tasks:</span></span> 

- <span data-ttu-id="7b5bd-116">Erstellen oder Löschen von Benutzern im Azure AD Ihrer Organisation</span><span class="sxs-lookup"><span data-stu-id="7b5bd-116">Create or delete users in your Azure AD organization.</span></span>
- <span data-ttu-id="7b5bd-117">Auflisten der Gruppenmitgliedschaften eines Benutzers und Ermitteln, ob ein Benutzer ein Mitglied einer Gruppe ist</span><span class="sxs-lookup"><span data-stu-id="7b5bd-117">List a user's group memberships and determine whether a user is a member of a group.</span></span>
- <span data-ttu-id="7b5bd-118">Auflisten der Benutzer, die einem Benutzer unterstellt sind, und Zuweisen eines Vorgesetzten zu einem Benutzer</span><span class="sxs-lookup"><span data-stu-id="7b5bd-118">List the users who report to a user and assign managers to a user.</span></span>
- <span data-ttu-id="7b5bd-119">Hochladen oder Abrufen eines Fotos des Benutzers</span><span class="sxs-lookup"><span data-stu-id="7b5bd-119">Upload or retrieve a photo for the user.</span></span>

### <a name="work-with-calendars-and-tasks"></a><span data-ttu-id="7b5bd-120">Arbeiten mit Kalendern und Aufgaben</span><span class="sxs-lookup"><span data-stu-id="7b5bd-120">Work with calendars and tasks</span></span>

<span data-ttu-id="7b5bd-121">Sie den Kalender und die Kalendergruppen, die einem Benutzer zugewiesen sind, anzeigen, Abfragen dazu durchführen und sie aktualisieren. Dies schließt Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="7b5bd-121">You can view, query, and update user calendar and calendar groups associated with a user, including:</span></span>

- <span data-ttu-id="7b5bd-122">Auflisten und Erstellen von Ereignissen in einem Benutzerkalender</span><span class="sxs-lookup"><span data-stu-id="7b5bd-122">List and create events on a users calendar.</span></span>
- <span data-ttu-id="7b5bd-123">Anzeigen von Aufgaben, die einem Benutzer zugewiesen sind</span><span class="sxs-lookup"><span data-stu-id="7b5bd-123">View tasks assigned to a user.</span></span>
- <span data-ttu-id="7b5bd-124">Suchen von freien Besprechungszeiten für eine Gruppe von Benutzern</span><span class="sxs-lookup"><span data-stu-id="7b5bd-124">Find free meeting times for a set of users.</span></span>
- <span data-ttu-id="7b5bd-125">Abrufen einer Liste von Erinnerungen, die im Benutzerkalender eingestellt sind</span><span class="sxs-lookup"><span data-stu-id="7b5bd-125">Get a list of reminders set on a user's calendar.</span></span>

### <a name="administer-mail-and-handle-contacts"></a><span data-ttu-id="7b5bd-126">Verwalten von E-Mails und Verarbeiten von Kontakten</span><span class="sxs-lookup"><span data-stu-id="7b5bd-126">Administer mail and handle contacts</span></span>

<span data-ttu-id="7b5bd-127">Sie können die E-Mail-Einstellungen und Kontaktlisten eines Benutzer konfigurieren und E-Mails im Auftrag eines Benutzers senden. Dies schließt Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="7b5bd-127">You can configure user mail settings and contact lists and send mail on a user's behalf, including:</span></span>

- <span data-ttu-id="7b5bd-128">Auflisten von E-Mail-Nachrichten und Senden neuer E-Mails</span><span class="sxs-lookup"><span data-stu-id="7b5bd-128">List mail messages and send new mail.</span></span>
- <span data-ttu-id="7b5bd-129">Erstellen und Auflisten von Benutzerkontakten und Organisieren von Kontakten in Ordnern</span><span class="sxs-lookup"><span data-stu-id="7b5bd-129">Create and list user contacts and organize contacts in folders.</span></span>
- <span data-ttu-id="7b5bd-130">Abrufen und Aktualisieren von Postfachordnern und Einstellungen</span><span class="sxs-lookup"><span data-stu-id="7b5bd-130">Retrieve and update mailbox folders and settings.</span></span>

### <a name="enrich-your-app-with-user-insights"></a><span data-ttu-id="7b5bd-131">Optimieren der App durch Einblicke in das Benutzerverhalten</span><span class="sxs-lookup"><span data-stu-id="7b5bd-131">Enrich your app with user insights</span></span>

<span data-ttu-id="7b5bd-132">Maximieren Sie die Relevanz in der Anwendung, indem Sie zuletzt verwendete oder beliebten Dokumente und Kontakte, die einem Benutzer zugeordnet sind, besonders hervorheben.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-132">Maximize relevance in your application by promoting recently used or trending documents and contacts associated with a user.</span></span> <span data-ttu-id="7b5bd-133">Mit Microsoft Graph haben Sie die folgenden Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="7b5bd-133">You can use Microsoft Graph to:</span></span>

- <span data-ttu-id="7b5bd-134">Zurückgeben der zuletzt angezeigten und durch einen Benutzer geänderten Dokumente</span><span class="sxs-lookup"><span data-stu-id="7b5bd-134">Return documents recently viewed and modified by a user.</span></span>
- <span data-ttu-id="7b5bd-135">Zurückgeben von Dokumenten und Websites, die einen Trend bei den Aktivitäten eines Benutzers zeigen</span><span class="sxs-lookup"><span data-stu-id="7b5bd-135">Return documents and sites trending around a user's activity.</span></span>
- <span data-ttu-id="7b5bd-136">Auflisten von Dokumenten, die über E-Mail oder OneDrive for Business mit dem Benutzer geteilt wurden</span><span class="sxs-lookup"><span data-stu-id="7b5bd-136">List documents shared with a user through email or OneDrive for Business.</span></span>

## <a name="api-reference"></a><span data-ttu-id="7b5bd-137">API-Referenz</span><span class="sxs-lookup"><span data-stu-id="7b5bd-137">API reference</span></span>
<span data-ttu-id="7b5bd-138">Suchen Sie die API-Referenz für diesen Dienst?</span><span class="sxs-lookup"><span data-stu-id="7b5bd-138">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="7b5bd-139">Benutzer-API in Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="7b5bd-139">Users API in Microsoft Graph v1.0</span></span>](/graph/api/resources/users?view=graph-rest-1.0)
- [<span data-ttu-id="7b5bd-140">Benutzer-API in Microsoft Graph, Betaversion</span><span class="sxs-lookup"><span data-stu-id="7b5bd-140">Users API in Microsoft Graph beta</span></span>](/graph/api/resources/users?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="7b5bd-141">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="7b5bd-141">Next steps</span></span>

- <span data-ttu-id="7b5bd-142">Erfahren Sie mehr über das [Arbeiten mit Benutzern](/graph/api/resources/users?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="7b5bd-142">Learn more about how to [work with users](/graph/api/resources/users?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="7b5bd-143">Untersuchen Sie Ihre eigenen Daten aus der **Benutzer**-Ressource im [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="7b5bd-143">Explore your own data from the **user** resource in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="7b5bd-144">Authentifizieren bei Microsoft Graph [im Auftrag eines Benutzers](auth-v2-user.md) oder [als Daemon oder als Dienst durch Zustimmung eines Administrators](auth-v2-service.md).</span><span class="sxs-lookup"><span data-stu-id="7b5bd-144">Authenticate with Microsoft Graph [on behalf of a user](auth-v2-user.md) or [as a daemon or service by consent of an administator](auth-v2-service.md).</span></span>
- <span data-ttu-id="7b5bd-145">Festlegen der Zugriffssteuerung und Richtlinien für Benutzer mit der [Azure AD-API](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="7b5bd-145">Set access control and policies for users with the [Azure AD API](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="7b5bd-146">Überprüfen der [Berechtigungen](permissions-reference.md), die Ihre App zum Zugreifen auf die Benutzerdaten haben muss.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-146">Review the [permissions](permissions-reference.md) your app will need to access user data.</span></span> 
<!-- This isn't really a next step; let's remove to keep the list of links concise.>
- Stay up to date with Microsoft Graph [changelog](changelog.md).
-->
