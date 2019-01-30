---
title: Arbeiten mit Benutzern in Microsoft Graph
description: Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f1a08e008f1de343ca6cf4986006c43c7e115af
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642058"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="d0460-103">Arbeiten mit Benutzern in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d0460-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0460-104">Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.</span><span class="sxs-lookup"><span data-stu-id="d0460-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="d0460-105">Sie können auf zwei Arten über Microsoft Graph auf Benutzer zugreifen:</span><span class="sxs-lookup"><span data-stu-id="d0460-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="d0460-106">Anhand der ID, `/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="d0460-106">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="d0460-107">Anhand des `/me`-Alias für den angemeldeten Benutzer, welcher `/users/{signed-in user's id}` entspricht</span><span class="sxs-lookup"><span data-stu-id="d0460-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="d0460-108">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d0460-108">Authorization</span></span>
<span data-ttu-id="d0460-p101">Für den Zugriff auf Benutzervorgänge ist eine der folgenden [Berechtigungen](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) erforderlich. Die ersten drei Berechtigungen können einer App durch einen Benutzer gewährt werden. Die übrigen können der App nur durch einen Administrator gewährt werden.</span><span class="sxs-lookup"><span data-stu-id="d0460-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="d0460-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="d0460-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="d0460-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="d0460-113">User.Read</span></span>
- <span data-ttu-id="d0460-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0460-114">User.ReadWrite</span></span>
- <span data-ttu-id="d0460-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0460-115">User.Read.All</span></span>
- <span data-ttu-id="d0460-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0460-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="d0460-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0460-117">Directory.Read.All</span></span>
- <span data-ttu-id="d0460-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0460-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="d0460-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0460-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="d0460-120">Allgemeine Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d0460-120">Common properties</span></span>

| <span data-ttu-id="d0460-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0460-121">Property</span></span> | <span data-ttu-id="d0460-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0460-122">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="d0460-123">displayName</span><span class="sxs-lookup"><span data-stu-id="d0460-123">displayName</span></span> | <span data-ttu-id="d0460-124">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d0460-124">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="d0460-125">givenName</span><span class="sxs-lookup"><span data-stu-id="d0460-125">givenName</span></span>| <span data-ttu-id="d0460-126">Der Vorname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d0460-126">The first name of the user.</span></span> |
|<span data-ttu-id="d0460-127">surname</span><span class="sxs-lookup"><span data-stu-id="d0460-127">surname</span></span>| <span data-ttu-id="d0460-128">Der Nachname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d0460-128">The last name of the user.</span></span> |
|<span data-ttu-id="d0460-129">mail</span><span class="sxs-lookup"><span data-stu-id="d0460-129">mail</span></span>| <span data-ttu-id="d0460-130">Die E-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d0460-130">The user's email address.</span></span> |
|<span data-ttu-id="d0460-131">photo</span><span class="sxs-lookup"><span data-stu-id="d0460-131">photo</span></span>| <span data-ttu-id="d0460-132">Das Profilfoto des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d0460-132">The user's profile photo.</span></span> |

<span data-ttu-id="d0460-133">Weitere Informationen und eine Liste aller Eigenschaften finden Sie unter [user](user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d0460-133">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="d0460-134">Allgemeine Vorgänge</span><span class="sxs-lookup"><span data-stu-id="d0460-134">Common operations</span></span>
><span data-ttu-id="d0460-135">**Hinweis:** Einige dieser Vorgänge erfordern zusätzliche Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="d0460-135">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="d0460-136">Pfad</span><span class="sxs-lookup"><span data-stu-id="d0460-136">Path</span></span>    | <span data-ttu-id="d0460-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0460-137">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="d0460-138">Listet die Benutzer in der Organisation auf.</span><span class="sxs-lookup"><span data-stu-id="d0460-138">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="d0460-139">Ruft einen bestimmten Benutzer anhand der ID ab.</span><span class="sxs-lookup"><span data-stu-id="d0460-139">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="d0460-140">Ruft das Profilfoto des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="d0460-140">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="d0460-141">Ruft den Vorgesetzten des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="d0460-141">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="d0460-142">Listet die E-Mails des Benutzers im primären Posteingang auf.</span><span class="sxs-lookup"><span data-stu-id="d0460-142">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="d0460-143">Listet bevorstehende Ereignisse des Benutzers im Kalender auf.</span><span class="sxs-lookup"><span data-stu-id="d0460-143">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="d0460-144">Ruft den OneDrive-Dateispeicher des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="d0460-144">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="d0460-145">Listet die Gruppen auf, deren Mitglied der Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="d0460-145">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="d0460-146">Listet die Microsoft Teams auf, deren Mitglied der Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="d0460-146">Lists the Microsoft Teams that the user is a member of.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
