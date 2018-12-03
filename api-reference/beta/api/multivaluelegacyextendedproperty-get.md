---
title: Get multiValueLegacyExtendedProperty
description: Erweitern Sie ".
ms.openlocfilehash: 9429737f3965acbf4c6bcc61c516327556223111
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063188"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="92496-103">Get multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="92496-103">Get multiValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="92496-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="92496-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92496-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92496-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92496-106">Dient zum Abrufen einer Ressourceninstanz mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="92496-106">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="92496-107">Mit dem Abfrageparameter `$expand` können Sie die angegebene Instanz abrufen, erweitert um die angegebene erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="92496-107">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="92496-108">Dies ist derzeit die einzige Möglichkeit zum Abrufen des [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="92496-108">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="92496-109">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="92496-109">The following user resources are supported:</span></span>

- [<span data-ttu-id="92496-110">calendar</span><span class="sxs-lookup"><span data-stu-id="92496-110">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="92496-111">contact</span><span class="sxs-lookup"><span data-stu-id="92496-111">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="92496-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="92496-112">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="92496-113">Ereignis</span><span class="sxs-lookup"><span data-stu-id="92496-113">event</span></span>](../resources/event.md)
- [<span data-ttu-id="92496-114">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92496-114">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="92496-115">Nachricht</span><span class="sxs-lookup"><span data-stu-id="92496-115">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="92496-116">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="92496-116">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="92496-117">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="92496-117">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="92496-118">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="92496-118">As well as the following group resources:</span></span>

- <span data-ttu-id="92496-119">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="92496-119">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="92496-120">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="92496-120">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="92496-121">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="92496-121">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="92496-122">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="92496-122">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="92496-123">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="92496-123">Permissions</span></span>
<span data-ttu-id="92496-124">Je nach der Ressource kommen die erweiterte Eigenschaft aus und geben Sie die Berechtigung (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="92496-124">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="92496-125">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92496-125">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92496-126">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="92496-126">Supported resource</span></span> | <span data-ttu-id="92496-127">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92496-127">Delegated (work or school account)</span></span> | <span data-ttu-id="92496-128">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92496-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92496-129">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92496-129">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="92496-130">Kalender</span><span class="sxs-lookup"><span data-stu-id="92496-130">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="92496-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="92496-131">Calendars.Read</span></span> | <span data-ttu-id="92496-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="92496-132">Calendars.Read</span></span> | <span data-ttu-id="92496-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="92496-133">Calendars.Read</span></span> |
| [<span data-ttu-id="92496-134">Kontakt</span><span class="sxs-lookup"><span data-stu-id="92496-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="92496-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="92496-135">Contacts.Read</span></span> | <span data-ttu-id="92496-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="92496-136">Contacts.Read</span></span> | <span data-ttu-id="92496-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="92496-137">Contacts.Read</span></span> |
| [<span data-ttu-id="92496-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="92496-138">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="92496-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="92496-139">Contacts.Read</span></span> | <span data-ttu-id="92496-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="92496-140">Contacts.Read</span></span> | <span data-ttu-id="92496-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="92496-141">Contacts.Read</span></span> |
| [<span data-ttu-id="92496-142">Ereignis</span><span class="sxs-lookup"><span data-stu-id="92496-142">event</span></span>](../resources/event.md) | <span data-ttu-id="92496-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="92496-143">Calendars.Read</span></span> | <span data-ttu-id="92496-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="92496-144">Calendars.Read</span></span> |  <span data-ttu-id="92496-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="92496-145">Calendars.Read</span></span>|
| <span data-ttu-id="92496-146">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="92496-146">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="92496-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="92496-147">Group.Read.All</span></span> | <span data-ttu-id="92496-148">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92496-148">Not supported</span></span> | <span data-ttu-id="92496-149">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92496-149">Not supported</span></span> |
| <span data-ttu-id="92496-150">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="92496-150">group [event](../resources/event.md)</span></span> | <span data-ttu-id="92496-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="92496-151">Group.Read.All</span></span> | <span data-ttu-id="92496-152">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92496-152">Not supported</span></span> | <span data-ttu-id="92496-153">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92496-153">Not supported</span></span> |
| <span data-ttu-id="92496-154">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="92496-154">group [post](../resources/post.md)</span></span> | <span data-ttu-id="92496-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="92496-155">Group.Read.All</span></span> | <span data-ttu-id="92496-156">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92496-156">Not supported</span></span> | <span data-ttu-id="92496-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="92496-157">Group.Read.All</span></span> |
| [<span data-ttu-id="92496-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="92496-158">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="92496-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="92496-159">Mail.Read</span></span> | <span data-ttu-id="92496-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="92496-160">Mail.Read</span></span> | <span data-ttu-id="92496-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="92496-161">Mail.Read</span></span> |
| [<span data-ttu-id="92496-162">Nachricht</span><span class="sxs-lookup"><span data-stu-id="92496-162">message</span></span>](../resources/message.md) | <span data-ttu-id="92496-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="92496-163">Mail.Read</span></span> | <span data-ttu-id="92496-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="92496-164">Mail.Read</span></span> | <span data-ttu-id="92496-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="92496-165">Mail.Read</span></span> |
| [<span data-ttu-id="92496-166">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="92496-166">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="92496-167">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="92496-167">Tasks.Read</span></span> | <span data-ttu-id="92496-168">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="92496-168">Tasks.Read</span></span> | <span data-ttu-id="92496-169">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92496-169">Not supported</span></span> |
| [<span data-ttu-id="92496-170">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="92496-170">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="92496-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="92496-171">Tasks.Read</span></span> | <span data-ttu-id="92496-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="92496-172">Tasks.Read</span></span> | <span data-ttu-id="92496-173">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92496-173">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="92496-174">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92496-174">HTTP request</span></span>

<span data-ttu-id="92496-p104">Rufen Sie eine erweiterte Ressourceninstanz mit erweiterter Eigenschaft ab, die einem Filter für die **id**-Eigenschaft entspricht. Stellen Sie sicher, dass Sie die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) auf die Leerzeichen in der Filterzeichenfolge anwenden.</span><span class="sxs-lookup"><span data-stu-id="92496-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="92496-177">Erhalten Sie eine Instanz der **Nachricht** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-177">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="92496-178">Eine **MailFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-178">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="92496-179">Rufen Sie eine Instanz **Ereignis** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-179">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="92496-180">Eine **Kalender** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-180">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="92496-181">Abrufen einer Instanz **wenden Sie sich an** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-181">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="92496-182">Eine **ContactFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-182">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="92496-183">Erhalten Sie eine Instanz **OutlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-183">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="92496-184">Erhalten Sie eine Instanz **OutlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-184">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="92496-185">Eine Gruppe **Ereignis** Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-185">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="92496-186">Eine Gruppe **Buchen** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="92496-186">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="92496-187">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="92496-187">Path parameters</span></span>
|<span data-ttu-id="92496-188">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="92496-188">**Parameter**</span></span>|<span data-ttu-id="92496-189">**Typ**</span><span class="sxs-lookup"><span data-stu-id="92496-189">**Type**</span></span>|<span data-ttu-id="92496-190">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="92496-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="92496-191">id_value</span><span class="sxs-lookup"><span data-stu-id="92496-191">id_value</span></span>|<span data-ttu-id="92496-192">String</span><span class="sxs-lookup"><span data-stu-id="92496-192">String</span></span>|<span data-ttu-id="92496-p105">Die ID der erweiterten übereinstimmenden Eigenschaft. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92496-p105">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="92496-197">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92496-197">Request headers</span></span>
| <span data-ttu-id="92496-198">Name</span><span class="sxs-lookup"><span data-stu-id="92496-198">Name</span></span>      |<span data-ttu-id="92496-199">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92496-199">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92496-200">Authorization</span><span class="sxs-lookup"><span data-stu-id="92496-200">Authorization</span></span>  | <span data-ttu-id="92496-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92496-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92496-203">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92496-203">Request body</span></span>
<span data-ttu-id="92496-204">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="92496-204">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92496-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="92496-205">Response</span></span>

<span data-ttu-id="92496-206">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92496-206">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="92496-207">Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, und das übereinstimmende [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="92496-207">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="92496-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92496-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92496-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92496-209">Request</span></span>
<span data-ttu-id="92496-p107">In diesem Beispiel wird das angegebene Ereignis abgerufen und um eine erweiterte mehrwertige Eigenschaften erwetiert. Der Filter gibt die erweiterte Eigenschaft mit der **ID** an, die mit der Zeichenfolge `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` übereinstimmt (URL-Codierung wurde zur besseren Lesbarkeit in diesem Beispiel entfernt).</span><span class="sxs-lookup"><span data-stu-id="92496-p107">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="92496-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="92496-212">Response</span></span>

<span data-ttu-id="92496-213">Der Antworttext enthält alle Eigenschaften des angegebenen Ereignisses und erweiterte Eigenschaften, die von dem Filter zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="92496-213">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="92496-p108">Hinweis: Das hier gezeigte **event**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92496-p108">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->