---
title: Mehrwertige erweiterte Eigenschaft erstellen
description: 'In diesem Artikel erläutern wir Ihnen,wie Sie eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource erstellen können. '
localization_priority: Normal
ms.openlocfilehash: 54be6f428ac5d7b604093fdad3a03b48b89243a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863049"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="12b82-103">Mehrwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="12b82-103">Create multi-value extended property</span></span>

> <span data-ttu-id="12b82-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12b82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12b82-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12b82-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12b82-106">In diesem Artikel erläutern wir Ihnen,wie Sie eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource erstellen können.</span><span class="sxs-lookup"><span data-stu-id="12b82-106">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="12b82-107">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="12b82-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="12b82-108">calendar</span><span class="sxs-lookup"><span data-stu-id="12b82-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="12b82-109">contact</span><span class="sxs-lookup"><span data-stu-id="12b82-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="12b82-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="12b82-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="12b82-111">Ereignis</span><span class="sxs-lookup"><span data-stu-id="12b82-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="12b82-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="12b82-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="12b82-113">message</span><span class="sxs-lookup"><span data-stu-id="12b82-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="12b82-114">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="12b82-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="12b82-115">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="12b82-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="12b82-116">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="12b82-116">As well as the following group resources:</span></span>

- <span data-ttu-id="12b82-117">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="12b82-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="12b82-118">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="12b82-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="12b82-119">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="12b82-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="12b82-120">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="12b82-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="12b82-121">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="12b82-121">Permissions</span></span>
<span data-ttu-id="12b82-122">Erstellen Sie je nach der Ressource in die erweiterte Eigenschaft und die Berechtigung geben (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="12b82-122">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="12b82-123">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12b82-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12b82-124">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="12b82-124">Supported resource</span></span> | <span data-ttu-id="12b82-125">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12b82-125">Delegated (work or school account)</span></span> | <span data-ttu-id="12b82-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12b82-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12b82-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12b82-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="12b82-128">Kalender</span><span class="sxs-lookup"><span data-stu-id="12b82-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="12b82-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="12b82-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-130">Calendars.ReadWrite</span></span> | <span data-ttu-id="12b82-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-131">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="12b82-132">Kontakt</span><span class="sxs-lookup"><span data-stu-id="12b82-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="12b82-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="12b82-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="12b82-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-135">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="12b82-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="12b82-136">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="12b82-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="12b82-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-138">Contacts.ReadWrite</span></span> | <span data-ttu-id="12b82-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-139">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="12b82-140">event</span><span class="sxs-lookup"><span data-stu-id="12b82-140">event</span></span>](../resources/event.md) | <span data-ttu-id="12b82-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-141">Calendars.ReadWrite</span></span> | <span data-ttu-id="12b82-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-142">Calendars.ReadWrite</span></span> |  <span data-ttu-id="12b82-143">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-143">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="12b82-144">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="12b82-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="12b82-145">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b82-145">Group.ReadWrite.All</span></span> | <span data-ttu-id="12b82-146">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12b82-146">Not supported</span></span> | <span data-ttu-id="12b82-147">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12b82-147">Not supported</span></span> |
| <span data-ttu-id="12b82-148">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="12b82-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="12b82-149">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b82-149">Group.ReadWrite.All</span></span> | <span data-ttu-id="12b82-150">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12b82-150">Not supported</span></span> | <span data-ttu-id="12b82-151">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12b82-151">Not supported</span></span> |
| <span data-ttu-id="12b82-152">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="12b82-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="12b82-153">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b82-153">Group.ReadWrite.All</span></span> | <span data-ttu-id="12b82-154">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12b82-154">Not supported</span></span> | <span data-ttu-id="12b82-155">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12b82-155">Not supported</span></span> |
| [<span data-ttu-id="12b82-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="12b82-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="12b82-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-157">Mail.ReadWrite</span></span> | <span data-ttu-id="12b82-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-158">Mail.ReadWrite</span></span> | <span data-ttu-id="12b82-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-159">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="12b82-160">message</span><span class="sxs-lookup"><span data-stu-id="12b82-160">message</span></span>](../resources/message.md) | <span data-ttu-id="12b82-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-161">Mail.ReadWrite</span></span> | <span data-ttu-id="12b82-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-162">Mail.ReadWrite</span></span> | <span data-ttu-id="12b82-163">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-163">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="12b82-164">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="12b82-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="12b82-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="12b82-166">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-166">Tasks.ReadWrite</span></span> | <span data-ttu-id="12b82-167">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12b82-167">Not supported</span></span> |
| [<span data-ttu-id="12b82-168">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="12b82-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="12b82-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="12b82-170">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b82-170">Tasks.ReadWrite</span></span> | <span data-ttu-id="12b82-171">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12b82-171">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="12b82-172">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12b82-172">HTTP request</span></span>
<span data-ttu-id="12b82-173">Sie können erweiterte Eigenschaften in einer neuen oder vorhandenen Ressourceninstanz erstellen.</span><span class="sxs-lookup"><span data-stu-id="12b82-173">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="12b82-174">Um eine oder mehrere erweiterte Eigenschaften in einer _neuen_ Instanz der Ressource zu erstellen, verwenden Sie die gleiche REST-Anforderung als die Instanz erstellt und enthalten Sie die Eigenschaften für die neue Ressource Instanz _und erweiterte Eigenschaft_ im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="12b82-174">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="12b82-175">Beachten Sie, dass einige Ressourcen in mehr als eine Möglichkeit der Erstellung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12b82-175">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="12b82-176">Weitere Informationen zum Erstellen dieser Ressourceninstanzen, finden Sie unter den entsprechenden Themen für die Erstellung einer [Nachricht](../resources/message.md), [MailFolder](../api/user-post-mailfolders.md), [Ereignis](../api/user-post-events.md), [Kalender](../api/user-post-calendars.md), [wenden Sie sich an](../api/user-post-contacts.md), [ContactFolder](../api/user-post-contactfolders.md), [Outlook-Aufgabe](../resources/outlooktask.md), [ Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md), [Gruppe Ereignis](../api/group-post-events.md)und [Gruppe Post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="12b82-176">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="12b82-177">So sieht die Syntax der Anforderungen aus:</span><span class="sxs-lookup"><span data-stu-id="12b82-177">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="12b82-178">Um eine oder mehrere erweiterte Eigenschaften in einer vorhandenen Ressourceninstanz zu erstellen,müssen Sie die Instanz in der Anforderung angeben und die erweiterte-Eigenschaft zum Anforderungstext hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="12b82-178">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="12b82-179">**Hinweis:** Sie können keine erweiterte Eigenschaft in einem vorhandenen Gruppenbeitrag erstellen.</span><span class="sxs-lookup"><span data-stu-id="12b82-179">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="12b82-180">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12b82-180">Request headers</span></span>
| <span data-ttu-id="12b82-181">Name</span><span class="sxs-lookup"><span data-stu-id="12b82-181">Name</span></span>       | <span data-ttu-id="12b82-182">Wert</span><span class="sxs-lookup"><span data-stu-id="12b82-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="12b82-183">Authorization</span><span class="sxs-lookup"><span data-stu-id="12b82-183">Authorization</span></span> | <span data-ttu-id="12b82-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12b82-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12b82-186">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12b82-186">Content-Type</span></span> | <span data-ttu-id="12b82-187">application/json</span><span class="sxs-lookup"><span data-stu-id="12b82-187">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="12b82-188">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12b82-188">Request body</span></span>

<span data-ttu-id="12b82-189">Geben Sie einen JSON-Text für jedes [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekt in der **multiValueExtendedProperties**-Sammlung der Ressourceninstanz an.</span><span class="sxs-lookup"><span data-stu-id="12b82-189">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="12b82-190">**Eigenschaft**</span><span class="sxs-lookup"><span data-stu-id="12b82-190">**Property**</span></span>|<span data-ttu-id="12b82-191">**Typ**</span><span class="sxs-lookup"><span data-stu-id="12b82-191">**Type**</span></span>|<span data-ttu-id="12b82-192">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="12b82-192">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="12b82-193">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="12b82-193">multiValueExtendedProperties</span></span>|<span data-ttu-id="12b82-194">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="12b82-194">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="12b82-195">Ein Array aus einer oder mehreren mehrwertigen erweiterten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="12b82-195">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="12b82-196">id</span><span class="sxs-lookup"><span data-stu-id="12b82-196">id</span></span>|<span data-ttu-id="12b82-197">String</span><span class="sxs-lookup"><span data-stu-id="12b82-197">String</span></span>|<span data-ttu-id="12b82-p105">Geben Sie diesen Parameter für jede Eigenschaft in der **multiValueExtendedProperties**-Sammlung an, um die Eigenschaft zu identifizieren. Der Parameter muss einem der unterstützten Formate entsprechen. Weitere Informationen finden Sie unter [Outlook extended properties overview](../resources/extended-properties-overview.md) (Überblick über erweiterte Outlook-Eigenschaften). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12b82-p105">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="12b82-202">value</span><span class="sxs-lookup"><span data-stu-id="12b82-202">value</span></span>|<span data-ttu-id="12b82-203">string</span><span class="sxs-lookup"><span data-stu-id="12b82-203">string</span></span>|<span data-ttu-id="12b82-p106">Geben Sie für jede Eigenschaft in der **multiValueExtendedProperties**-Sammlung den Eigenschaftswert an. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12b82-p106">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="12b82-206">Beim Erstellen einer erweiterten Eigenschaft in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu der neuen **multiValueExtendedProperties**-Sammlung eine JSON-Darstellung der betreffenden Ressourceninstanz angeben (d. h. eine Ressource des Typs [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) usw.).</span><span class="sxs-lookup"><span data-stu-id="12b82-206">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="12b82-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="12b82-207">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="12b82-208">Antwortcode</span><span class="sxs-lookup"><span data-stu-id="12b82-208">Response code</span></span>
<span data-ttu-id="12b82-209">Ist die Operation zur Erstellung einer erweiterten Eigenschaft in einer neuen Ressourceninstanz erfolgreich, wird `201 Created` zurückgegeben. Ausnahme: In einem neuen Gruppenbeitrag kann die Operation je nach verwendeter Methode `200 OK` oder `202 Accepted` zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="12b82-209">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="12b82-210">Eine erfolgreiche Erstellungsoperation in einer vorhandenen Ressourceninstanz gibt `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="12b82-210">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="12b82-211">Antworttext</span><span class="sxs-lookup"><span data-stu-id="12b82-211">Response body</span></span>

<span data-ttu-id="12b82-p107">Für alle unterstützten Ressourcen außer [Gruppenbeiträge](../resources/post.md) gilt: Wenn Sie eine erweiterte Eigenschaft erstellen, enthält die Antwort nur die neue oder bereits vorhandene Instanz, nicht jedoch die neue erweiterte Eigenschaft. Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Instanz abrufen](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="12b82-p107">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="12b82-p108">Beim Erstellen einer erweiterten Eigenschaft in einem _neuen_ Gruppenbeitrag enthält die Antwort nur einen Antwortcode, nicht aber den neuen Beitrag oder die erweiterte Eigenschaft. In bereits vorhandenen Gruppenbeiträgen können Sie keine erweiterten Eigenschaften erstellen.</span><span class="sxs-lookup"><span data-stu-id="12b82-p108">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="12b82-216">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12b82-216">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="12b82-217">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="12b82-217">Request 1</span></span>

<span data-ttu-id="12b82-p109">Im ersten Beispiel wird mit einer einzigen POST-Operation eine mehrwertige erweiterte Eigenschaft in einem neuen Ereignis erstellt. Abgesehen von den Eigenschaften, die Sie normalerweise für ein neues Ereignis definieren würden, enthält der Anforderungstext die **multiValueExtendedProperties**-Sammlung. Diese wiederum enthält eine erweiterte Eigenschaft. Der Anforderungstext enthält die folgenden Parameter für diese mehrwertige erweiterte Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="12b82-p109">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="12b82-221">**id**: Dieser Parameter definiert die Eigenschaft als ein Array von Zeichenfolgen mit der angegebenen GUID und dem Namen `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="12b82-221">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="12b82-222">**value**: Dieser Parameter definiert `Recreation` als ein Array von 3 Zeichenfolgewerten, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="12b82-222">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="12b82-223">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="12b82-223">Response 1</span></span>

<span data-ttu-id="12b82-p110">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 201 Created` gekennzeichnet und enthält das neue Ereignis im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [nur ein Ereignis erstellen](../api/user-post-events.md). Die Antwort enthält keine neu erstellten erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="12b82-p110">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="12b82-226">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie das um die erweiterte Eigenschaft erweiterte Ereignis abrufen](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="12b82-226">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="12b82-227">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="12b82-227">Request 2</span></span>

<span data-ttu-id="12b82-p111">Das zweite Beispiel erstellt eine mehrwertige erweiterte Eigenschaft für die angegebene Nachricht. Diese erweiterte Eigenschaft ist das einzige Element in der **multiValueExtendedProperties**-Sammlung. Der Anforderungstext enthält die folgenden Parameter für diese erweiterte Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="12b82-p111">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="12b82-231">**id**: Dieser Parameter definiert die Eigenschaft als ein Array von Zeichenfolgen mit der angegebenen GUID und dem Namen `Palette`.</span><span class="sxs-lookup"><span data-stu-id="12b82-231">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="12b82-232">**value**: Dieser Parameter definiert `Palette` als ein Array von 3 Zeichenfolgewerten, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="12b82-232">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="12b82-233">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="12b82-233">Response 2</span></span>

<span data-ttu-id="12b82-p112">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 200 OK` gekennzeichnet und enthält die angegebene Nachricht im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [eine Nachricht aktualisieren](../api/message-update.md). Die Antwort enthält nicht die neu erstellte erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="12b82-p112">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="12b82-236">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Nachricht abrufen](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="12b82-236">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


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




