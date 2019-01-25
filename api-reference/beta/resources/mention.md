---
title: Erwähnen Ressourcentyp
description: Stellt eine Benachrichtigung an eine Person basierend auf e-Mail-Adresse der Person.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8e04722edf878b4f3851de837908dc5c0a02de7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523197"
---
# <a name="mention-resource-type"></a><span data-ttu-id="9dc75-103">Erwähnen Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9dc75-103">mention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dc75-104">Stellt eine Benachrichtigung an eine Person basierend auf e-Mail-Adresse der Person.</span><span class="sxs-lookup"><span data-stu-id="9dc75-104">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="9dc75-105">Die Benachrichtigung wird auch als @ erwähnungen.</span><span class="sxs-lookup"><span data-stu-id="9dc75-105">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="9dc75-106">Die [Nachricht](../resources/message.md) Ressource unterstützt **erwähnen**.</span><span class="sxs-lookup"><span data-stu-id="9dc75-106">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="9dc75-107">Sie umfasst eine **MentionsPreview** -Eigenschaft, die angibt, ob der angemeldeten Benutzer in dieser Nachrichteninstanz genannt wird.</span><span class="sxs-lookup"><span data-stu-id="9dc75-107">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="9dc75-108">Darüber hinaus Navigationseigenschaft **erwähnt** , das die erste Details der Vermerk oder Löschen der Vermerk in dieser Instanz unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9dc75-108">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="9dc75-109">Beim Erstellen einer Nachricht kann eine app in der gleichen Vermerk erstellen `POST` Anforderung durch, einschließlich der Angabe in der **erwähnungen** -Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="9dc75-109">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="9dc75-110">Verwenden einer `GET` fordern Sie mit der `$filter` Abfragezeichenfolgen-Parameter eine app kann Zurückgeben aller Nachrichten im Postfach des angemeldeten Benutzers, in denen den Benutzer erwähnt.</span><span class="sxs-lookup"><span data-stu-id="9dc75-110">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="9dc75-111">Eine `GET` fordern Sie mit der `$expand` Abfrage Parameter können die app alle Vorkommnisse in eine bestimmte Nachricht zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="9dc75-111">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="9dc75-112">Dieser Mechanismus, lassen eine app festlegen und Abrufen erwähnungen in Nachrichten ermöglicht lightweight-Benachrichtigungen, in dem der Benutzer die Erwähnung, in dem vorhandenen Kontext (beispielsweise Verfassen eines Nachrichtentexts) verbleiben kann während der app wird die zugrunde liegende **erwähnt** -Eigenschaft .</span><span class="sxs-lookup"><span data-stu-id="9dc75-112">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="9dc75-113">Erwähnten Personen können auf einfache Weise ermitteln, ob die und, in denen sie über erwähnt sind `GET` fordert mit der `$filter` oder `$expand` Parameter Abfragen.</span><span class="sxs-lookup"><span data-stu-id="9dc75-113">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="9dc75-114">In der Outlook-Mailclient, wenn ein Benutzer beispielsweise `@` beim Verfassen einer Nachricht, lässt Outlook den Benutzer aktivieren, oder geben Sie einen Namen für die Durchführung der @ Erwähnung.</span><span class="sxs-lookup"><span data-stu-id="9dc75-114">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="9dc75-115">Outlook wird die Eigenschaft **erwähnt** , bevor er erstellt und die Nachricht oder Ereignis sendet.</span><span class="sxs-lookup"><span data-stu-id="9dc75-115">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="9dc75-116">Outlook verwendet auch `GET` Vorgänge mit `$filter` und `$expand` warnen der Benutzer zum Aufgaben oder Diskussionen, wodurch eine schnellere Antwort ermöglicht, um die angemeldeten Benutzer nach Nachrichten suchen, in denen den Benutzer erwähnt,.</span><span class="sxs-lookup"><span data-stu-id="9dc75-116">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9dc75-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9dc75-117">JSON representation</span></span>

<span data-ttu-id="9dc75-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9dc75-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mention"
}-->

```json
{
  "application": "string",
  "clientReference": "string",
  "createdBy": {"@odata.type": "microsoft.graph.emailAddress"},
  "createdDateTime": "DateTimeOffset",
  "deepLink": "string",
  "id": "string (identifier)",
  "mentioned": {"@odata.type": "microsoft.graph.emailAddress"},
  "mentionText": "string",
  "serverCreatedDateTime": "DateTimeOffset"
}

```
## <a name="properties"></a><span data-ttu-id="9dc75-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9dc75-119">Properties</span></span>
| <span data-ttu-id="9dc75-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9dc75-120">Property</span></span>     | <span data-ttu-id="9dc75-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9dc75-121">Type</span></span>   |<span data-ttu-id="9dc75-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dc75-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dc75-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9dc75-123">application</span></span> | <span data-ttu-id="9dc75-124">String</span><span class="sxs-lookup"><span data-stu-id="9dc75-124">String</span></span> | <span data-ttu-id="9dc75-125">Der Name der Anwendung, in dem die Erwähnung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="9dc75-125">The name of the application where the mention is created.</span></span> <span data-ttu-id="9dc75-126">Optional.</span><span class="sxs-lookup"><span data-stu-id="9dc75-126">Optional.</span></span> <span data-ttu-id="9dc75-127">Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen.</span><span class="sxs-lookup"><span data-stu-id="9dc75-127">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="9dc75-128">clientReference</span><span class="sxs-lookup"><span data-stu-id="9dc75-128">clientReference</span></span> | <span data-ttu-id="9dc75-129">String</span><span class="sxs-lookup"><span data-stu-id="9dc75-129">String</span></span> | <span data-ttu-id="9dc75-130">Ein eindeutiger Bezeichner, der ein übergeordnetes Element der Ressourceninstanz darstellt.</span><span class="sxs-lookup"><span data-stu-id="9dc75-130">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="9dc75-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="9dc75-131">Optional.</span></span> <span data-ttu-id="9dc75-132">Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen.</span><span class="sxs-lookup"><span data-stu-id="9dc75-132">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="9dc75-133">createdBy</span><span class="sxs-lookup"><span data-stu-id="9dc75-133">createdBy</span></span>  | [<span data-ttu-id="9dc75-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9dc75-134">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="9dc75-135">Die e-Mail-Informationen des Benutzers, der die Erwähnung vorgenommen.</span><span class="sxs-lookup"><span data-stu-id="9dc75-135">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="9dc75-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc75-136">createdDateTime</span></span>  |<span data-ttu-id="9dc75-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc75-137">DateTimeOffset</span></span> |<span data-ttu-id="9dc75-138">Das Datum und die Uhrzeit, die auf dem Client die Erwähnung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="9dc75-138">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="9dc75-139">deepLink</span><span class="sxs-lookup"><span data-stu-id="9dc75-139">deepLink</span></span> | <span data-ttu-id="9dc75-140">String</span><span class="sxs-lookup"><span data-stu-id="9dc75-140">String</span></span> | <span data-ttu-id="9dc75-141">Tiefe Weblink zu den Kontext des Hinweises auf die Instanz der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9dc75-141">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="9dc75-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="9dc75-142">Optional.</span></span> <span data-ttu-id="9dc75-143">Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen.</span><span class="sxs-lookup"><span data-stu-id="9dc75-143">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="9dc75-144">id</span><span class="sxs-lookup"><span data-stu-id="9dc75-144">id</span></span> | <span data-ttu-id="9dc75-145">String</span><span class="sxs-lookup"><span data-stu-id="9dc75-145">String</span></span>| <span data-ttu-id="9dc75-146">Der eindeutige Bezeichner des Vermerk in einer Ressourceninstanz einer.</span><span class="sxs-lookup"><span data-stu-id="9dc75-146">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="9dc75-147">erwähnten</span><span class="sxs-lookup"><span data-stu-id="9dc75-147">mentioned</span></span> | [<span data-ttu-id="9dc75-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9dc75-148">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="9dc75-149">Die e-Mail-Informationen der weiter oben erwähnt Person.</span><span class="sxs-lookup"><span data-stu-id="9dc75-149">The email information of the mentioned person.</span></span> <span data-ttu-id="9dc75-150">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9dc75-150">Required.</span></span> |
|<span data-ttu-id="9dc75-151">mentionText</span><span class="sxs-lookup"><span data-stu-id="9dc75-151">mentionText</span></span> | <span data-ttu-id="9dc75-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9dc75-152">String</span></span> | <span data-ttu-id="9dc75-153">Optional.</span><span class="sxs-lookup"><span data-stu-id="9dc75-153">Optional.</span></span> <span data-ttu-id="9dc75-154">Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen.</span><span class="sxs-lookup"><span data-stu-id="9dc75-154">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="9dc75-155">Wenn die erwähnungen in einer Nachricht erhalten möchten, finden Sie stattdessen die **BodyPreview** -Eigenschaft der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="9dc75-155">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="9dc75-156">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc75-156">serverCreatedDateTime</span></span> | <span data-ttu-id="9dc75-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc75-157">DateTimeOffset</span></span> | <span data-ttu-id="9dc75-158">Das Datum und die Uhrzeit, die die Erwähnung auf dem Server erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="9dc75-158">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="9dc75-159">Optional.</span><span class="sxs-lookup"><span data-stu-id="9dc75-159">Optional.</span></span> <span data-ttu-id="9dc75-160">Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen.</span><span class="sxs-lookup"><span data-stu-id="9dc75-160">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9dc75-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9dc75-161">Relationships</span></span>
<span data-ttu-id="9dc75-162">Keine</span><span class="sxs-lookup"><span data-stu-id="9dc75-162">None</span></span>


## <a name="methods"></a><span data-ttu-id="9dc75-163">Methoden</span><span class="sxs-lookup"><span data-stu-id="9dc75-163">Methods</span></span>

| <span data-ttu-id="9dc75-164">Methode</span><span class="sxs-lookup"><span data-stu-id="9dc75-164">Method</span></span>           | <span data-ttu-id="9dc75-165">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9dc75-165">Return Type</span></span>    |<span data-ttu-id="9dc75-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dc75-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dc75-167">[POST-Anforderung](../api/user-sendmail.md#request-2) und senden</span><span class="sxs-lookup"><span data-stu-id="9dc75-167">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="9dc75-168">Keine</span><span class="sxs-lookup"><span data-stu-id="9dc75-168">None</span></span> | <span data-ttu-id="9dc75-169">Erstellen und Senden von erwähnungen im Rahmen einer neuen Nachricht.</span><span class="sxs-lookup"><span data-stu-id="9dc75-169">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="9dc75-170">[POST-Anforderung](../api/user-post-messages.md#request-2) an einen neuen Entwurf</span><span class="sxs-lookup"><span data-stu-id="9dc75-170">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="9dc75-171">[Nachricht](../resources/message.md) , die ein oder mehrere **erwähnen** Objekte enthält.</span><span class="sxs-lookup"><span data-stu-id="9dc75-171">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="9dc75-172">Erstellen ein Entwurfs oder eine neue Nachricht und fügen Sie ein oder mehrere **erwähnen** Objekte.</span><span class="sxs-lookup"><span data-stu-id="9dc75-172">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="9dc75-173">[Abrufen](../api/user-list-messages.md#request-2) von Nachrichten Erwähnung me</span><span class="sxs-lookup"><span data-stu-id="9dc75-173">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="9dc75-174">[message](../resources/message.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9dc75-174">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="9dc75-175">Rufen Sie alle Nachrichten im Postfach des angemeldeten Benutzers, die ein **erwähnen** dieses Benutzers enthalten.</span><span class="sxs-lookup"><span data-stu-id="9dc75-175">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="9dc75-176">Eine Meldung [erhalten](../api/message-get.md#request-2) und seine erwähnungen</span><span class="sxs-lookup"><span data-stu-id="9dc75-176">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="9dc75-177">[message](../resources/message.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9dc75-177">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="9dc75-178">Möchten Sie eine Meldung erhalten, und erweitern Sie die Details der einzelnen **erwähnen** in der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="9dc75-178">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="9dc75-179">[Löschen](../api/message-delete.md#request-2) der Vermerk</span><span class="sxs-lookup"><span data-stu-id="9dc75-179">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="9dc75-180">Keine</span><span class="sxs-lookup"><span data-stu-id="9dc75-180">None</span></span> |<span data-ttu-id="9dc75-181">Löscht die angegebene Erwähnung in der angegebenen Nachricht im Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9dc75-181">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
