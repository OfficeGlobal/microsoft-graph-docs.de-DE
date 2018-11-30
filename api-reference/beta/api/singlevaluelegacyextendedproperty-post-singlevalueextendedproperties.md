---
title: Erweiterte einwertige Eigenschaft erstellen
description: 'Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource. '
ms.openlocfilehash: c55ab01ecde214feb38857e8d77f83eb3bfbabc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060107"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="e0409-103">Erweiterte einwertige Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="e0409-103">Create single-value extended property</span></span>

> <span data-ttu-id="e0409-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e0409-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0409-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e0409-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0409-106">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource.</span><span class="sxs-lookup"><span data-stu-id="e0409-106">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="e0409-107">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="e0409-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="e0409-108">calendar</span><span class="sxs-lookup"><span data-stu-id="e0409-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="e0409-109">contact</span><span class="sxs-lookup"><span data-stu-id="e0409-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="e0409-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e0409-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="e0409-111">Ereignis</span><span class="sxs-lookup"><span data-stu-id="e0409-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="e0409-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e0409-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="e0409-113">Nachricht</span><span class="sxs-lookup"><span data-stu-id="e0409-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="e0409-114">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="e0409-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="e0409-115">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="e0409-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="e0409-116">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="e0409-116">As well as the following group resources:</span></span>

- <span data-ttu-id="e0409-117">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="e0409-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="e0409-118">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="e0409-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="e0409-119">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="e0409-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="e0409-120">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e0409-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0409-121">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e0409-121">Permissions</span></span>
<span data-ttu-id="e0409-122">Erstellen Sie je nach der Ressource in die erweiterte Eigenschaft und die Berechtigung geben (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="e0409-122">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="e0409-123">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0409-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0409-124">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="e0409-124">Supported resource</span></span> | <span data-ttu-id="e0409-125">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0409-125">Delegated (work or school account)</span></span> | <span data-ttu-id="e0409-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0409-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0409-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0409-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="e0409-128">Kalender</span><span class="sxs-lookup"><span data-stu-id="e0409-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="e0409-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="e0409-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-130">Calendars.ReadWrite</span></span> | <span data-ttu-id="e0409-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-131">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="e0409-132">Kontakt</span><span class="sxs-lookup"><span data-stu-id="e0409-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e0409-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="e0409-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="e0409-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-135">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="e0409-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e0409-136">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="e0409-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="e0409-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-138">Contacts.ReadWrite</span></span> | <span data-ttu-id="e0409-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-139">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="e0409-140">event</span><span class="sxs-lookup"><span data-stu-id="e0409-140">event</span></span>](../resources/event.md) | <span data-ttu-id="e0409-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-141">Calendars.ReadWrite</span></span> | <span data-ttu-id="e0409-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-142">Calendars.ReadWrite</span></span> |  <span data-ttu-id="e0409-143">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-143">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="e0409-144">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="e0409-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="e0409-145">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0409-145">Group.ReadWrite.All</span></span> | <span data-ttu-id="e0409-146">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0409-146">Not supported</span></span> | <span data-ttu-id="e0409-147">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0409-147">Not supported</span></span> |
| <span data-ttu-id="e0409-148">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="e0409-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="e0409-149">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0409-149">Group.ReadWrite.All</span></span> | <span data-ttu-id="e0409-150">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0409-150">Not supported</span></span> | <span data-ttu-id="e0409-151">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0409-151">Not supported</span></span> |
| <span data-ttu-id="e0409-152">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="e0409-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="e0409-153">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0409-153">Group.ReadWrite.All</span></span> | <span data-ttu-id="e0409-154">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0409-154">Not supported</span></span> | <span data-ttu-id="e0409-155">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0409-155">Not supported</span></span> |
| [<span data-ttu-id="e0409-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e0409-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="e0409-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-157">Mail.ReadWrite</span></span> | <span data-ttu-id="e0409-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-158">Mail.ReadWrite</span></span> | <span data-ttu-id="e0409-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-159">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="e0409-160">message</span><span class="sxs-lookup"><span data-stu-id="e0409-160">message</span></span>](../resources/message.md) | <span data-ttu-id="e0409-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-161">Mail.ReadWrite</span></span> | <span data-ttu-id="e0409-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-162">Mail.ReadWrite</span></span> | <span data-ttu-id="e0409-163">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-163">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="e0409-164">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="e0409-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="e0409-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="e0409-166">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-166">Tasks.ReadWrite</span></span> | <span data-ttu-id="e0409-167">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0409-167">Not supported</span></span> |
| [<span data-ttu-id="e0409-168">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="e0409-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="e0409-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="e0409-170">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-170">Tasks.ReadWrite</span></span> | <span data-ttu-id="e0409-171">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0409-171">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="e0409-172">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0409-172">HTTP request</span></span>
<span data-ttu-id="e0409-173">Sie können erweiterte Eigenschaften in einer neuen oder vorhandenen Ressourceninstanz erstellen.</span><span class="sxs-lookup"><span data-stu-id="e0409-173">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="e0409-174">Um eine oder mehrere erweiterte Eigenschaften in einer _neuen_ Instanz der Ressource zu erstellen, verwenden Sie die gleiche REST-Anforderung als die Instanz erstellt und enthalten Sie die Eigenschaften für die neue Ressource Instanz _und erweiterte Eigenschaft_ im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0409-174">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="e0409-175">Beachten Sie, dass einige Ressourcen in mehr als eine Möglichkeit der Erstellung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e0409-175">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="e0409-176">Weitere Informationen zum Erstellen dieser Ressourceninstanzen, finden Sie unter den entsprechenden Themen für die Erstellung einer [Nachricht](../resources/message.md), [MailFolder](../api/user-post-mailfolders.md), [Ereignis](../api/user-post-events.md), [Kalender](../api/user-post-calendars.md), [wenden Sie sich an](../api/user-post-contacts.md), [ContactFolder](../api/user-post-contactfolders.md), [Outlook-Aufgabe](../resources/outlooktask.md), [ Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md), [Gruppe Ereignis](../api/group-post-events.md)und [Gruppe Post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="e0409-176">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="e0409-177">So sieht die Syntax der Anforderungen aus:</span><span class="sxs-lookup"><span data-stu-id="e0409-177">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="e0409-178">Um eine oder mehrere erweiterte Eigenschaften in einer vorhandenen Ressourceninstanz zu erstellen,müssen Sie die Instanz in der Anforderung angeben und die erweiterte-Eigenschaft zum Anforderungstext hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="e0409-178">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="e0409-179">**Hinweis:** Sie können keine erweiterte Eigenschaft in einem vorhandenen Gruppenbeitrag erstellen.</span><span class="sxs-lookup"><span data-stu-id="e0409-179">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="e0409-180">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0409-180">Request headers</span></span>
| <span data-ttu-id="e0409-181">Name</span><span class="sxs-lookup"><span data-stu-id="e0409-181">Name</span></span>       | <span data-ttu-id="e0409-182">Wert</span><span class="sxs-lookup"><span data-stu-id="e0409-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e0409-183">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0409-183">Authorization</span></span> | <span data-ttu-id="e0409-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0409-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0409-186">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0409-186">Content-Type</span></span> | <span data-ttu-id="e0409-187">application/json</span><span class="sxs-lookup"><span data-stu-id="e0409-187">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0409-188">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0409-188">Request body</span></span>

<span data-ttu-id="e0409-189">Stellen Sie einen JSON-Text für jedes [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekt in der **singleValueExtendedProperties**-Sammlungseigenschaft der Ressourceninstanz bereit.</span><span class="sxs-lookup"><span data-stu-id="e0409-189">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="e0409-190">**Eigenschaft**</span><span class="sxs-lookup"><span data-stu-id="e0409-190">**Property**</span></span>|<span data-ttu-id="e0409-191">**Typ**</span><span class="sxs-lookup"><span data-stu-id="e0409-191">**Type**</span></span>|<span data-ttu-id="e0409-192">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="e0409-192">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e0409-193">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e0409-193">singleValueExtendedProperties</span></span>|<span data-ttu-id="e0409-194">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e0409-194">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e0409-195">Ein Array aus erweiterten mehrwertigen Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="e0409-195">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="e0409-196">id</span><span class="sxs-lookup"><span data-stu-id="e0409-196">id</span></span>|<span data-ttu-id="e0409-197">String</span><span class="sxs-lookup"><span data-stu-id="e0409-197">String</span></span>|<span data-ttu-id="e0409-p105">Geben Sie diese für jede Eigenschaft in der **singleValueExtendedProperties**-Sammlung an, um die Eigenschaft zu identifizieren. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0409-p105">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="e0409-202">value</span><span class="sxs-lookup"><span data-stu-id="e0409-202">value</span></span>|<span data-ttu-id="e0409-203">string</span><span class="sxs-lookup"><span data-stu-id="e0409-203">string</span></span>|<span data-ttu-id="e0409-p106">Geben Sie für jede Eigenschaft in der **singleValueExtendedProperties**-Sammlung den Eigenschaftswert an. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0409-p106">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="e0409-206">Beim Erstellen einer erweiterten Eigenschaft in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu der neuen **singleValueExtendedProperties**-Sammlung eine JSON-Darstellung der betreffenden Ressourceninstanz spezifizieren (d. h. eine Ressource des Typs [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) usw.).</span><span class="sxs-lookup"><span data-stu-id="e0409-206">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="e0409-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0409-207">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="e0409-208">Antwortcode</span><span class="sxs-lookup"><span data-stu-id="e0409-208">Response code</span></span>
<span data-ttu-id="e0409-209">Ist die Operation zur Erstellung einer erweiterten Eigenschaft in einer neuen Ressourceninstanz erfolgreich, wird `201 Created` zurückgegeben. Ausnahme: In einem neuen Gruppenbeitrag kann die Operation je nach verwendeter Methode `200 OK` oder `202 Accepted` zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="e0409-209">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="e0409-210">Eine erfolgreiche Erstellungsoperation in einer vorhandenen Ressourceninstanz gibt `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="e0409-210">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="e0409-211">Antworttext</span><span class="sxs-lookup"><span data-stu-id="e0409-211">Response body</span></span>

<span data-ttu-id="e0409-p107">Wenn Sie eine erweiterte Eigenschaft erstellen, enthält die Antwort nur die neue oder bereits vorhandene Instanz, nicht jedoch die neue erweiterte Eigenschaft. Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Instanz abrufen](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="e0409-p107">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="e0409-214">Beim Erstellen einer erweiterten Eigenschaft in einem _neuen_ [Gruppenbeitrag](../resources/post.md) durch Antwort auf einen Thread oder Beitrag enthält die Antwort nur einen Antwortcode, nicht aber den neuen Beitrag oder die erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="e0409-214">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="e0409-215">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0409-215">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e0409-216">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="e0409-216">Request 1</span></span>

<span data-ttu-id="e0409-p108">Im ersten Beispiel wird mit einer einzigen POST-Operation ein neuer Ereignis und eine einwertige erweiterte Eigenschaft erstellt. Abgesehen von den Eigenschaften, die Sie normalerweise für ein neues Ereignis definieren würden, enthält der Anforderungstext die **singleValueExtendedProperties**-Sammlung. Diese wiederum enthält eine erweiterte einwertige Eigenschaft und folgende Angaben für die Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="e0409-p108">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>

- <span data-ttu-id="e0409-219">**ID** Gibt den Eigenschaftstyp als `String`, die GUID und die Eigenschaft mit dem Namen `Fun` an.</span><span class="sxs-lookup"><span data-stu-id="e0409-219">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="e0409-220">**Wert** Gibt `Food` als den Wert der `Fun`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="e0409-220">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

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

##### <a name="response-1"></a><span data-ttu-id="e0409-221">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="e0409-221">Response 1</span></span>

<span data-ttu-id="e0409-p109">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 201 Created` gekennzeichnet und enthält das neue Ereignis im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [nur ein Ereignis erstellen](../api/user-post-events.md). Die Antwort enthält keine neu erstellten erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="e0409-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="e0409-224">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie das um die erweiterte Eigenschaft erweiterte Ereignis abrufen](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="e0409-224">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="e0409-225">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="e0409-225">Request 2</span></span>

<span data-ttu-id="e0409-p110">Das zweite Beispiel erstellt eine einwertige erweiterte Eigenschaft für die angegebene vorhandene Nachricht. Diese erweiterte Eigenschaft ist das einzige Element in dem **singleValueExtendedProperties**-Array. Der Anforderungstext enthält die folgenden Parameter für diese erweiterte Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="e0409-p110">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="e0409-229">**ID** Gibt den Eigenschaftstyp als `String`, die GUID und die `Color`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="e0409-229">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="e0409-230">**Wert** Gibt `Green` als den Wert der `Color`-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="e0409-230">**value** specifies `Green` as the value of the `Color` property.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="e0409-231">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="e0409-231">Response 2</span></span>

<span data-ttu-id="e0409-p111">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 200 OK` gekennzeichnet und enthält die angegebene Nachricht im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [eine Nachricht aktualisieren](../api/message-update.md). Die Antwort enthält nicht die neu erstellte erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="e0409-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="e0409-234">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Nachricht abrufen](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="e0409-234">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

