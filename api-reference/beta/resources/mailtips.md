---
title: e-Mail-Infos Ressourcentyp
description: 'Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden. Beispielsweise eine Out-of-Office-Nachricht '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11e64c09a90d130b7656d4e87770e6df3fb67408
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508412"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="c58ea-104">e-Mail-Infos Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c58ea-104">mailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c58ea-105">Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c58ea-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="c58ea-106">Beispielsweise eine Abwesenheits Nachricht als automatische Antwort für einen Nachrichtenempfänger.</span><span class="sxs-lookup"><span data-stu-id="c58ea-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="c58ea-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c58ea-107">Properties</span></span>
| <span data-ttu-id="c58ea-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c58ea-108">Property</span></span>     | <span data-ttu-id="c58ea-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c58ea-109">Type</span></span>   |<span data-ttu-id="c58ea-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c58ea-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c58ea-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="c58ea-111">automaticReplies</span></span> | [<span data-ttu-id="c58ea-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="c58ea-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="c58ea-113">Mail-Tipps für die automatische Antwort, wenn es vom Empfänger eingerichtet wurde.</span><span class="sxs-lookup"><span data-stu-id="c58ea-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="c58ea-114">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="c58ea-114">customMailTip</span></span> | <span data-ttu-id="c58ea-115">String</span><span class="sxs-lookup"><span data-stu-id="c58ea-115">String</span></span> | <span data-ttu-id="c58ea-116">Eine benutzerdefinierte e-Mail-Info, die für das Postfach des Empfängers festgelegt werden kann.</span><span class="sxs-lookup"><span data-stu-id="c58ea-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="c58ea-117">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="c58ea-117">deliveryRestricted</span></span>| <span data-ttu-id="c58ea-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c58ea-118">Boolean</span></span> | <span data-ttu-id="c58ea-119">Gibt an, ob das Postfach des Empfängers beschränkt, beispielsweise ist akzeptieren von Nachrichten aus einer vordefinierten Liste Absender, ablehnen von Nachrichten aus einer vordefinierten Liste der Absender oder Nachrichten von nur von authentifizierten Absendern akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="c58ea-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="c58ea-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c58ea-120">emailAddress</span></span> | [<span data-ttu-id="c58ea-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c58ea-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="c58ea-122">Die e-Mail-Adresse des Empfängers zum Abrufen von e-Mail-Infos für.</span><span class="sxs-lookup"><span data-stu-id="c58ea-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="c58ea-123">error</span><span class="sxs-lookup"><span data-stu-id="c58ea-123">error</span></span> | [<span data-ttu-id="c58ea-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="c58ea-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="c58ea-125">Fehler, die während der Aktion [GetMailTips](../api/user-getmailtips.md) auftreten.</span><span class="sxs-lookup"><span data-stu-id="c58ea-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="c58ea-126">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="c58ea-126">externalMemberCount</span></span> | <span data-ttu-id="c58ea-127">Int32</span><span class="sxs-lookup"><span data-stu-id="c58ea-127">Int32</span></span> | <span data-ttu-id="c58ea-128">Die Anzahl der externen Elemente, wenn beim Empfänger um eine Verteilerliste handelt.</span><span class="sxs-lookup"><span data-stu-id="c58ea-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="c58ea-129">IsModerated</span><span class="sxs-lookup"><span data-stu-id="c58ea-129">isModerated</span></span> |<span data-ttu-id="c58ea-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c58ea-130">Boolean</span></span>  | <span data-ttu-id="c58ea-131">Gibt an, ob das Senden von Nachrichten an den Empfänger genehmigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="c58ea-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="c58ea-132">Angenommen, wurde Wenn der Empfänger eine große Verteilerliste ist und eine Moderator festgelegt bis zu an diese Verteilerliste gesendete Nachrichten genehmigen oder wenn Senden von Nachrichten an ein Empfänger Genehmigung des Managers des Empfängers erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c58ea-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="c58ea-133">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="c58ea-133">mailboxFull</span></span> | <span data-ttu-id="c58ea-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c58ea-134">Boolean</span></span> | <span data-ttu-id="c58ea-135">Der vollständige Postfachstatus des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="c58ea-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="c58ea-136">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="c58ea-136">maxMessageSize</span></span> | <span data-ttu-id="c58ea-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c58ea-137">Int32</span></span> | <span data-ttu-id="c58ea-138">Die maximale Nachrichtengröße für die Organisation oder das Postfach des Empfängers konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="c58ea-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="c58ea-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="c58ea-139">recipientScope</span></span> | <span data-ttu-id="c58ea-140">String</span><span class="sxs-lookup"><span data-stu-id="c58ea-140">String</span></span> | <span data-ttu-id="c58ea-141">Der Bereich des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="c58ea-141">The scope of the recipient.</span></span> <span data-ttu-id="c58ea-142">Mögliche Werte sind: `none`, `internal`, `external`, `externalPartner` und `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="c58ea-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="c58ea-143">Beispielsweise kann ein Administrator einer anderen Organisation zu seinem "Partner" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c58ea-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="c58ea-144">Der Bereich ist nützlich, wenn ein Administrator möchte, dass bestimmte e-Mail-Infos für bestimmte Bereiche zugänglich sein.</span><span class="sxs-lookup"><span data-stu-id="c58ea-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="c58ea-145">Es ist außerdem hilfreich, Absender zu informieren, dass ihre Nachricht die Organisation, deren Unterstützung bei der richtigen Entscheidungen zu Wortlaut, Ton und Inhalte lassen kann.</span><span class="sxs-lookup"><span data-stu-id="c58ea-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="c58ea-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="c58ea-146">recipientSuggestions</span></span> | <span data-ttu-id="c58ea-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="c58ea-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="c58ea-148">Empfänger vorgeschlagene basierend auf vorherigen Kontext, in dem sie in der gleichen Nachricht angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c58ea-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="c58ea-149">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="c58ea-149">totalMemberCount</span></span> | <span data-ttu-id="c58ea-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c58ea-150">Int32</span></span> | <span data-ttu-id="c58ea-151">Die Anzahl der Elemente, wenn der Empfänger eine Verteilerliste handelt.</span><span class="sxs-lookup"><span data-stu-id="c58ea-151">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c58ea-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c58ea-152">JSON representation</span></span>

<span data-ttu-id="c58ea-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c58ea-153">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
