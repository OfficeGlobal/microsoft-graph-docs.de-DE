---
title: Erweiterte einwertige Eigenschaft erstellen
description: 'Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource. '
localization_priority: Normal
ms.openlocfilehash: 3b122eb1a02ddd9e413f5c58bf840b912dd8365f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641393"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="7c27f-103">Erweiterte einwertige Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="7c27f-103">Create single-value extended property</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c27f-104">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource.</span><span class="sxs-lookup"><span data-stu-id="7c27f-104">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="7c27f-105">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="7c27f-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="7c27f-106">calendar</span><span class="sxs-lookup"><span data-stu-id="7c27f-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="7c27f-107">contact</span><span class="sxs-lookup"><span data-stu-id="7c27f-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="7c27f-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="7c27f-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="7c27f-109">event</span><span class="sxs-lookup"><span data-stu-id="7c27f-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="7c27f-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="7c27f-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="7c27f-111">message</span><span class="sxs-lookup"><span data-stu-id="7c27f-111">message</span></span>](../resources/message.md)
- [<span data-ttu-id="7c27f-112">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="7c27f-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="7c27f-113">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="7c27f-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="7c27f-114">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="7c27f-114">As well as the following group resources:</span></span>

- <span data-ttu-id="7c27f-115">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="7c27f-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="7c27f-116">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="7c27f-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="7c27f-117">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="7c27f-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="7c27f-118">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="7c27f-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c27f-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c27f-119">Permissions</span></span>
<span data-ttu-id="7c27f-120">Erstellen Sie je nach der Ressource in die erweiterte Eigenschaft und die Berechtigung geben (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="7c27f-120">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="7c27f-121">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c27f-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c27f-122">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="7c27f-122">Supported resource</span></span> | <span data-ttu-id="7c27f-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c27f-123">Delegated (work or school account)</span></span> | <span data-ttu-id="7c27f-124">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c27f-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c27f-125">Application</span><span class="sxs-lookup"><span data-stu-id="7c27f-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="7c27f-126">Kalender</span><span class="sxs-lookup"><span data-stu-id="7c27f-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="7c27f-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="7c27f-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="7c27f-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-129">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="7c27f-130">Kontakt</span><span class="sxs-lookup"><span data-stu-id="7c27f-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="7c27f-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="7c27f-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="7c27f-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="7c27f-134">contactFolder</span><span class="sxs-lookup"><span data-stu-id="7c27f-134">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="7c27f-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="7c27f-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="7c27f-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-137">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="7c27f-138">event</span><span class="sxs-lookup"><span data-stu-id="7c27f-138">event</span></span>](../resources/event.md) | <span data-ttu-id="7c27f-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-139">Calendars.ReadWrite</span></span> | <span data-ttu-id="7c27f-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-140">Calendars.ReadWrite</span></span> |  <span data-ttu-id="7c27f-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-141">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="7c27f-142">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="7c27f-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="7c27f-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c27f-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="7c27f-144">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c27f-144">Not supported</span></span> | <span data-ttu-id="7c27f-145">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c27f-145">Not supported</span></span> |
| <span data-ttu-id="7c27f-146">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="7c27f-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="7c27f-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c27f-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="7c27f-148">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c27f-148">Not supported</span></span> | <span data-ttu-id="7c27f-149">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c27f-149">Not supported</span></span> |
| <span data-ttu-id="7c27f-150">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="7c27f-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="7c27f-151">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c27f-151">Group.ReadWrite.All</span></span> | <span data-ttu-id="7c27f-152">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c27f-152">Not supported</span></span> | <span data-ttu-id="7c27f-153">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c27f-153">Not supported</span></span> |
| [<span data-ttu-id="7c27f-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="7c27f-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="7c27f-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-155">Mail.ReadWrite</span></span> | <span data-ttu-id="7c27f-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-156">Mail.ReadWrite</span></span> | <span data-ttu-id="7c27f-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-157">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="7c27f-158">message</span><span class="sxs-lookup"><span data-stu-id="7c27f-158">message</span></span>](../resources/message.md) | <span data-ttu-id="7c27f-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-159">Mail.ReadWrite</span></span> | <span data-ttu-id="7c27f-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-160">Mail.ReadWrite</span></span> | <span data-ttu-id="7c27f-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-161">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="7c27f-162">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="7c27f-162">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="7c27f-163">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-163">Tasks.ReadWrite</span></span> | <span data-ttu-id="7c27f-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="7c27f-165">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c27f-165">Not supported</span></span> |
| [<span data-ttu-id="7c27f-166">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="7c27f-166">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="7c27f-167">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-167">Tasks.ReadWrite</span></span> | <span data-ttu-id="7c27f-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c27f-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="7c27f-169">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c27f-169">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="7c27f-170">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c27f-170">HTTP request</span></span>
<span data-ttu-id="7c27f-171">Sie können erweiterte Eigenschaften in einer neuen oder vorhandenen Ressourceninstanz erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c27f-171">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="7c27f-172">Um eine oder mehrere erweiterte Eigenschaften in einer _neuen_ Instanz der Ressource zu erstellen, verwenden Sie die gleiche REST-Anforderung als die Instanz erstellt und enthalten Sie die Eigenschaften für die neue Ressource Instanz _und erweiterte Eigenschaft_ im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c27f-172">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="7c27f-173">Beachten Sie, dass einige Ressourcen in mehr als eine Möglichkeit der Erstellung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c27f-173">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="7c27f-174">Weitere Informationen zum Erstellen dieser Ressourceninstanzen, finden Sie unter den entsprechenden Themen für die Erstellung einer [Nachricht](../resources/message.md), [MailFolder](../api/user-post-mailfolders.md), [Ereignis](../api/user-post-events.md), [Kalender](../api/user-post-calendars.md), [wenden Sie sich an](../api/user-post-contacts.md), [ContactFolder](../api/user-post-contactfolders.md), [Outlook-Aufgabe](../resources/outlooktask.md), [ Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md), [Gruppe Ereignis](../api/group-post-events.md)und [Gruppe Post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="7c27f-174">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="7c27f-175">So sieht die Syntax der Anforderungen aus:</span><span class="sxs-lookup"><span data-stu-id="7c27f-175">The following is the syntax of the requests.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
POST /me/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks

POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="7c27f-176">Um eine oder mehrere erweiterte Eigenschaften in einer vorhandenen Ressourceninstanz zu erstellen,müssen Sie die Instanz in der Anforderung angeben und die erweiterte-Eigenschaft zum Anforderungstext hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="7c27f-176">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="7c27f-177">**Hinweis:** Sie können keine erweiterte Eigenschaft in einem vorhandenen Gruppenbeitrag erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c27f-177">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /me/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}

PATCH /me/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7c27f-178">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c27f-178">Request headers</span></span>
| <span data-ttu-id="7c27f-179">Name</span><span class="sxs-lookup"><span data-stu-id="7c27f-179">Name</span></span>       | <span data-ttu-id="7c27f-180">Wert</span><span class="sxs-lookup"><span data-stu-id="7c27f-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7c27f-181">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c27f-181">Authorization</span></span> | <span data-ttu-id="7c27f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c27f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c27f-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c27f-184">Content-Type</span></span> | <span data-ttu-id="7c27f-185">application/json</span><span class="sxs-lookup"><span data-stu-id="7c27f-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c27f-186">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c27f-186">Request body</span></span>

<span data-ttu-id="7c27f-187">Stellen Sie einen JSON-Text für jedes [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekt in der **singleValueExtendedProperties**-Sammlungseigenschaft der Ressourceninstanz bereit.</span><span class="sxs-lookup"><span data-stu-id="7c27f-187">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="7c27f-188">**Eigenschaft**</span><span class="sxs-lookup"><span data-stu-id="7c27f-188">**Property**</span></span>|<span data-ttu-id="7c27f-189">**Typ**</span><span class="sxs-lookup"><span data-stu-id="7c27f-189">**Type**</span></span>|<span data-ttu-id="7c27f-190">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="7c27f-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7c27f-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7c27f-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="7c27f-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7c27f-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="7c27f-193">Ein Array aus erweiterten mehrwertigen Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="7c27f-193">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="7c27f-194">id</span><span class="sxs-lookup"><span data-stu-id="7c27f-194">id</span></span>|<span data-ttu-id="7c27f-195">String</span><span class="sxs-lookup"><span data-stu-id="7c27f-195">String</span></span>|<span data-ttu-id="7c27f-p104">Geben Sie diese für jede Eigenschaft in der **singleValueExtendedProperties**-Sammlung an, um die Eigenschaft zu identifizieren. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c27f-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="7c27f-200">value</span><span class="sxs-lookup"><span data-stu-id="7c27f-200">value</span></span>|<span data-ttu-id="7c27f-201">string</span><span class="sxs-lookup"><span data-stu-id="7c27f-201">string</span></span>|<span data-ttu-id="7c27f-p105">Geben Sie für jede Eigenschaft in der **singleValueExtendedProperties**-Sammlung den Eigenschaftswert an. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c27f-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="7c27f-204">Beim Erstellen einer erweiterten Eigenschaft in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu der neuen **singleValueExtendedProperties**-Sammlung eine JSON-Darstellung der betreffenden Ressourceninstanz spezifizieren (d. h. eine Ressource des Typs [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) usw.).</span><span class="sxs-lookup"><span data-stu-id="7c27f-204">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="7c27f-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c27f-205">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="7c27f-206">Antwortcode</span><span class="sxs-lookup"><span data-stu-id="7c27f-206">Response code</span></span>
<span data-ttu-id="7c27f-207">Ist die Operation zur Erstellung einer erweiterten Eigenschaft in einer neuen Ressourceninstanz erfolgreich, wird `201 Created` zurückgegeben. Ausnahme: In einem neuen Gruppenbeitrag kann die Operation je nach verwendeter Methode `200 OK` oder `202 Accepted` zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="7c27f-207">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="7c27f-208">Eine erfolgreiche Erstellungsoperation in einer vorhandenen Ressourceninstanz gibt `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="7c27f-208">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="7c27f-209">Antworttext</span><span class="sxs-lookup"><span data-stu-id="7c27f-209">Response body</span></span>

<span data-ttu-id="7c27f-p106">Wenn Sie eine erweiterte Eigenschaft erstellen, enthält die Antwort nur die neue oder bereits vorhandene Instanz, nicht jedoch die neue erweiterte Eigenschaft. Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Instanz abrufen](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="7c27f-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="7c27f-212">Beim Erstellen einer erweiterten Eigenschaft in einem _neuen_ [Gruppenbeitrag](../resources/post.md) durch Antwort auf einen Thread oder Beitrag enthält die Antwort nur einen Antwortcode, nicht aber den neuen Beitrag oder die erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="7c27f-212">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="7c27f-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c27f-213">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="7c27f-214">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="7c27f-214">Request 1</span></span>

<span data-ttu-id="7c27f-p107">Im ersten Beispiel wird mit einer einzigen POST-Operation ein neuer Ereignis und eine einwertige erweiterte Eigenschaft erstellt. Abgesehen von den Eigenschaften, die Sie normalerweise für ein neues Ereignis definieren würden, enthält der Anforderungstext die **singleValueExtendedProperties**-Sammlung. Diese wiederum enthält eine erweiterte einwertige Eigenschaft und folgende Angaben für die Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="7c27f-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>

- <span data-ttu-id="7c27f-217">**ID** Gibt den Eigenschaftstyp als `String`, die GUID und die Eigenschaft mit dem Namen `Fun` an.</span><span class="sxs-lookup"><span data-stu-id="7c27f-217">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="7c27f-218">**Wert** Gibt `Food` als den Wert der `Fun`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="7c27f-218">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="7c27f-219">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="7c27f-219">Response 1</span></span>

<span data-ttu-id="7c27f-p108">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 201 Created` gekennzeichnet und enthält das neue Ereignis im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [nur ein Ereignis erstellen](../api/user-post-events.md). Die Antwort enthält keine neu erstellten erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="7c27f-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="7c27f-222">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie das um die erweiterte Eigenschaft erweiterte Ereignis abrufen](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="7c27f-222">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="7c27f-223">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="7c27f-223">Request 2</span></span>

<span data-ttu-id="7c27f-p109">Das zweite Beispiel erstellt eine einwertige erweiterte Eigenschaft für die angegebene vorhandene Nachricht. Diese erweiterte Eigenschaft ist das einzige Element in dem **singleValueExtendedProperties**-Array. Der Anforderungstext enthält die folgenden Parameter für diese erweiterte Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="7c27f-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="7c27f-227">**ID** Gibt den Eigenschaftstyp als `String`, die GUID und die `Color`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="7c27f-227">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="7c27f-228">**Wert** Gibt `Green` als den Wert der `Color`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="7c27f-228">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="7c27f-229">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="7c27f-229">Response 2</span></span>

<span data-ttu-id="7c27f-p110">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 200 OK` gekennzeichnet und enthält die angegebene Nachricht im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [eine Nachricht aktualisieren](../api/message-update.md). Die Antwort enthält nicht die neu erstellte erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="7c27f-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="7c27f-232">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Nachricht abrufen](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="7c27f-232">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

