---
title: e-Mail-Infos Ressourcentyp
description: 'Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden. Beispielsweise eine Out-of-Office-Nachricht '
localization_priority: Normal
ms.openlocfilehash: 0506d10ad4b1c5eb473b04a30eb8d48334685574
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891693"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="898ff-104">e-Mail-Infos Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="898ff-104">mailTips resource type</span></span>

<span data-ttu-id="898ff-105">Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="898ff-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="898ff-106">Beispielsweise eine Abwesenheits Nachricht als automatische Antwort für einen Nachrichtenempfänger.</span><span class="sxs-lookup"><span data-stu-id="898ff-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="898ff-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="898ff-107">Properties</span></span>
| <span data-ttu-id="898ff-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="898ff-108">Property</span></span>     | <span data-ttu-id="898ff-109">Typ</span><span class="sxs-lookup"><span data-stu-id="898ff-109">Type</span></span>   |<span data-ttu-id="898ff-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="898ff-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="898ff-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="898ff-111">automaticReplies</span></span> | [<span data-ttu-id="898ff-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="898ff-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="898ff-113">Mail-Tipps für die automatische Antwort, wenn es vom Empfänger eingerichtet wurde.</span><span class="sxs-lookup"><span data-stu-id="898ff-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="898ff-114">customMailTip</span><span class="sxs-lookup"><span data-stu-id="898ff-114">customMailTip</span></span> | <span data-ttu-id="898ff-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="898ff-115">String</span></span> | <span data-ttu-id="898ff-116">Eine benutzerdefinierte e-Mail-Info, die für das Postfach des Empfängers festgelegt werden kann.</span><span class="sxs-lookup"><span data-stu-id="898ff-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="898ff-117">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="898ff-117">deliveryRestricted</span></span>| <span data-ttu-id="898ff-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="898ff-118">Boolean</span></span> | <span data-ttu-id="898ff-119">Gibt an, ob das Postfach des Empfängers beschränkt, beispielsweise ist akzeptieren von Nachrichten aus einer vordefinierten Liste Absender, ablehnen von Nachrichten aus einer vordefinierten Liste der Absender oder Nachrichten von nur von authentifizierten Absendern akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="898ff-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="898ff-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="898ff-120">emailAddress</span></span> | [<span data-ttu-id="898ff-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="898ff-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="898ff-122">Die e-Mail-Adresse des Empfängers zum Abrufen von e-Mail-Infos für.</span><span class="sxs-lookup"><span data-stu-id="898ff-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="898ff-123">error</span><span class="sxs-lookup"><span data-stu-id="898ff-123">error</span></span> | [<span data-ttu-id="898ff-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="898ff-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="898ff-125">Fehler, die während der Aktion [GetMailTips](../api/user-getmailtips.md) auftreten.</span><span class="sxs-lookup"><span data-stu-id="898ff-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="898ff-126">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="898ff-126">externalMemberCount</span></span> | <span data-ttu-id="898ff-127">Int32</span><span class="sxs-lookup"><span data-stu-id="898ff-127">Int32</span></span> | <span data-ttu-id="898ff-128">Die Anzahl der externen Elemente, wenn beim Empfänger um eine Verteilerliste handelt.</span><span class="sxs-lookup"><span data-stu-id="898ff-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="898ff-129">isModerated</span><span class="sxs-lookup"><span data-stu-id="898ff-129">isModerated</span></span> |<span data-ttu-id="898ff-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="898ff-130">Boolean</span></span>  | <span data-ttu-id="898ff-131">Gibt an, ob das Senden von Nachrichten an den Empfänger genehmigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="898ff-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="898ff-132">Angenommen, wurde Wenn der Empfänger eine große Verteilerliste ist und eine Moderator festgelegt bis zu an diese Verteilerliste gesendete Nachrichten genehmigen oder wenn Senden von Nachrichten an ein Empfänger Genehmigung des Managers des Empfängers erforderlich.</span><span class="sxs-lookup"><span data-stu-id="898ff-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="898ff-133">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="898ff-133">mailboxFull</span></span> | <span data-ttu-id="898ff-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="898ff-134">Boolean</span></span> | <span data-ttu-id="898ff-135">Der vollständige Postfachstatus des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="898ff-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="898ff-136">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="898ff-136">maxMessageSize</span></span> | <span data-ttu-id="898ff-137">Int32</span><span class="sxs-lookup"><span data-stu-id="898ff-137">Int32</span></span> | <span data-ttu-id="898ff-138">Die maximale Nachrichtengröße für die Organisation oder das Postfach des Empfängers konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="898ff-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="898ff-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="898ff-139">recipientScope</span></span> | <span data-ttu-id="898ff-140">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="898ff-140">recipientScopeType</span></span> | <span data-ttu-id="898ff-141">Der Bereich des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="898ff-141">The scope of the recipient.</span></span> <span data-ttu-id="898ff-142">Mögliche Werte sind: `none`, `internal`, `external`, `externalPartner` und `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="898ff-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="898ff-143">Beispielsweise kann ein Administrator einer anderen Organisation zu seinem "Partner" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="898ff-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="898ff-144">Der Bereich ist nützlich, wenn ein Administrator möchte, dass bestimmte e-Mail-Infos für bestimmte Bereiche zugänglich sein.</span><span class="sxs-lookup"><span data-stu-id="898ff-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="898ff-145">Es ist außerdem hilfreich, Absender zu informieren, dass ihre Nachricht die Organisation, deren Unterstützung bei der richtigen Entscheidungen zu Wortlaut, Ton und Inhalte lassen kann.</span><span class="sxs-lookup"><span data-stu-id="898ff-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="898ff-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="898ff-146">recipientSuggestions</span></span> | <span data-ttu-id="898ff-147">[recipient](../resources/recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="898ff-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="898ff-148">Empfänger vorgeschlagene basierend auf vorherigen Kontext, in dem sie in der gleichen Nachricht angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="898ff-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="898ff-149">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="898ff-149">totalMemberCount</span></span> | <span data-ttu-id="898ff-150">Int32</span><span class="sxs-lookup"><span data-stu-id="898ff-150">Int32</span></span> | <span data-ttu-id="898ff-151">Die Anzahl der Elemente, wenn der Empfänger eine Verteilerliste handelt.</span><span class="sxs-lookup"><span data-stu-id="898ff-151">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="898ff-152">RecipientScopeType Werte</span><span class="sxs-lookup"><span data-stu-id="898ff-152">recipientScopeType values</span></span>

| <span data-ttu-id="898ff-153">Wert</span><span class="sxs-lookup"><span data-stu-id="898ff-153">Value</span></span>
|:-------------------------
| <span data-ttu-id="898ff-154">n/v</span><span class="sxs-lookup"><span data-stu-id="898ff-154">none</span></span>
| <span data-ttu-id="898ff-155">interne</span><span class="sxs-lookup"><span data-stu-id="898ff-155">internal</span></span>
| <span data-ttu-id="898ff-156">externe</span><span class="sxs-lookup"><span data-stu-id="898ff-156">external</span></span>
| <span data-ttu-id="898ff-157">externalPartner</span><span class="sxs-lookup"><span data-stu-id="898ff-157">externalPartner</span></span>
| <span data-ttu-id="898ff-158">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="898ff-158">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="898ff-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="898ff-159">JSON representation</span></span>

<span data-ttu-id="898ff-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="898ff-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
