---
title: singleValueLegacyExtendedProperty abrufen
description: Sie können eine einzelne Ressourceninstanz erweitert mit einer bestimmten erweiterten Eigenschaft oder eine Auflistung von Resource-Instanzen abzurufen.
ms.openlocfilehash: 72ae071d2c5c92af02d26af2474c776a5dc1c83c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064612"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="aa96d-103">singleValueLegacyExtendedProperty abrufen</span><span class="sxs-lookup"><span data-stu-id="aa96d-103">Get singleValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="aa96d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aa96d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa96d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa96d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa96d-106">Sie können eine einzelne, mit einer bestimmten erweiterten Eigenschaft erweiterte Ressourceninstanz oder eine Sammlung von Ressourceninstanzen abrufen, die einem Filter entsprechende erweiterte Eigenschaften enthalten.</span><span class="sxs-lookup"><span data-stu-id="aa96d-106">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="aa96d-107">Mit dem Abfrageparameter `$expand` können Sie die angegebene Ressourceninstanz, erweitert um die angegebene erweiterte Eigenschaft, abrufen.</span><span class="sxs-lookup"><span data-stu-id="aa96d-107">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="aa96d-108">Wenden Sie einen `$filter`- und einen `eq`-Operator auf die **ID**-Eigenschaft an, um die erweiterte Eigenschaft anzugeben.</span><span class="sxs-lookup"><span data-stu-id="aa96d-108">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="aa96d-109">Dies ist derzeit die einzige Möglichkeit zum Abrufen des [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="aa96d-109">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="aa96d-110">Um Ressourceninstanzen mit bestimmten erweiterten Eigenschaften abzurufen, verwenden Sie den Abfrageparameter `$filter`, und wenden Sie einen `eq`-Operator auf die **ID**-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="aa96d-110">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="aa96d-111">Wenden Sie für nummerische erweiterte Eigenschaften zudem einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `eq`, `ne`,`ge`, `gt`, `le` oder `lt`.</span><span class="sxs-lookup"><span data-stu-id="aa96d-111">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="aa96d-112">Für erweiterte Eigenschaften vom Typ Zeichenfolge wenden Sie einen `contains`-, `startswith`-, `eq`-, oder `ne`-Operator auf den **Wert** an.</span><span class="sxs-lookup"><span data-stu-id="aa96d-112">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="aa96d-113">Beim Filtern des Namens der Zeichenfolge (`Name`) in der **ID** einer erweiterten Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="aa96d-113">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="aa96d-114">Beim Filtern der Eigenschaft **Wert** einer erweiterten Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="aa96d-114">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="aa96d-115">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="aa96d-115">The following user resources are supported:</span></span>

- [<span data-ttu-id="aa96d-116">calendar</span><span class="sxs-lookup"><span data-stu-id="aa96d-116">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="aa96d-117">contact</span><span class="sxs-lookup"><span data-stu-id="aa96d-117">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="aa96d-118">contactFolder</span><span class="sxs-lookup"><span data-stu-id="aa96d-118">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="aa96d-119">Ereignis</span><span class="sxs-lookup"><span data-stu-id="aa96d-119">event</span></span>](../resources/event.md)
- [<span data-ttu-id="aa96d-120">mailFolder</span><span class="sxs-lookup"><span data-stu-id="aa96d-120">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="aa96d-121">Nachricht</span><span class="sxs-lookup"><span data-stu-id="aa96d-121">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="aa96d-122">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="aa96d-122">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="aa96d-123">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="aa96d-123">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="aa96d-124">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="aa96d-124">As well as the following group resources:</span></span>

- <span data-ttu-id="aa96d-125">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="aa96d-125">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="aa96d-126">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="aa96d-126">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="aa96d-127">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="aa96d-127">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="aa96d-128">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="aa96d-128">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa96d-129">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa96d-129">Permissions</span></span>
<span data-ttu-id="aa96d-130">Je nach der Ressource kommen die erweiterte Eigenschaft aus und geben Sie die Berechtigung (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="aa96d-130">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="aa96d-131">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa96d-131">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa96d-132">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="aa96d-132">Supported resource</span></span> | <span data-ttu-id="aa96d-133">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa96d-133">Delegated (work or school account)</span></span> | <span data-ttu-id="aa96d-134">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa96d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa96d-135">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa96d-135">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="aa96d-136">Kalender</span><span class="sxs-lookup"><span data-stu-id="aa96d-136">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="aa96d-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-137">Calendars.Read</span></span> | <span data-ttu-id="aa96d-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-138">Calendars.Read</span></span> | <span data-ttu-id="aa96d-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-139">Calendars.Read</span></span> |
| [<span data-ttu-id="aa96d-140">Kontakt</span><span class="sxs-lookup"><span data-stu-id="aa96d-140">contact</span></span>](../resources/contact.md) | <span data-ttu-id="aa96d-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-141">Contacts.Read</span></span> | <span data-ttu-id="aa96d-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-142">Contacts.Read</span></span> | <span data-ttu-id="aa96d-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-143">Contacts.Read</span></span> |
| [<span data-ttu-id="aa96d-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="aa96d-144">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="aa96d-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-145">Contacts.Read</span></span> | <span data-ttu-id="aa96d-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-146">Contacts.Read</span></span> | <span data-ttu-id="aa96d-147">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-147">Contacts.Read</span></span> |
| [<span data-ttu-id="aa96d-148">Ereignis</span><span class="sxs-lookup"><span data-stu-id="aa96d-148">event</span></span>](../resources/event.md) | <span data-ttu-id="aa96d-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-149">Calendars.Read</span></span> | <span data-ttu-id="aa96d-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-150">Calendars.Read</span></span> |  <span data-ttu-id="aa96d-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-151">Calendars.Read</span></span>|
| <span data-ttu-id="aa96d-152">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="aa96d-152">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="aa96d-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa96d-153">Group.Read.All</span></span> | <span data-ttu-id="aa96d-154">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa96d-154">Not supported</span></span> | <span data-ttu-id="aa96d-155">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa96d-155">Not supported</span></span> |
| <span data-ttu-id="aa96d-156">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="aa96d-156">group [event](../resources/event.md)</span></span> | <span data-ttu-id="aa96d-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa96d-157">Group.Read.All</span></span> | <span data-ttu-id="aa96d-158">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa96d-158">Not supported</span></span> | <span data-ttu-id="aa96d-159">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa96d-159">Not supported</span></span> |
| <span data-ttu-id="aa96d-160">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="aa96d-160">group [post](../resources/post.md)</span></span> | <span data-ttu-id="aa96d-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa96d-161">Group.Read.All</span></span> | <span data-ttu-id="aa96d-162">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa96d-162">Not supported</span></span> | <span data-ttu-id="aa96d-163">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa96d-163">Group.Read.All</span></span> |
| [<span data-ttu-id="aa96d-164">mailFolder</span><span class="sxs-lookup"><span data-stu-id="aa96d-164">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="aa96d-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-165">Mail.Read</span></span> | <span data-ttu-id="aa96d-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-166">Mail.Read</span></span> | <span data-ttu-id="aa96d-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-167">Mail.Read</span></span> |
| [<span data-ttu-id="aa96d-168">Nachricht</span><span class="sxs-lookup"><span data-stu-id="aa96d-168">message</span></span>](../resources/message.md) | <span data-ttu-id="aa96d-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-169">Mail.Read</span></span> | <span data-ttu-id="aa96d-170">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-170">Mail.Read</span></span> | <span data-ttu-id="aa96d-171">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-171">Mail.Read</span></span> |
| [<span data-ttu-id="aa96d-172">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="aa96d-172">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="aa96d-173">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-173">Tasks.Read</span></span> | <span data-ttu-id="aa96d-174">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-174">Tasks.Read</span></span> | <span data-ttu-id="aa96d-175">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa96d-175">Not supported</span></span> |
| [<span data-ttu-id="aa96d-176">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="aa96d-176">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="aa96d-177">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-177">Tasks.Read</span></span> | <span data-ttu-id="aa96d-178">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="aa96d-178">Tasks.Read</span></span> | <span data-ttu-id="aa96d-179">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa96d-179">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="aa96d-180">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa96d-180">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="aa96d-181">Abrufen einer Ressourceninstanz, erweitert um eine erweiterte Eigenschaft, die einem Filter entspricht</span><span class="sxs-lookup"><span data-stu-id="aa96d-181">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="aa96d-p106">Hier sehen Sie, wie Sie eine Ressourceninstanz abrufen können, erweitert um die erweiterte Eigenschaft, deren **id**-Eigenschaft dem definierten Filter entspricht. Stellen Sie sicher, dass Sie für die Leerzeichen in der Filterzeichenfolge die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) verwenden.</span><span class="sxs-lookup"><span data-stu-id="aa96d-p106">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="aa96d-184">Erhalten Sie eine Instanz der **Nachricht** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-184">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="aa96d-185">Eine **MailFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-185">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="aa96d-186">Rufen Sie eine Instanz **Ereignis** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-186">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="aa96d-187">Eine **Kalender** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-187">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="aa96d-188">Abrufen einer Instanz **wenden Sie sich an** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-188">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="aa96d-189">Eine **ContactFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-189">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="aa96d-190">Erhalten Sie eine Instanz **OutlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-190">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="aa96d-191">Erhalten Sie eine Instanz **OutlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-191">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="aa96d-192">Eine Gruppe **Ereignis** Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-192">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="aa96d-193">Eine Gruppe **Buchen** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-193">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="aa96d-194">Abrufen von Ressourceninstanzen, die numerische erweiterte Eigenschaften enthalten, die einem Filter entsprechen</span><span class="sxs-lookup"><span data-stu-id="aa96d-194">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="aa96d-195">Rufen Sie Instanzen einer unterstützten Ressource ab, die eine numerische erweiterte Eigenschaft besitzen, die einem Filter entspricht.</span><span class="sxs-lookup"><span data-stu-id="aa96d-195">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="aa96d-196">Der Filter wendet einen `eq`-Operator auf die **ID**-Eigenschaft und einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `eq`, `ne`,`ge`, `gt` , `le` oder `lt`.</span><span class="sxs-lookup"><span data-stu-id="aa96d-196">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="aa96d-197">Stellen Sie sicher, dass Sie anwenden, stellen Sie sicher, dass Sie auf der folgenden Zeichen in der Filterzeichenfolge - Doppelpunkt, Schrägstrich und Speicherplatz anwenden [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) .</span><span class="sxs-lookup"><span data-stu-id="aa96d-197">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="aa96d-198">Die folgenden Syntaxzeilen zeigen einen Filter, der den `eq`-Operator auf die ID anwendet, und einen `eq`-Operator, der auf den Eigenschaftswert angewandt wird.</span><span class="sxs-lookup"><span data-stu-id="aa96d-198">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="aa96d-199">Sie können den `eq`-Operator, der auf den **Wert** angewandt wird, durch einen der anderen Operatoren (`ne`,`ge`, `gt`, `le` oder `lt`) ersetzen, die auf numerische Werte angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="aa96d-199">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="aa96d-200">**Nachricht** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-200">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="aa96d-201">**MailFolder** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-201">Get **mailFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="aa96d-202">**Ereignis** -Instanzen abzurufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-202">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="aa96d-203">**Kalender** -Instanzen abzurufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-203">Get **calendar** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="aa96d-204">**Wenden Sie sich an** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-204">Get **contact** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="aa96d-205">**ContactFolder** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-205">Get **contactFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="aa96d-206">Erhalten Sie eine Instanz **OutlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-206">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="aa96d-207">Erhalten Sie eine Instanz **OutlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-207">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="aa96d-208">Gruppe **Ereignis** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-208">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="aa96d-209">Gruppe **Buchen** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-209">Get group **post** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="aa96d-210">Abrufen von Ressourceninstanzen mit erweiterten Eigenschaften des Typs Zeichenfolge, die einem Filter entsprechen</span><span class="sxs-lookup"><span data-stu-id="aa96d-210">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="aa96d-211">Rufen Sie Instanzen der Ressource **Nachricht** oder **Ereignis** mit einer erweiterten Eigenschaft des Typs Zeichenfolge ab, die einem Filter entspricht.</span><span class="sxs-lookup"><span data-stu-id="aa96d-211">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="aa96d-212">Der Filter wendet einen `eq`-Operator auf die **ID**-Eigenschaft und einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `contains`, `startswith`, `eq` oder `ne`.</span><span class="sxs-lookup"><span data-stu-id="aa96d-212">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="aa96d-213">Stellen Sie sicher, dass Sie für die folgenden Zeichen in der Filterzeichenfolge die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) verwenden: Doppelpunkte, Vorwärtsschrägstriche und Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="aa96d-213">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="aa96d-214">**Nachricht** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-214">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="aa96d-215">**Ereignis** -Instanzen abzurufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-215">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="aa96d-216">Gruppe **Ereignis** Instanzen abgerufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="aa96d-216">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="aa96d-217">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="aa96d-217">Path parameters</span></span>
|<span data-ttu-id="aa96d-218">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="aa96d-218">**Parameter**</span></span>|<span data-ttu-id="aa96d-219">**Typ**</span><span class="sxs-lookup"><span data-stu-id="aa96d-219">**Type**</span></span>|<span data-ttu-id="aa96d-220">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="aa96d-220">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="aa96d-221">id_value</span><span class="sxs-lookup"><span data-stu-id="aa96d-221">id_value</span></span>|<span data-ttu-id="aa96d-222">String</span><span class="sxs-lookup"><span data-stu-id="aa96d-222">String</span></span>|<span data-ttu-id="aa96d-p110">Die ID der erweiterten Eigenschaft, nach der gefiltert wird. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa96d-p110">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="aa96d-227">property_value</span><span class="sxs-lookup"><span data-stu-id="aa96d-227">property_value</span></span> |<span data-ttu-id="aa96d-228">String</span><span class="sxs-lookup"><span data-stu-id="aa96d-228">String</span></span>|<span data-ttu-id="aa96d-229">Der Wert der erweiterten Eigenschaft, nach der gefiltert wird.</span><span class="sxs-lookup"><span data-stu-id="aa96d-229">The value of the extended property to match.</span></span> <span data-ttu-id="aa96d-230">Erforderlich, wo im Abschnitt **HTTP-Anforderung** oben aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="aa96d-230">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="aa96d-231">Wenn {property_value} keine Zeichenfolge ist, müssen Sie sicherstellen, dass `ep/value` explizit in den entsprechenden Edm-Datentyp beim Vergleich mit {property_value} umgewandelt wird.</span><span class="sxs-lookup"><span data-stu-id="aa96d-231">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="aa96d-232">Beispiele finden Sie unter [Anforderung 4](#request-4) weiter unter.</span><span class="sxs-lookup"><span data-stu-id="aa96d-232">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="aa96d-233">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa96d-233">Request headers</span></span>
| <span data-ttu-id="aa96d-234">Name</span><span class="sxs-lookup"><span data-stu-id="aa96d-234">Name</span></span>      |<span data-ttu-id="aa96d-235">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa96d-235">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa96d-236">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa96d-236">Authorization</span></span>  | <span data-ttu-id="aa96d-p112">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa96d-p112">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa96d-239">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa96d-239">Request body</span></span>
<span data-ttu-id="aa96d-240">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aa96d-240">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa96d-241">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa96d-241">Response</span></span>

<span data-ttu-id="aa96d-242">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa96d-242">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="aa96d-243">Abrufen von Ressourceninstanzen mithilfe von `$expand`</span><span class="sxs-lookup"><span data-stu-id="aa96d-243">GET resource instance using `$expand`</span></span>
<span data-ttu-id="aa96d-244">Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, erweitert um das dem Filter entsprechende [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="aa96d-244">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="aa96d-245">Abrufen von Ressourceninstanzen mit einer erweiterten Eigenschaft, die einem Filter entspricht</span><span class="sxs-lookup"><span data-stu-id="aa96d-245">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="aa96d-246">Der Antworttext enthält ein oder mehrere Objekte, die Ressourceninstanzen darstellen, die einem dem Filter entsprechende erweiterte Eigenschaft enthalten.</span><span class="sxs-lookup"><span data-stu-id="aa96d-246">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="aa96d-247">Der Antworttext enthält nicht die erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="aa96d-247">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="aa96d-248">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa96d-248">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="aa96d-249">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="aa96d-249">Request 1</span></span>

<span data-ttu-id="aa96d-p114">Im ersten Beispiel wird die angegebene Nachricht abgerufen und um eine einwertige erweiterte Eigenschaft erweitert. Der Filter gibt die erweiterte Eigenschaft zurück, deren **id** der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="aa96d-p114">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="aa96d-252">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="aa96d-252">Response 1</span></span>
<span data-ttu-id="aa96d-253">Der Antworttext enthält alle Eigenschaften der angegebenen Nachricht und die vom Filter zurückgegebene erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="aa96d-253">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="aa96d-p115">Hinweis: Das hier gezeigte **message**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa96d-p115">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a><span data-ttu-id="aa96d-256">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="aa96d-256">Request 2</span></span>

<span data-ttu-id="aa96d-257">Das zweite Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft vom Typ Zeichenfolge haben.</span><span class="sxs-lookup"><span data-stu-id="aa96d-257">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="aa96d-258">Der Filter sucht nach der erweiterten Eigenschaft, die folgende Merkmale hat:</span><span class="sxs-lookup"><span data-stu-id="aa96d-258">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="aa96d-259">Die **ID** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="aa96d-259">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="aa96d-260">Der **Wert** ist gleich der Zeichenfolge `Green`.</span><span class="sxs-lookup"><span data-stu-id="aa96d-260">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="aa96d-261">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="aa96d-261">Response 2</span></span>

<span data-ttu-id="aa96d-p117">Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben. Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user-list-messages.md). Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="aa96d-p117">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="aa96d-265">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="aa96d-265">Request 3</span></span>

<span data-ttu-id="aa96d-266">Das dritte Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft vom Typ Zeichenfolge haben.</span><span class="sxs-lookup"><span data-stu-id="aa96d-266">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="aa96d-267">Der Filter sucht nach der erweiterten Eigenschaft, die folgende Merkmale hat:</span><span class="sxs-lookup"><span data-stu-id="aa96d-267">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="aa96d-268">Die **ID** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).</span><span class="sxs-lookup"><span data-stu-id="aa96d-268">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="aa96d-269">Die **Wert**, der die Zeichenfolge `green` enthält.</span><span class="sxs-lookup"><span data-stu-id="aa96d-269">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="aa96d-270">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="aa96d-270">Response 3</span></span>

<span data-ttu-id="aa96d-271">Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben.</span><span class="sxs-lookup"><span data-stu-id="aa96d-271">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="aa96d-272">Wie zum Beispiel eine Nachricht, die eine einwertige erweiterte Eigenschaft mit einer **ID** besitzt, die der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht, und der **Wert** `Light green` stimmt mit dem Filter überein und ist in der Antwort enthalten.</span><span class="sxs-lookup"><span data-stu-id="aa96d-272">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="aa96d-273">Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="aa96d-273">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="aa96d-274">Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="aa96d-274">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="aa96d-275">Anforderung 4</span><span class="sxs-lookup"><span data-stu-id="aa96d-275">Request 4</span></span>

<span data-ttu-id="aa96d-276">Die nächsten 2 Beispiele zeigen, wie Sie Nachrichten abrufen, die erweiterte einwertige Eigenschaften vom Typ Nicht-Zeichenfolge enthalten.</span><span class="sxs-lookup"><span data-stu-id="aa96d-276">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="aa96d-277">Zur besseren Lesbarkeit ist die erforderliche URL-Codierung dort nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="aa96d-277">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="aa96d-278">Das folgende Beispiel zeigt einen Filter, der nach der erweiterte Eigenschaft mit den folgenden Merkmalen sucht:</span><span class="sxs-lookup"><span data-stu-id="aa96d-278">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="aa96d-279">Die **id** entspricht der Zeichenfolge `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="aa96d-279">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="aa96d-280">Der **Wert** ist die GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="aa96d-280">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="aa96d-281">Wenn Sie den Eigenschaftswert mit einer GUID vergleichen möchten, ändern Sie `ep/value` in `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="aa96d-281">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="aa96d-282">Das folgende Beispiel zeigt einen Filter, der nach der erweiterte Eigenschaft mit den folgenden Merkmalen sucht:</span><span class="sxs-lookup"><span data-stu-id="aa96d-282">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="aa96d-283">Die **id** entspricht der Zeichenfolge `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="aa96d-283">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="aa96d-284">Der **Wert** ist gleich der ganzen Zahl 12.</span><span class="sxs-lookup"><span data-stu-id="aa96d-284">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="aa96d-285">Um den Eigenschaftswert mit einer ganzen Zahl zu vergleichen, ändern Sie `ep/value` in `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="aa96d-285">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="aa96d-286">Antwort 4</span><span class="sxs-lookup"><span data-stu-id="aa96d-286">Response 4</span></span>

<span data-ttu-id="aa96d-287">Bei den zwei vorhergehenden Beispielen ist eine erfolgreiche Antwort durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben.</span><span class="sxs-lookup"><span data-stu-id="aa96d-287">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="aa96d-288">Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="aa96d-288">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="aa96d-289">Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="aa96d-289">The response does not include the matching extended property.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->