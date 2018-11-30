---
title: e-Mail-Infos Ressourcentyp
description: 'Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden. Beispielsweise eine Out-of-Office-Nachricht '
ms.openlocfilehash: a8686f256301317af5b02388052c6ccb02e81f69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064696"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="c7a68-104">e-Mail-Infos Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c7a68-104">mailTips resource type</span></span>

> <span data-ttu-id="c7a68-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7a68-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7a68-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7a68-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7a68-107">Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c7a68-107">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="c7a68-108">Beispielsweise eine Abwesenheits Nachricht als automatische Antwort für einen Nachrichtenempfänger.</span><span class="sxs-lookup"><span data-stu-id="c7a68-108">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="c7a68-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7a68-109">Properties</span></span>
| <span data-ttu-id="c7a68-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7a68-110">Property</span></span>     | <span data-ttu-id="c7a68-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c7a68-111">Type</span></span>   |<span data-ttu-id="c7a68-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7a68-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c7a68-113">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="c7a68-113">automaticReplies</span></span> | [<span data-ttu-id="c7a68-114">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="c7a68-114">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="c7a68-115">Mail-Tipps für die automatische Antwort, wenn es vom Empfänger eingerichtet wurde.</span><span class="sxs-lookup"><span data-stu-id="c7a68-115">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="c7a68-116">customMailTip</span><span class="sxs-lookup"><span data-stu-id="c7a68-116">customMailTip</span></span> | <span data-ttu-id="c7a68-117">String</span><span class="sxs-lookup"><span data-stu-id="c7a68-117">String</span></span> | <span data-ttu-id="c7a68-118">Eine benutzerdefinierte e-Mail-Info, die für das Postfach des Empfängers festgelegt werden kann.</span><span class="sxs-lookup"><span data-stu-id="c7a68-118">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="c7a68-119">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="c7a68-119">deliveryRestricted</span></span>| <span data-ttu-id="c7a68-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c7a68-120">Boolean</span></span> | <span data-ttu-id="c7a68-121">Gibt an, ob das Postfach des Empfängers beschränkt, beispielsweise ist akzeptieren von Nachrichten aus einer vordefinierten Liste Absender, ablehnen von Nachrichten aus einer vordefinierten Liste der Absender oder Nachrichten von nur von authentifizierten Absendern akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="c7a68-121">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="c7a68-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c7a68-122">emailAddress</span></span> | [<span data-ttu-id="c7a68-123">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c7a68-123">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="c7a68-124">Die e-Mail-Adresse des Empfängers zum Abrufen von e-Mail-Infos für.</span><span class="sxs-lookup"><span data-stu-id="c7a68-124">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="c7a68-125">error</span><span class="sxs-lookup"><span data-stu-id="c7a68-125">error</span></span> | [<span data-ttu-id="c7a68-126">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="c7a68-126">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="c7a68-127">Fehler, die während der Aktion [GetMailTips](../api/user-getmailtips.md) auftreten.</span><span class="sxs-lookup"><span data-stu-id="c7a68-127">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="c7a68-128">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="c7a68-128">externalMemberCount</span></span> | <span data-ttu-id="c7a68-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c7a68-129">Int32</span></span> | <span data-ttu-id="c7a68-130">Die Anzahl der externen Elemente, wenn beim Empfänger um eine Verteilerliste handelt.</span><span class="sxs-lookup"><span data-stu-id="c7a68-130">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="c7a68-131">isModerated</span><span class="sxs-lookup"><span data-stu-id="c7a68-131">isModerated</span></span> |<span data-ttu-id="c7a68-132">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c7a68-132">Boolean</span></span>  | <span data-ttu-id="c7a68-133">Gibt an, ob das Senden von Nachrichten an den Empfänger genehmigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="c7a68-133">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="c7a68-134">Angenommen, wurde Wenn der Empfänger eine große Verteilerliste ist und eine Moderator festgelegt bis zu an diese Verteilerliste gesendete Nachrichten genehmigen oder wenn Senden von Nachrichten an ein Empfänger Genehmigung des Managers des Empfängers erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c7a68-134">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="c7a68-135">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="c7a68-135">mailboxFull</span></span> | <span data-ttu-id="c7a68-136">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c7a68-136">Boolean</span></span> | <span data-ttu-id="c7a68-137">Der vollständige Postfachstatus des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="c7a68-137">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="c7a68-138">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="c7a68-138">maxMessageSize</span></span> | <span data-ttu-id="c7a68-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c7a68-139">Int32</span></span> | <span data-ttu-id="c7a68-140">Die maximale Nachrichtengröße für die Organisation oder das Postfach des Empfängers konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="c7a68-140">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="c7a68-141">recipientScope</span><span class="sxs-lookup"><span data-stu-id="c7a68-141">recipientScope</span></span> | <span data-ttu-id="c7a68-142">String</span><span class="sxs-lookup"><span data-stu-id="c7a68-142">String</span></span> | <span data-ttu-id="c7a68-143">Der Bereich des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="c7a68-143">The scope of the recipient.</span></span> <span data-ttu-id="c7a68-144">Mögliche Werte sind: `none`, `internal`, `external`, `externalPartner` und `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="c7a68-144">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="c7a68-145">Beispielsweise kann ein Administrator einer anderen Organisation zu seinem "Partner" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c7a68-145">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="c7a68-146">Der Bereich ist nützlich, wenn ein Administrator möchte, dass bestimmte e-Mail-Infos für bestimmte Bereiche zugänglich sein.</span><span class="sxs-lookup"><span data-stu-id="c7a68-146">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="c7a68-147">Es ist außerdem hilfreich, Absender zu informieren, dass ihre Nachricht die Organisation, deren Unterstützung bei der richtigen Entscheidungen zu Wortlaut, Ton und Inhalte lassen kann.</span><span class="sxs-lookup"><span data-stu-id="c7a68-147">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="c7a68-148">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="c7a68-148">recipientSuggestions</span></span> | <span data-ttu-id="c7a68-149">[recipient](../resources/recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c7a68-149">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="c7a68-150">Empfänger vorgeschlagene basierend auf vorherigen Kontext, in dem sie in der gleichen Nachricht angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c7a68-150">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="c7a68-151">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="c7a68-151">totalMemberCount</span></span> | <span data-ttu-id="c7a68-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c7a68-152">Int32</span></span> | <span data-ttu-id="c7a68-153">Die Anzahl der Elemente, wenn der Empfänger eine Verteilerliste handelt.</span><span class="sxs-lookup"><span data-stu-id="c7a68-153">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7a68-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7a68-154">JSON representation</span></span>

<span data-ttu-id="c7a68-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7a68-155">Here is a JSON representation of the resource.</span></span>

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