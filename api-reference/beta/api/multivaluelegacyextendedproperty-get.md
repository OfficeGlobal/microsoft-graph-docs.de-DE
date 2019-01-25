---
title: Get multiValueLegacyExtendedProperty
description: $expand
localization_priority: Normal
ms.openlocfilehash: 7a649020bf326d4ec1ed3a83ae0c759a012378d4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525241"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="98d8a-103">Get multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="98d8a-103">Get multiValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98d8a-104">Dient zum Abrufen einer Ressourceninstanz mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="98d8a-104">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="98d8a-105">Mit dem Abfrageparameter `$expand` können Sie die angegebene Instanz abrufen, erweitert um die angegebene erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="98d8a-105">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="98d8a-106">Dies ist derzeit die einzige Möglichkeit zum Abrufen des [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="98d8a-106">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="98d8a-107">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="98d8a-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="98d8a-108">calendar</span><span class="sxs-lookup"><span data-stu-id="98d8a-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="98d8a-109">contact</span><span class="sxs-lookup"><span data-stu-id="98d8a-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="98d8a-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="98d8a-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="98d8a-111">Ereignis</span><span class="sxs-lookup"><span data-stu-id="98d8a-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="98d8a-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="98d8a-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="98d8a-113">Nachricht</span><span class="sxs-lookup"><span data-stu-id="98d8a-113">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="98d8a-114">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="98d8a-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="98d8a-115">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="98d8a-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="98d8a-116">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="98d8a-116">As well as the following group resources:</span></span>

- <span data-ttu-id="98d8a-117">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="98d8a-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="98d8a-118">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="98d8a-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="98d8a-119">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="98d8a-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="98d8a-120">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="98d8a-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="98d8a-121">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="98d8a-121">Permissions</span></span>
<span data-ttu-id="98d8a-122">Je nach der Ressource kommen die erweiterte Eigenschaft aus und geben Sie die Berechtigung (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="98d8a-122">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="98d8a-123">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98d8a-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98d8a-124">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="98d8a-124">Supported resource</span></span> | <span data-ttu-id="98d8a-125">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="98d8a-125">Delegated (work or school account)</span></span> | <span data-ttu-id="98d8a-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="98d8a-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98d8a-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="98d8a-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="98d8a-128">Kalender</span><span class="sxs-lookup"><span data-stu-id="98d8a-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="98d8a-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-129">Calendars.Read</span></span> | <span data-ttu-id="98d8a-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-130">Calendars.Read</span></span> | <span data-ttu-id="98d8a-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-131">Calendars.Read</span></span> |
| [<span data-ttu-id="98d8a-132">Kontakt</span><span class="sxs-lookup"><span data-stu-id="98d8a-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="98d8a-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-133">Contacts.Read</span></span> | <span data-ttu-id="98d8a-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-134">Contacts.Read</span></span> | <span data-ttu-id="98d8a-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-135">Contacts.Read</span></span> |
| [<span data-ttu-id="98d8a-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="98d8a-136">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="98d8a-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-137">Contacts.Read</span></span> | <span data-ttu-id="98d8a-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-138">Contacts.Read</span></span> | <span data-ttu-id="98d8a-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-139">Contacts.Read</span></span> |
| [<span data-ttu-id="98d8a-140">Ereignis</span><span class="sxs-lookup"><span data-stu-id="98d8a-140">event</span></span>](../resources/event.md) | <span data-ttu-id="98d8a-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-141">Calendars.Read</span></span> | <span data-ttu-id="98d8a-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-142">Calendars.Read</span></span> |  <span data-ttu-id="98d8a-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-143">Calendars.Read</span></span>|
| <span data-ttu-id="98d8a-144">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="98d8a-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="98d8a-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="98d8a-145">Group.Read.All</span></span> | <span data-ttu-id="98d8a-146">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98d8a-146">Not supported</span></span> | <span data-ttu-id="98d8a-147">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98d8a-147">Not supported</span></span> |
| <span data-ttu-id="98d8a-148">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="98d8a-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="98d8a-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="98d8a-149">Group.Read.All</span></span> | <span data-ttu-id="98d8a-150">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98d8a-150">Not supported</span></span> | <span data-ttu-id="98d8a-151">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98d8a-151">Not supported</span></span> |
| <span data-ttu-id="98d8a-152">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="98d8a-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="98d8a-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="98d8a-153">Group.Read.All</span></span> | <span data-ttu-id="98d8a-154">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98d8a-154">Not supported</span></span> | <span data-ttu-id="98d8a-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="98d8a-155">Group.Read.All</span></span> |
| [<span data-ttu-id="98d8a-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="98d8a-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="98d8a-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-157">Mail.Read</span></span> | <span data-ttu-id="98d8a-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-158">Mail.Read</span></span> | <span data-ttu-id="98d8a-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-159">Mail.Read</span></span> |
| [<span data-ttu-id="98d8a-160">Nachricht</span><span class="sxs-lookup"><span data-stu-id="98d8a-160">message</span></span>](../resources/message.md) | <span data-ttu-id="98d8a-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-161">Mail.Read</span></span> | <span data-ttu-id="98d8a-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-162">Mail.Read</span></span> | <span data-ttu-id="98d8a-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-163">Mail.Read</span></span> |
| [<span data-ttu-id="98d8a-164">Outlook-Aufgabe</span><span class="sxs-lookup"><span data-stu-id="98d8a-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="98d8a-165">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-165">Tasks.Read</span></span> | <span data-ttu-id="98d8a-166">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-166">Tasks.Read</span></span> | <span data-ttu-id="98d8a-167">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98d8a-167">Not supported</span></span> |
| [<span data-ttu-id="98d8a-168">Outlook-Ordner "Aufgaben"</span><span class="sxs-lookup"><span data-stu-id="98d8a-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="98d8a-169">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-169">Tasks.Read</span></span> | <span data-ttu-id="98d8a-170">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="98d8a-170">Tasks.Read</span></span> | <span data-ttu-id="98d8a-171">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98d8a-171">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="98d8a-172">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98d8a-172">HTTP request</span></span>

<span data-ttu-id="98d8a-p103">Rufen Sie eine erweiterte Ressourceninstanz mit erweiterter Eigenschaft ab, die einem Filter für die **id**-Eigenschaft entspricht. Stellen Sie sicher, dass Sie die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) auf die Leerzeichen in der Filterzeichenfolge anwenden.</span><span class="sxs-lookup"><span data-stu-id="98d8a-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="98d8a-175">Abrufen einer **message**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="98d8a-175">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="98d8a-176">Abrufen einer **mailFolder**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="98d8a-176">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="98d8a-177">Abrufen einer **event**-Instanz</span><span class="sxs-lookup"><span data-stu-id="98d8a-177">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="98d8a-178">Abrufen einer **calendar**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="98d8a-178">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="98d8a-179">Abrufen einer **contact**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="98d8a-179">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="98d8a-180">Abrufen einer **contactFolder**-Instanz:</span><span class="sxs-lookup"><span data-stu-id="98d8a-180">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="98d8a-181">Erhalten Sie eine Instanz **OutlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="98d8a-181">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="98d8a-182">Erhalten Sie eine Instanz **OutlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="98d8a-182">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="98d8a-183">Abrufen einer **event**-Instanz für eine Gruppe:</span><span class="sxs-lookup"><span data-stu-id="98d8a-183">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="98d8a-184">Abrufen einer **post**-Instanz für eine Gruppe:</span><span class="sxs-lookup"><span data-stu-id="98d8a-184">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="98d8a-185">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="98d8a-185">Path parameters</span></span>
|<span data-ttu-id="98d8a-186">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="98d8a-186">**Parameter**</span></span>|<span data-ttu-id="98d8a-187">**Typ**</span><span class="sxs-lookup"><span data-stu-id="98d8a-187">**Type**</span></span>|<span data-ttu-id="98d8a-188">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="98d8a-188">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="98d8a-189">id_value</span><span class="sxs-lookup"><span data-stu-id="98d8a-189">id_value</span></span>|<span data-ttu-id="98d8a-190">String</span><span class="sxs-lookup"><span data-stu-id="98d8a-190">String</span></span>|<span data-ttu-id="98d8a-p104">Die ID der erweiterten übereinstimmenden Eigenschaft. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="98d8a-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="98d8a-195">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="98d8a-195">Request headers</span></span>
| <span data-ttu-id="98d8a-196">Name</span><span class="sxs-lookup"><span data-stu-id="98d8a-196">Name</span></span>      |<span data-ttu-id="98d8a-197">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98d8a-197">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98d8a-198">Authorization</span><span class="sxs-lookup"><span data-stu-id="98d8a-198">Authorization</span></span>  | <span data-ttu-id="98d8a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="98d8a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98d8a-201">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="98d8a-201">Request body</span></span>
<span data-ttu-id="98d8a-202">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="98d8a-202">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98d8a-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="98d8a-203">Response</span></span>

<span data-ttu-id="98d8a-204">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98d8a-204">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="98d8a-205">Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, und das übereinstimmende [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="98d8a-205">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="98d8a-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98d8a-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98d8a-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="98d8a-207">Request</span></span>
<span data-ttu-id="98d8a-p106">In diesem Beispiel wird das angegebene Ereignis abgerufen und um eine erweiterte mehrwertige Eigenschaften erwetiert. Der Filter gibt die erweiterte Eigenschaft mit der **ID** an, die mit der Zeichenfolge `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` übereinstimmt (URL-Codierung wurde zur besseren Lesbarkeit in diesem Beispiel entfernt).</span><span class="sxs-lookup"><span data-stu-id="98d8a-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="98d8a-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="98d8a-210">Response</span></span>

<span data-ttu-id="98d8a-211">Der Antworttext enthält alle Eigenschaften des angegebenen Ereignisses und erweiterte Eigenschaften, die von dem Filter zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="98d8a-211">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="98d8a-p107">Hinweis: Das hier gezeigte **event**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98d8a-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/multivaluelegacyextendedproperty-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
