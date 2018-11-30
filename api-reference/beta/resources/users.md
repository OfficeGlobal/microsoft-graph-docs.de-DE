---
title: Arbeiten mit Benutzern in Microsoft Graph
description: Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.
ms.openlocfilehash: ee084bb52042b0c42f0308584ec6b3989b5b6114
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061686"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="9c63a-103">Arbeiten mit Benutzern in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9c63a-103">Working with users in Microsoft Graph</span></span>

> <span data-ttu-id="9c63a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9c63a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c63a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9c63a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c63a-106">Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.</span><span class="sxs-lookup"><span data-stu-id="9c63a-106">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="9c63a-107">Sie können auf zwei Arten über Microsoft Graph auf Benutzer zugreifen:</span><span class="sxs-lookup"><span data-stu-id="9c63a-107">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="9c63a-108">Anhand der ID, `/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="9c63a-108">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="9c63a-109">Anhand des `/me`-Alias für den angemeldeten Benutzer, welcher `/users/{signed-in user's id}` entspricht</span><span class="sxs-lookup"><span data-stu-id="9c63a-109">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="9c63a-110">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9c63a-110">Authorization</span></span>
<span data-ttu-id="9c63a-p102">Für den Zugriff auf Benutzervorgänge ist eine der folgenden [Berechtigungen](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) erforderlich. Die ersten drei Berechtigungen können einer App durch einen Benutzer gewährt werden. Die übrigen können der App nur durch einen Administrator gewährt werden.</span><span class="sxs-lookup"><span data-stu-id="9c63a-p102">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="9c63a-114">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="9c63a-114">User.ReadBasic.All</span></span>
- <span data-ttu-id="9c63a-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="9c63a-115">User.Read</span></span>
- <span data-ttu-id="9c63a-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c63a-116">User.ReadWrite</span></span>
- <span data-ttu-id="9c63a-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c63a-117">User.Read.All</span></span>
- <span data-ttu-id="9c63a-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c63a-118">User.ReadWrite.All</span></span>
- <span data-ttu-id="9c63a-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c63a-119">Directory.Read.All</span></span>
- <span data-ttu-id="9c63a-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c63a-120">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="9c63a-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c63a-121">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="9c63a-122">Allgemeine Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9c63a-122">Common properties</span></span>

| <span data-ttu-id="9c63a-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c63a-123">Property</span></span> | <span data-ttu-id="9c63a-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c63a-124">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="9c63a-125">displayName</span><span class="sxs-lookup"><span data-stu-id="9c63a-125">displayName</span></span> | <span data-ttu-id="9c63a-126">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="9c63a-126">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="9c63a-127">givenName</span><span class="sxs-lookup"><span data-stu-id="9c63a-127">givenName</span></span>| <span data-ttu-id="9c63a-128">Der Vorname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9c63a-128">The first name of the user.</span></span> |
|<span data-ttu-id="9c63a-129">surname</span><span class="sxs-lookup"><span data-stu-id="9c63a-129">surname</span></span>| <span data-ttu-id="9c63a-130">Der Nachname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9c63a-130">The last name of the user.</span></span> |
|<span data-ttu-id="9c63a-131">mail</span><span class="sxs-lookup"><span data-stu-id="9c63a-131">mail</span></span>| <span data-ttu-id="9c63a-132">Die E-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9c63a-132">The user's email address.</span></span> |
|<span data-ttu-id="9c63a-133">photo</span><span class="sxs-lookup"><span data-stu-id="9c63a-133">photo</span></span>| <span data-ttu-id="9c63a-134">Profil-Foto des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9c63a-134">The user's profile photo.</span></span> |

<span data-ttu-id="9c63a-135">Weitere Informationen und eine Liste aller Eigenschaften finden Sie unter [user](user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="9c63a-135">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="9c63a-136">Allgemeine Vorgänge</span><span class="sxs-lookup"><span data-stu-id="9c63a-136">Common operations</span></span>
><span data-ttu-id="9c63a-137">**Hinweis:** Einige dieser Vorgänge erfordern zusätzliche Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="9c63a-137">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="9c63a-138">Pfad</span><span class="sxs-lookup"><span data-stu-id="9c63a-138">Path</span></span>    | <span data-ttu-id="9c63a-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c63a-139">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="9c63a-140">Listet die Benutzer in der Organisation auf.</span><span class="sxs-lookup"><span data-stu-id="9c63a-140">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="9c63a-141">Ruft einen bestimmten Benutzer anhand der ID ab.</span><span class="sxs-lookup"><span data-stu-id="9c63a-141">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="9c63a-142">Ruft das Profilfoto des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="9c63a-142">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="9c63a-143">Ruft den Vorgesetzten des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="9c63a-143">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="9c63a-144">Listet die E-Mails des Benutzers im primären Posteingang auf.</span><span class="sxs-lookup"><span data-stu-id="9c63a-144">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="9c63a-145">Listet bevorstehende Ereignisse des Benutzers im Kalender auf.</span><span class="sxs-lookup"><span data-stu-id="9c63a-145">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="9c63a-146">Ruft den OneDrive-Dateispeicher des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="9c63a-146">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="9c63a-147">Listet die Gruppen auf, deren Mitglied der Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="9c63a-147">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="9c63a-148">Listet die Microsoft-Teams, die der Benutzer Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="9c63a-148">Lists the Microsoft Teams that the user is a member of.</span></span> |
