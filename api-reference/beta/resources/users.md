---
title: Arbeiten mit Benutzern in Microsoft Graph
description: Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b98bdd3f84171823942b3a48dd49a8993597a5ee
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572178"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="2da9d-103">Arbeiten mit Benutzern in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2da9d-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2da9d-104">Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.</span><span class="sxs-lookup"><span data-stu-id="2da9d-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="2da9d-105">Sie können auf zwei Arten über Microsoft Graph auf Benutzer zugreifen:</span><span class="sxs-lookup"><span data-stu-id="2da9d-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="2da9d-106">Anhand der ID, `/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="2da9d-106">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="2da9d-107">Anhand des `/me`-Alias für den angemeldeten Benutzer, welcher `/users/{signed-in user's id}` entspricht</span><span class="sxs-lookup"><span data-stu-id="2da9d-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="2da9d-108">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2da9d-108">Authorization</span></span>
<span data-ttu-id="2da9d-p101">Für den Zugriff auf Benutzervorgänge ist eine der folgenden [Berechtigungen](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) erforderlich. Die ersten drei Berechtigungen können einer App durch einen Benutzer gewährt werden. Die übrigen können der App nur durch einen Administrator gewährt werden.</span><span class="sxs-lookup"><span data-stu-id="2da9d-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="2da9d-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="2da9d-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="2da9d-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="2da9d-113">User.Read</span></span>
- <span data-ttu-id="2da9d-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2da9d-114">User.ReadWrite</span></span>
- <span data-ttu-id="2da9d-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2da9d-115">User.Read.All</span></span>
- <span data-ttu-id="2da9d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2da9d-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="2da9d-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2da9d-117">Directory.Read.All</span></span>
- <span data-ttu-id="2da9d-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2da9d-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="2da9d-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2da9d-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="2da9d-120">Allgemeine Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2da9d-120">Common properties</span></span>

<span data-ttu-id="2da9d-121">Im Folgenden werden standardmäßige Eigenschaften dargestellt, die beim Abrufen eines Benutzers oder beim Auflisten von Benutzern zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="2da9d-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="2da9d-122">Diese stellen eine Teilmenge aller verfügbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="2da9d-122">These are a subset of all available properties.</span></span> <span data-ttu-id="2da9d-123">Verwenden Sie zum Abrufen weiterer Benutzereigenschaften den `$select`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="2da9d-123">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="2da9d-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2da9d-124">Property</span></span> |<span data-ttu-id="2da9d-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2da9d-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="2da9d-126">id</span><span class="sxs-lookup"><span data-stu-id="2da9d-126">id</span></span> | <span data-ttu-id="2da9d-127">Die eindeutige ID des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="2da9d-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="2da9d-128">businessPhones</span></span> | <span data-ttu-id="2da9d-129">Telefonnummern des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="2da9d-130">displayName</span><span class="sxs-lookup"><span data-stu-id="2da9d-130">displayName</span></span> | <span data-ttu-id="2da9d-131">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="2da9d-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="2da9d-132">givenName</span><span class="sxs-lookup"><span data-stu-id="2da9d-132">givenName</span></span>| <span data-ttu-id="2da9d-133">Der Vorname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-133">The first name of the user.</span></span> |
|<span data-ttu-id="2da9d-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="2da9d-134">jobTitle</span></span> | <span data-ttu-id="2da9d-135">Die Position des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-135">The user's job title.</span></span>|
|<span data-ttu-id="2da9d-136">mail</span><span class="sxs-lookup"><span data-stu-id="2da9d-136">mail</span></span>| <span data-ttu-id="2da9d-137">Die E-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-137">The user's email address.</span></span> |
|<span data-ttu-id="2da9d-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="2da9d-138">mobilePhone</span></span> | <span data-ttu-id="2da9d-139">Die Mobiltelefonnummern des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="2da9d-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="2da9d-140">officeLocation</span></span> | <span data-ttu-id="2da9d-141">Der Bürostandort des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-141">The user's physical office location.</span></span>|
|<span data-ttu-id="2da9d-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="2da9d-142">preferredLanguage</span></span> | <span data-ttu-id="2da9d-143">Die vom Benutzer bevorzugte Sprache.</span><span class="sxs-lookup"><span data-stu-id="2da9d-143">The user's language of preference.</span></span>|
|<span data-ttu-id="2da9d-144">surname</span><span class="sxs-lookup"><span data-stu-id="2da9d-144">surname</span></span>| <span data-ttu-id="2da9d-145">Der Nachname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-145">The last name of the user.</span></span> |
|<span data-ttu-id="2da9d-146">mail</span><span class="sxs-lookup"><span data-stu-id="2da9d-146">mail</span></span>| <span data-ttu-id="2da9d-147">Die E-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-147">The user's email address.</span></span> |
|<span data-ttu-id="2da9d-148">photo</span><span class="sxs-lookup"><span data-stu-id="2da9d-148">photo</span></span>| <span data-ttu-id="2da9d-149">Das Profilfoto des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2da9d-149">The user's profile photo. Read-only.</span></span> |
|<span data-ttu-id="2da9d-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2da9d-150">userPrincipalName</span></span>| <span data-ttu-id="2da9d-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="2da9d-151">The user's principal name.</span></span> |

<span data-ttu-id="2da9d-152">Weitere Informationen und eine Liste aller Eigenschaften finden Sie unter [user](user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2da9d-152">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="2da9d-153">Allgemeine Vorgänge</span><span class="sxs-lookup"><span data-stu-id="2da9d-153">Common operations</span></span>
><span data-ttu-id="2da9d-154">**Hinweis:** Einige dieser Vorgänge erfordern zusätzliche Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="2da9d-154">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="2da9d-155">Pfad</span><span class="sxs-lookup"><span data-stu-id="2da9d-155">Path</span></span>    | <span data-ttu-id="2da9d-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2da9d-156">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="2da9d-157">Listet die Benutzer in der Organisation auf.</span><span class="sxs-lookup"><span data-stu-id="2da9d-157">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="2da9d-158">Ruft einen bestimmten Benutzer anhand der ID ab.</span><span class="sxs-lookup"><span data-stu-id="2da9d-158">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="2da9d-159">Ruft das Profilfoto des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="2da9d-159">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="2da9d-160">Ruft den Vorgesetzten des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="2da9d-160">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="2da9d-161">Listet die E-Mails des Benutzers im primären Posteingang auf.</span><span class="sxs-lookup"><span data-stu-id="2da9d-161">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="2da9d-162">Listet bevorstehende Ereignisse des Benutzers im Kalender auf.</span><span class="sxs-lookup"><span data-stu-id="2da9d-162">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="2da9d-163">Ruft den OneDrive-Dateispeicher des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="2da9d-163">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="2da9d-164">Listet die Gruppen auf, deren Mitglied der Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="2da9d-164">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="2da9d-165">Listet die Microsoft Teams auf, deren Mitglied der Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="2da9d-165">Get the Microsoft Teams that the user is a direct member of.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
