---
title: Verwenden Sie die Microsoft Graph-API für soziale Netzwerke Intelligence in einer app integrieren
description: Microsoft Graph unterstützt für soziale Netzwerke Gesten in sozialen Kontext des Benutzers und ermöglicht den Zugriff auf nützliche Personen und Daten in sozialen Netzwerken.
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: 3ccc574a966c5a0dc81f62fe4fa0a595fb25a982
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944880"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="abed7-103">Verwenden Sie die Microsoft Graph-API für soziale Netzwerke Intelligence in einer app integrieren</span><span class="sxs-lookup"><span data-stu-id="abed7-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

> <span data-ttu-id="abed7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="abed7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abed7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="abed7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="abed7-106">Microsoft Graph unterstützt für soziale Netzwerke Gesten in sozialen Kontext des Benutzers und ermöglicht den Zugriff auf nützliche Personen und Daten in sozialen Netzwerken.</span><span class="sxs-lookup"><span data-stu-id="abed7-106">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="abed7-107">Aggregieren Sie und extrahieren Sie spezifische Informationen zu Personen</span><span class="sxs-lookup"><span data-stu-id="abed7-107">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="abed7-108">Verwenden Sie die [Person](../resources/person.md) -Ressource und die API Personen aggregierte Informationen von einer Person über e-Mail, Kontakte und sozialen Netzwerken.</span><span class="sxs-lookup"><span data-stu-id="abed7-108">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="abed7-109">Die Ergebnisse werden nach ihrer Relevanz basierend auf mehreren Kommunikation, Zusammenarbeit und Business Beziehungen sortiert.</span><span class="sxs-lookup"><span data-stu-id="abed7-109">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="abed7-110">Die API können Sie durchsuchen, sortieren, auswählen, filtern oder suchen Sie nach Personen basierend auf den angegebenen Suchkriterien.</span><span class="sxs-lookup"><span data-stu-id="abed7-110">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="abed7-111">List people</span><span class="sxs-lookup"><span data-stu-id="abed7-111">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="abed7-112">Verwalten von @ Erwähnungen</span><span class="sxs-lookup"><span data-stu-id="abed7-112">Manage @-Mentions</span></span>

<span data-ttu-id="abed7-113">Aufrufen von einen Empfänger zu benachrichtigen und Aufmerksamkeit des Empfängers in einer Nachricht erhalten möchten, ist eine allgemeine für soziale Netzwerke Eingabeaktion.</span><span class="sxs-lookup"><span data-stu-id="abed7-113">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="abed7-114">Die Ressource [erwähnen](../resources/mention.md) und die API erwähnt bieten einen leicht Mechanismus, rufen Sie einen Empfänger in einer [Nachricht](../resources/message.md), erhalten alle Nachrichten, die in denen ein Benutzer benachrichtigt wird mithilfe der @ Erwähnung oder jede Erwähnung in einer Nachricht erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="abed7-114">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="abed7-115">Erstellen von erwähnungen in einer neuen Nachricht</span><span class="sxs-lookup"><span data-stu-id="abed7-115">Create mentions in a new message</span></span>

  - [<span data-ttu-id="abed7-116">Erstellen und Senden von erwähnungen im Rahmen einer neuen Nachricht</span><span class="sxs-lookup"><span data-stu-id="abed7-116">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="abed7-117">Erstellen von erwähnungen als Teil eines e-Mail-Entwurfs</span><span class="sxs-lookup"><span data-stu-id="abed7-117">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="abed7-118">Abrufen von Informationen über erwähnungen in einer Nachricht</span><span class="sxs-lookup"><span data-stu-id="abed7-118">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="abed7-119">Abrufen Sie aller Nachrichten im Postfach des angemeldeten Benutzers, in denen den Benutzer erwähnt</span><span class="sxs-lookup"><span data-stu-id="abed7-119">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="abed7-120">Abrufen von Details der einzelnen Erwähnung in einer Nachricht</span><span class="sxs-lookup"><span data-stu-id="abed7-120">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="abed7-121">[Löschen der Vermerk](../api/message-delete.md#request-2) in einer Nachricht</span><span class="sxs-lookup"><span data-stu-id="abed7-121">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="abed7-122">Zugriff auf Daten in sozialen Netzwerken um sowie zu einem Benutzer</span><span class="sxs-lookup"><span data-stu-id="abed7-122">Access social data around and about a user</span></span>

<span data-ttu-id="abed7-123">Office-Diagramm kapselt die Beziehungen zwischen verschiedenen Entitäten in Office 365.</span><span class="sxs-lookup"><span data-stu-id="abed7-123">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="abed7-124">Verwenden Sie Office-Diagramm um soziale Einsichten in einzelne Benutzer über Office 365 abzurufen.</span><span class="sxs-lookup"><span data-stu-id="abed7-124">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="abed7-125">Liste der Elemente [Trend, um](../api/insights-list-trending.md) einen Benutzer</span><span class="sxs-lookup"><span data-stu-id="abed7-125">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="abed7-126">Auflisten von Waren, [Arbeiten mit](../api/user-list-people.md) Benutzern eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="abed7-126">List users who have been [working with](../api/user-list-people.md) a user</span></span>
