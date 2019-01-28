---
title: Verwenden der Microsoft Graph-API, um soziale Intelligenz in eine App zu integrieren
description: Microsoft Graph unterstützt soziale Gesten im sozialen Kontext des Benutzers und bietet Zugriff auf hilfreiche Personen- und soziale Daten.
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: b5a89f46c8480fb90cd019e5b4fb370e0a6592bf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509595"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="511ac-103">Verwenden der Microsoft Graph-API, um soziale Intelligenz in eine App zu integrieren</span><span class="sxs-lookup"><span data-stu-id="511ac-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="511ac-104">Microsoft Graph unterstützt soziale Gesten im sozialen Kontext des Benutzers und bietet Zugriff auf hilfreiche Personen- und soziale Daten.</span><span class="sxs-lookup"><span data-stu-id="511ac-104">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="511ac-105">Sammeln und Extrahieren von spezifischen Informationen zu Personen</span><span class="sxs-lookup"><span data-stu-id="511ac-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="511ac-106">Sie können die [person](../resources/person.md)-Ressource und die Personen-API zum Aggregieren von Informationen über eine Person aus E-Mails, Kontakten und sozialen Netzwerken verwenden.</span><span class="sxs-lookup"><span data-stu-id="511ac-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="511ac-107">Die Ergebnisse werden nach ihrer Relevanz basierend auf Mustern bei der Kommunikation und Zusammenarbeit sowie auf Geschäftsbeziehungen sortiert.</span><span class="sxs-lookup"><span data-stu-id="511ac-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="511ac-108">Mit der API können Sie Personen durchsuchen, sortieren, auswählen, filtern oder anhand eigener Kriterien nach Personen suchen.</span><span class="sxs-lookup"><span data-stu-id="511ac-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="511ac-109">Personen auflisten</span><span class="sxs-lookup"><span data-stu-id="511ac-109">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="511ac-110">Verwalten von @-Erwähnungen</span><span class="sxs-lookup"><span data-stu-id="511ac-110">Manage @-Mentions</span></span>

<span data-ttu-id="511ac-111">Es ist eine häufige soziale Geste, einen Empfänger zu benachrichtigen und die Aufmerksamkeit des Empfängers auf eine Nachricht zu lenken.</span><span class="sxs-lookup"><span data-stu-id="511ac-111">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="511ac-112">Die [mention](../resources/mention.md)-Ressource und die Erwähnungs-API bieten eine einfache Methode, um einen Empfänger in einer [Nachricht](../resources/message.md) zu benachrichtigen, alle Nachrichten mithilfe einer @-Erwähnung abzurufen, in denen ein Benutzer benachrichtigt wird, oder alle Erwähnungen in einer Nachricht abzurufen.</span><span class="sxs-lookup"><span data-stu-id="511ac-112">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="511ac-113">Erstellen von Erwähnungen in einer neuen Nachricht</span><span class="sxs-lookup"><span data-stu-id="511ac-113">Create mentions in a new message</span></span>

  - [<span data-ttu-id="511ac-114">Erstellen und Senden von Erwähnungen als Teil einer neuen Nachricht</span><span class="sxs-lookup"><span data-stu-id="511ac-114">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="511ac-115">Erstellen von Erwähnungen als Teil eines E-Mail-Entwurfs</span><span class="sxs-lookup"><span data-stu-id="511ac-115">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="511ac-116">Abrufen von Informationen zu Erwähnungen in einer Nachricht</span><span class="sxs-lookup"><span data-stu-id="511ac-116">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="511ac-117">Abrufen aller Nachrichten im Postfach des angemeldeten Benutzers, in denen der Benutzer erwähnt wird</span><span class="sxs-lookup"><span data-stu-id="511ac-117">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="511ac-118">Abrufen von Details zu den einzelnen Erwähnungen in einer Nachricht</span><span class="sxs-lookup"><span data-stu-id="511ac-118">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="511ac-119">[Löschen einer Erwähnung](../api/message-delete.md#request-2) in einer Nachricht</span><span class="sxs-lookup"><span data-stu-id="511ac-119">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="511ac-120">Zugriff auf Daten aus sozialen Netzwerken und über einen Benutzer</span><span class="sxs-lookup"><span data-stu-id="511ac-120">Access social data around and about a user</span></span>

<span data-ttu-id="511ac-121">Office Graph fasst die Beziehungen zwischen unterschiedlichen Entitäten in Office 365 zusammen.</span><span class="sxs-lookup"><span data-stu-id="511ac-121">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="511ac-122">Verwenden Sie Office Graph, um soziale Einblicke zu einzelnen Benutzern in Office 365 zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="511ac-122">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="511ac-123">Auflisten der Elemente, die bei einem Benutzer [beliebt sind](../api/insights-list-trending.md)</span><span class="sxs-lookup"><span data-stu-id="511ac-123">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="511ac-124">Auflisten der Benutzer, die [mit einem Benutzer gearbeitet haben](../api/user-list-people.md)</span><span class="sxs-lookup"><span data-stu-id="511ac-124">List users who have been [working with](../api/user-list-people.md) a user</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/social-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
