---
title: Mehrwertige erweiterte Eigenschaft erstellen
description: 'In diesem Artikel erläutern wir Ihnen,wie Sie eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource erstellen können. '
localization_priority: Normal
ms.openlocfilehash: ba54bc3de2eb80fd7283f1a313448b77a04bbe4d
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642254"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="ed648-103">Mehrwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="ed648-103">Create multi-value extended property</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed648-104">In diesem Artikel erläutern wir Ihnen,wie Sie eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource erstellen können.</span><span class="sxs-lookup"><span data-stu-id="ed648-104">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="ed648-105">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="ed648-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="ed648-106">calendar</span><span class="sxs-lookup"><span data-stu-id="ed648-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="ed648-107">contact</span><span class="sxs-lookup"><span data-stu-id="ed648-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="ed648-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ed648-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="ed648-109">event</span><span class="sxs-lookup"><span data-stu-id="ed648-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="ed648-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="ed648-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="ed648-111">message</span><span class="sxs-lookup"><span data-stu-id="ed648-111">message</span></span>](../resources/message.md)
- [<span data-ttu-id="ed648-112">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="ed648-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="ed648-113">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="ed648-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="ed648-114">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="ed648-114">As well as the following group resources:</span></span>

- <span data-ttu-id="ed648-115">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="ed648-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="ed648-116">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="ed648-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="ed648-117">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="ed648-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="ed648-118">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="ed648-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed648-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ed648-119">Permissions</span></span>
<span data-ttu-id="ed648-120">Erstellen Sie je nach der Ressource in die erweiterte Eigenschaft und die Berechtigung geben (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="ed648-120">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="ed648-121">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed648-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed648-122">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="ed648-122">Supported resource</span></span> | <span data-ttu-id="ed648-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed648-123">Delegated (work or school account)</span></span> | <span data-ttu-id="ed648-124">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed648-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed648-125">Application</span><span class="sxs-lookup"><span data-stu-id="ed648-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="ed648-126">Kalender</span><span class="sxs-lookup"><span data-stu-id="ed648-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="ed648-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="ed648-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="ed648-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-129">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="ed648-130">Kontakt</span><span class="sxs-lookup"><span data-stu-id="ed648-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="ed648-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="ed648-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="ed648-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="ed648-134">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ed648-134">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="ed648-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="ed648-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="ed648-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-137">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="ed648-138">event</span><span class="sxs-lookup"><span data-stu-id="ed648-138">event</span></span>](../resources/event.md) | <span data-ttu-id="ed648-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-139">Calendars.ReadWrite</span></span> | <span data-ttu-id="ed648-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-140">Calendars.ReadWrite</span></span> |  <span data-ttu-id="ed648-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-141">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="ed648-142">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="ed648-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="ed648-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed648-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="ed648-144">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed648-144">Not supported</span></span> | <span data-ttu-id="ed648-145">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed648-145">Not supported</span></span> |
| <span data-ttu-id="ed648-146">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="ed648-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="ed648-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed648-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="ed648-148">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed648-148">Not supported</span></span> | <span data-ttu-id="ed648-149">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed648-149">Not supported</span></span> |
| <span data-ttu-id="ed648-150">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="ed648-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="ed648-151">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed648-151">Group.ReadWrite.All</span></span> | <span data-ttu-id="ed648-152">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed648-152">Not supported</span></span> | <span data-ttu-id="ed648-153">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed648-153">Not supported</span></span> |
| [<span data-ttu-id="ed648-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="ed648-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="ed648-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-155">Mail.ReadWrite</span></span> | <span data-ttu-id="ed648-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-156">Mail.ReadWrite</span></span> | <span data-ttu-id="ed648-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-157">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="ed648-158">message</span><span class="sxs-lookup"><span data-stu-id="ed648-158">message</span></span>](../resources/message.md) | <span data-ttu-id="ed648-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-159">Mail.ReadWrite</span></span> | <span data-ttu-id="ed648-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-160">Mail.ReadWrite</span></span> | <span data-ttu-id="ed648-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-161">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="ed648-162">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="ed648-162">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="ed648-163">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-163">Tasks.ReadWrite</span></span> | <span data-ttu-id="ed648-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="ed648-165">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed648-165">Not supported</span></span> |
| [<span data-ttu-id="ed648-166">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="ed648-166">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="ed648-167">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-167">Tasks.ReadWrite</span></span> | <span data-ttu-id="ed648-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed648-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="ed648-169">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed648-169">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed648-170">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed648-170">HTTP request</span></span>
<span data-ttu-id="ed648-171">Sie können erweiterte Eigenschaften in einer neuen oder vorhandenen Ressourceninstanz erstellen.</span><span class="sxs-lookup"><span data-stu-id="ed648-171">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="ed648-172">Um eine oder mehrere erweiterte Eigenschaften in einer _neuen_ Instanz der Ressource zu erstellen, verwenden Sie die gleiche REST-Anforderung als die Instanz erstellt und enthalten Sie die Eigenschaften für die neue Ressource Instanz _und erweiterte Eigenschaft_ im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed648-172">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="ed648-173">Beachten Sie, dass einige Ressourcen in mehr als eine Möglichkeit der Erstellung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed648-173">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="ed648-174">Weitere Informationen zum Erstellen dieser Ressourceninstanzen, finden Sie unter den entsprechenden Themen für die Erstellung einer [Nachricht](../resources/message.md), [MailFolder](../api/user-post-mailfolders.md), [Ereignis](../api/user-post-events.md), [Kalender](../api/user-post-calendars.md), [wenden Sie sich an](../api/user-post-contacts.md), [ContactFolder](../api/user-post-contactfolders.md), [Outlook-Aufgabe](../resources/outlooktask.md), [ Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md), [Gruppe Ereignis](../api/group-post-events.md)und [Gruppe Post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="ed648-174">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="ed648-175">So sieht die Syntax der Anforderungen aus:</span><span class="sxs-lookup"><span data-stu-id="ed648-175">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="ed648-176">Um eine oder mehrere erweiterte Eigenschaften in einer vorhandenen Ressourceninstanz zu erstellen,müssen Sie die Instanz in der Anforderung angeben und die erweiterte-Eigenschaft zum Anforderungstext hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="ed648-176">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="ed648-177">**Hinweis:** Sie können keine erweiterte Eigenschaft in einem vorhandenen Gruppenbeitrag erstellen.</span><span class="sxs-lookup"><span data-stu-id="ed648-177">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="ed648-178">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed648-178">Request headers</span></span>
| <span data-ttu-id="ed648-179">Name</span><span class="sxs-lookup"><span data-stu-id="ed648-179">Name</span></span>       | <span data-ttu-id="ed648-180">Wert</span><span class="sxs-lookup"><span data-stu-id="ed648-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ed648-181">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed648-181">Authorization</span></span> | <span data-ttu-id="ed648-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed648-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed648-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed648-184">Content-Type</span></span> | <span data-ttu-id="ed648-185">application/json</span><span class="sxs-lookup"><span data-stu-id="ed648-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed648-186">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed648-186">Request body</span></span>

<span data-ttu-id="ed648-187">Geben Sie einen JSON-Text für jedes [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekt in der **multiValueExtendedProperties**-Sammlung der Ressourceninstanz an.</span><span class="sxs-lookup"><span data-stu-id="ed648-187">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="ed648-188">**Eigenschaft**</span><span class="sxs-lookup"><span data-stu-id="ed648-188">**Property**</span></span>|<span data-ttu-id="ed648-189">**Typ**</span><span class="sxs-lookup"><span data-stu-id="ed648-189">**Type**</span></span>|<span data-ttu-id="ed648-190">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="ed648-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ed648-191">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ed648-191">multiValueExtendedProperties</span></span>|<span data-ttu-id="ed648-192">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="ed648-192">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ed648-193">Ein Array aus einer oder mehreren mehrwertigen erweiterten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ed648-193">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="ed648-194">id</span><span class="sxs-lookup"><span data-stu-id="ed648-194">id</span></span>|<span data-ttu-id="ed648-195">String</span><span class="sxs-lookup"><span data-stu-id="ed648-195">String</span></span>|<span data-ttu-id="ed648-p104">Geben Sie diesen Parameter für jede Eigenschaft in der **multiValueExtendedProperties**-Sammlung an, um die Eigenschaft zu identifizieren. Der Parameter muss einem der unterstützten Formate entsprechen. Weitere Informationen finden Sie unter [Outlook extended properties overview](../resources/extended-properties-overview.md) (Überblick über erweiterte Outlook-Eigenschaften). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed648-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="ed648-200">value</span><span class="sxs-lookup"><span data-stu-id="ed648-200">value</span></span>|<span data-ttu-id="ed648-201">string</span><span class="sxs-lookup"><span data-stu-id="ed648-201">string</span></span>|<span data-ttu-id="ed648-p105">Geben Sie für jede Eigenschaft in der **multiValueExtendedProperties**-Sammlung den Eigenschaftswert an. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed648-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="ed648-204">Beim Erstellen einer erweiterten Eigenschaft in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu der neuen **multiValueExtendedProperties**-Sammlung eine JSON-Darstellung der betreffenden Ressourceninstanz angeben (d. h. eine Ressource des Typs [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) usw.).</span><span class="sxs-lookup"><span data-stu-id="ed648-204">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="ed648-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed648-205">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="ed648-206">Antwortcode</span><span class="sxs-lookup"><span data-stu-id="ed648-206">Response code</span></span>
<span data-ttu-id="ed648-207">Ist die Operation zur Erstellung einer erweiterten Eigenschaft in einer neuen Ressourceninstanz erfolgreich, wird `201 Created` zurückgegeben. Ausnahme: In einem neuen Gruppenbeitrag kann die Operation je nach verwendeter Methode `200 OK` oder `202 Accepted` zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="ed648-207">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="ed648-208">Eine erfolgreiche Erstellungsoperation in einer vorhandenen Ressourceninstanz gibt `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="ed648-208">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="ed648-209">Antworttext</span><span class="sxs-lookup"><span data-stu-id="ed648-209">Response body</span></span>

<span data-ttu-id="ed648-p106">Für alle unterstützten Ressourcen außer [Gruppenbeiträge](../resources/post.md) gilt: Wenn Sie eine erweiterte Eigenschaft erstellen, enthält die Antwort nur die neue oder bereits vorhandene Instanz, nicht jedoch die neue erweiterte Eigenschaft. Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Instanz abrufen](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="ed648-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="ed648-p107">Beim Erstellen einer erweiterten Eigenschaft in einem _neuen_ Gruppenbeitrag enthält die Antwort nur einen Antwortcode, nicht aber den neuen Beitrag oder die erweiterte Eigenschaft. In bereits vorhandenen Gruppenbeiträgen können Sie keine erweiterten Eigenschaften erstellen.</span><span class="sxs-lookup"><span data-stu-id="ed648-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="ed648-214">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed648-214">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="ed648-215">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="ed648-215">Request 1</span></span>

<span data-ttu-id="ed648-p108">Im ersten Beispiel wird mit einer einzigen POST-Operation eine mehrwertige erweiterte Eigenschaft in einem neuen Ereignis erstellt. Abgesehen von den Eigenschaften, die Sie normalerweise für ein neues Ereignis definieren würden, enthält der Anforderungstext die **multiValueExtendedProperties**-Sammlung. Diese wiederum enthält eine erweiterte Eigenschaft. Der Anforderungstext enthält die folgenden Parameter für diese mehrwertige erweiterte Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="ed648-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="ed648-219">**id**: Dieser Parameter definiert die Eigenschaft als ein Array von Zeichenfolgen mit der angegebenen GUID und dem Namen `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="ed648-219">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="ed648-220">**value**: Dieser Parameter definiert `Recreation` als ein Array von 3 Zeichenfolgewerten, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="ed648-220">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

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

##### <a name="response-1"></a><span data-ttu-id="ed648-221">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="ed648-221">Response 1</span></span>

<span data-ttu-id="ed648-p109">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 201 Created` gekennzeichnet und enthält das neue Ereignis im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [nur ein Ereignis erstellen](../api/user-post-events.md). Die Antwort enthält keine neu erstellten erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="ed648-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="ed648-224">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie das um die erweiterte Eigenschaft erweiterte Ereignis abrufen](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="ed648-224">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="ed648-225">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="ed648-225">Request 2</span></span>

<span data-ttu-id="ed648-p110">Das zweite Beispiel erstellt eine mehrwertige erweiterte Eigenschaft für die angegebene Nachricht. Diese erweiterte Eigenschaft ist das einzige Element in der **multiValueExtendedProperties**-Sammlung. Der Anforderungstext enthält die folgenden Parameter für diese erweiterte Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="ed648-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="ed648-229">**id**: Dieser Parameter definiert die Eigenschaft als ein Array von Zeichenfolgen mit der angegebenen GUID und dem Namen `Palette`.</span><span class="sxs-lookup"><span data-stu-id="ed648-229">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="ed648-230">**value**: Dieser Parameter definiert `Palette` als ein Array von 3 Zeichenfolgewerten, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="ed648-230">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="ed648-231">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="ed648-231">Response 2</span></span>

<span data-ttu-id="ed648-p111">Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 200 OK` gekennzeichnet und enthält die angegebene Nachricht im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [eine Nachricht aktualisieren](../api/message-update.md). Die Antwort enthält nicht die neu erstellte erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="ed648-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="ed648-234">Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Nachricht abrufen](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="ed648-234">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


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
    "Error: /api-reference/beta/api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->




