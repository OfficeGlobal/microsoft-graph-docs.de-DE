---
title: Get multiValueLegacyExtendedProperty
description: Erweitern Sie ".
localization_priority: Normal
ms.openlocfilehash: c1d95e319637df17f04e706055245d5e19762a87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866325"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="6cb82-103">Get multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6cb82-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="6cb82-104">Dient zum Abrufen einer Ressourceninstanz mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="6cb82-104">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="6cb82-105">Mit dem Abfrageparameter `$expand` können Sie die angegebene Instanz abrufen, erweitert um die angegebene erweiterte Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="6cb82-105">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="6cb82-106">Dies ist derzeit die einzige Möglichkeit zum Abrufen des [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="6cb82-106">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="6cb82-107">Die folgenden Benutzerressourcen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="6cb82-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="6cb82-108">calendar</span><span class="sxs-lookup"><span data-stu-id="6cb82-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="6cb82-109">contact</span><span class="sxs-lookup"><span data-stu-id="6cb82-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="6cb82-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6cb82-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="6cb82-111">Ereignis</span><span class="sxs-lookup"><span data-stu-id="6cb82-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="6cb82-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6cb82-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="6cb82-113">message</span><span class="sxs-lookup"><span data-stu-id="6cb82-113">message</span></span>](../resources/message.md) 

<span data-ttu-id="6cb82-114">Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="6cb82-114">As well as the following group resources:</span></span>

- <span data-ttu-id="6cb82-115">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6cb82-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="6cb82-116">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6cb82-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="6cb82-117">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6cb82-117">group [post](../resources/post.md)</span></span>

<span data-ttu-id="6cb82-118">Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="6cb82-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cb82-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6cb82-119">Permissions</span></span>
<span data-ttu-id="6cb82-120">Je nach der Ressource kommen die erweiterte Eigenschaft aus und geben Sie die Berechtigung (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="6cb82-120">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="6cb82-121">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb82-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cb82-122">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="6cb82-122">Supported resource</span></span> | <span data-ttu-id="6cb82-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6cb82-123">Delegated (work or school account)</span></span> | <span data-ttu-id="6cb82-124">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6cb82-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cb82-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6cb82-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="6cb82-126">Kalender</span><span class="sxs-lookup"><span data-stu-id="6cb82-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="6cb82-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-127">Calendars.Read</span></span> | <span data-ttu-id="6cb82-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-128">Calendars.Read</span></span> | <span data-ttu-id="6cb82-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-129">Calendars.Read</span></span> |
| [<span data-ttu-id="6cb82-130">Kontakt</span><span class="sxs-lookup"><span data-stu-id="6cb82-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6cb82-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-131">Contacts.Read</span></span> | <span data-ttu-id="6cb82-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-132">Contacts.Read</span></span> | <span data-ttu-id="6cb82-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-133">Contacts.Read</span></span> |
| [<span data-ttu-id="6cb82-134">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6cb82-134">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="6cb82-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-135">Contacts.Read</span></span> | <span data-ttu-id="6cb82-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-136">Contacts.Read</span></span> | <span data-ttu-id="6cb82-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-137">Contacts.Read</span></span> |
| [<span data-ttu-id="6cb82-138">Ereignis</span><span class="sxs-lookup"><span data-stu-id="6cb82-138">event</span></span>](../resources/event.md) | <span data-ttu-id="6cb82-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-139">Calendars.Read</span></span> | <span data-ttu-id="6cb82-140">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-140">Calendars.Read</span></span> |  <span data-ttu-id="6cb82-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-141">Calendars.Read</span></span>|
| <span data-ttu-id="6cb82-142">[calendar](../resources/calendar.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6cb82-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="6cb82-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cb82-143">Group.Read.All</span></span> | <span data-ttu-id="6cb82-144">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cb82-144">Not supported</span></span> | <span data-ttu-id="6cb82-145">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cb82-145">Not supported</span></span> |
| <span data-ttu-id="6cb82-146">[event](../resources/event.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6cb82-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="6cb82-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cb82-147">Group.Read.All</span></span> | <span data-ttu-id="6cb82-148">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cb82-148">Not supported</span></span> | <span data-ttu-id="6cb82-149">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cb82-149">Not supported</span></span> |
| <span data-ttu-id="6cb82-150">[post](../resources/post.md)-Ressourcen für Gruppen</span><span class="sxs-lookup"><span data-stu-id="6cb82-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="6cb82-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cb82-151">Group.Read.All</span></span> | <span data-ttu-id="6cb82-152">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cb82-152">Not supported</span></span> | <span data-ttu-id="6cb82-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cb82-153">Group.Read.All</span></span> |
| [<span data-ttu-id="6cb82-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6cb82-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="6cb82-155">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-155">Mail.Read</span></span> | <span data-ttu-id="6cb82-156">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-156">Mail.Read</span></span> | <span data-ttu-id="6cb82-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-157">Mail.Read</span></span> |
| [<span data-ttu-id="6cb82-158">message</span><span class="sxs-lookup"><span data-stu-id="6cb82-158">message</span></span>](../resources/message.md) | <span data-ttu-id="6cb82-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-159">Mail.Read</span></span> | <span data-ttu-id="6cb82-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-160">Mail.Read</span></span> | <span data-ttu-id="6cb82-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6cb82-161">Mail.Read</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="6cb82-162">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cb82-162">HTTP request</span></span>

<span data-ttu-id="6cb82-p103">Rufen Sie eine erweiterte Ressourceninstanz mit erweiterter Eigenschaft ab, die einem Filter für die **id**-Eigenschaft entspricht. Stellen Sie sicher, dass Sie die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) auf die Leerzeichen in der Filterzeichenfolge anwenden.</span><span class="sxs-lookup"><span data-stu-id="6cb82-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="6cb82-165">Erhalten Sie eine Instanz der **Nachricht** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6cb82-165">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6cb82-166">Eine **MailFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6cb82-166">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="6cb82-167">Rufen Sie eine Instanz **Ereignis** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6cb82-167">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6cb82-168">Eine **Kalender** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6cb82-168">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6cb82-169">Abrufen einer Instanz **wenden Sie sich an** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6cb82-169">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6cb82-170">Eine **ContactFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6cb82-170">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="6cb82-171">Eine Gruppe **Ereignis** Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6cb82-171">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="6cb82-172">Eine Gruppe **Buchen** -Instanz abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6cb82-172">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="6cb82-173">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="6cb82-173">Path parameters</span></span>
|<span data-ttu-id="6cb82-174">Parameter</span><span class="sxs-lookup"><span data-stu-id="6cb82-174">Parameter</span></span>|<span data-ttu-id="6cb82-175">Typ</span><span class="sxs-lookup"><span data-stu-id="6cb82-175">Type</span></span>|<span data-ttu-id="6cb82-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6cb82-176">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6cb82-177">id_value</span><span class="sxs-lookup"><span data-stu-id="6cb82-177">id_value</span></span>|<span data-ttu-id="6cb82-178">String</span><span class="sxs-lookup"><span data-stu-id="6cb82-178">String</span></span>|<span data-ttu-id="6cb82-p104">Die ID der erweiterten übereinstimmenden Eigenschaft. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6cb82-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6cb82-183">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6cb82-183">Request headers</span></span>
| <span data-ttu-id="6cb82-184">Name</span><span class="sxs-lookup"><span data-stu-id="6cb82-184">Name</span></span>      |<span data-ttu-id="6cb82-185">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6cb82-185">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6cb82-186">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cb82-186">Authorization</span></span>  | <span data-ttu-id="6cb82-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6cb82-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cb82-189">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6cb82-189">Request body</span></span>
<span data-ttu-id="6cb82-190">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6cb82-190">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cb82-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cb82-191">Response</span></span>

<span data-ttu-id="6cb82-192">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6cb82-192">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="6cb82-193">Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, und das übereinstimmende [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="6cb82-193">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="6cb82-194">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6cb82-194">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6cb82-195">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cb82-195">Request</span></span>
<span data-ttu-id="6cb82-p106">In diesem Beispiel wird das angegebene Ereignis abgerufen und um eine erweiterte mehrwertige Eigenschaften erwetiert. Der Filter gibt die erweiterte Eigenschaft mit der **ID** an, die mit der Zeichenfolge `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` übereinstimmt (URL-Codierung wurde zur besseren Lesbarkeit in diesem Beispiel entfernt).</span><span class="sxs-lookup"><span data-stu-id="6cb82-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="6cb82-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cb82-198">Response</span></span>

<span data-ttu-id="6cb82-199">Der Antworttext enthält alle Eigenschaften des angegebenen Ereignisses und erweiterte Eigenschaften, die von dem Filter zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="6cb82-199">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="6cb82-p107">Hinweis: Das hier gezeigte **event**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6cb82-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
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
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
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
