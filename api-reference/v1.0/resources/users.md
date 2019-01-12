---
title: Arbeiten mit Benutzern in Microsoft Graph
description: Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bfd7778d3fdc9675880b98a356dd690c4b1eaec8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966944"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="64d73-103">Arbeiten mit Benutzern in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="64d73-103">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="64d73-104">Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.</span><span class="sxs-lookup"><span data-stu-id="64d73-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="64d73-105">Sie können auf zwei Arten über Microsoft Graph auf [Benutzer](user.md) zugreifen:</span><span class="sxs-lookup"><span data-stu-id="64d73-105">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="64d73-106">Anhand der ID, `/users/{id | userPrincipalName}`</span><span class="sxs-lookup"><span data-stu-id="64d73-106">By their ID, `/users/{id | userPrincipalName}`</span></span> 
- <span data-ttu-id="64d73-107">Anhand des `/me`-Alias für den angemeldeten Benutzer, welcher `/users/{signed-in user's id}` entspricht</span><span class="sxs-lookup"><span data-stu-id="64d73-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="64d73-108">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="64d73-108">Authorization</span></span>

<span data-ttu-id="64d73-p101">Für den Zugriff auf Benutzervorgänge ist eine der folgenden [Berechtigungen](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) erforderlich. Die ersten drei Berechtigungen können einer App durch einen Benutzer gewährt werden. Die übrigen können der App nur durch einen Administrator gewährt werden.</span><span class="sxs-lookup"><span data-stu-id="64d73-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="64d73-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="64d73-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="64d73-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="64d73-113">User.Read</span></span>
- <span data-ttu-id="64d73-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64d73-114">User.ReadWrite</span></span>
- <span data-ttu-id="64d73-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="64d73-115">User.Read.All</span></span>
- <span data-ttu-id="64d73-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64d73-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="64d73-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="64d73-117">Directory.Read.All</span></span>
- <span data-ttu-id="64d73-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64d73-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="64d73-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64d73-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="64d73-120">Allgemeine Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="64d73-120">Common properties</span></span>

<span data-ttu-id="64d73-121">Im Folgenden werden standardmäßige Eigenschaften dargestellt, die beim Abrufen eines Benutzers oder beim Auflisten von Benutzern zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="64d73-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="64d73-122">Diese stellen eine Teilmenge aller verfügbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="64d73-122">These are a subset of all available properties.</span></span> <span data-ttu-id="64d73-123">Verwenden Sie zum Abrufen weiterer Benutzereigenschaften den `$select`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="64d73-123">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="64d73-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="64d73-124">Property</span></span> |<span data-ttu-id="64d73-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64d73-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="64d73-126">id</span><span class="sxs-lookup"><span data-stu-id="64d73-126">id</span></span> | <span data-ttu-id="64d73-127">Die eindeutige ID des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="64d73-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="64d73-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="64d73-128">businessPhones</span></span> | <span data-ttu-id="64d73-129">Telefonnummern des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="64d73-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="64d73-130">displayName</span><span class="sxs-lookup"><span data-stu-id="64d73-130">displayName</span></span> | <span data-ttu-id="64d73-131">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="64d73-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="64d73-132">givenName</span><span class="sxs-lookup"><span data-stu-id="64d73-132">givenName</span></span>| <span data-ttu-id="64d73-133">Der Vorname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="64d73-133">The first name of the user.</span></span> |
|<span data-ttu-id="64d73-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="64d73-134">jobTitle</span></span> | <span data-ttu-id="64d73-135">Die Position des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="64d73-135">The user's job title.</span></span>|
|<span data-ttu-id="64d73-136">mail</span><span class="sxs-lookup"><span data-stu-id="64d73-136">mail</span></span>| <span data-ttu-id="64d73-137">Die E-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="64d73-137">The user's email address.</span></span> |
|<span data-ttu-id="64d73-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="64d73-138">mobilePhone</span></span> | <span data-ttu-id="64d73-139">Die Mobiltelefonnummern des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="64d73-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="64d73-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="64d73-140">officeLocation</span></span> | <span data-ttu-id="64d73-141">Der Bürostandort des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="64d73-141">The user's physical office location.</span></span>|
|<span data-ttu-id="64d73-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="64d73-142">preferredLanguage</span></span> | <span data-ttu-id="64d73-143">Die vom Benutzer bevorzugte Sprache.</span><span class="sxs-lookup"><span data-stu-id="64d73-143">The user's language of preference.</span></span>|
|<span data-ttu-id="64d73-144">surname</span><span class="sxs-lookup"><span data-stu-id="64d73-144">surname</span></span>| <span data-ttu-id="64d73-145">Der Nachname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="64d73-145">The last name of the user.</span></span> |
|<span data-ttu-id="64d73-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="64d73-146">userPrincipalName</span></span>| <span data-ttu-id="64d73-147">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="64d73-147">The user's principal name.</span></span> |

<br/>

<span data-ttu-id="64d73-148">Weitere Informationen und eine Liste aller Eigenschaften finden Sie unter [user](user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="64d73-148">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="64d73-149">Allgemeine Vorgänge</span><span class="sxs-lookup"><span data-stu-id="64d73-149">Common operations</span></span>

> <span data-ttu-id="64d73-150">**Hinweis:** Einige dieser Vorgänge erfordern zusätzliche Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="64d73-150">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="64d73-151">Pfad</span><span class="sxs-lookup"><span data-stu-id="64d73-151">Path</span></span>    | <span data-ttu-id="64d73-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64d73-152">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="64d73-153">Listet die Benutzer in der Organisation auf.</span><span class="sxs-lookup"><span data-stu-id="64d73-153">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="64d73-154">Ruft einen bestimmten Benutzer anhand der ID ab.</span><span class="sxs-lookup"><span data-stu-id="64d73-154">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="64d73-155">Ruft das Profilfoto des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="64d73-155">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="64d73-156">Ruft den Vorgesetzten des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="64d73-156">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="64d73-157">Listet die E-Mails des Benutzers im primären Posteingang auf.</span><span class="sxs-lookup"><span data-stu-id="64d73-157">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="64d73-158">Listet bevorstehende Ereignisse des Benutzers im Kalender auf.</span><span class="sxs-lookup"><span data-stu-id="64d73-158">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="64d73-159">Ruft den OneDrive-Dateispeicher des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="64d73-159">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="64d73-160">Listet die Gruppen auf, deren Mitglied der Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="64d73-160">Lists the groups that the user is a member of.</span></span> |
