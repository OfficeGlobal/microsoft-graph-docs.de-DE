---
title: Abrufen von Outlook-Nachrichten in einem freigegebenen oder delegierten Ordner
description: In Outlook können Kunden E-Mail-Ordner für andere freigeben und „Lesen“-, „Erstellen“- oder „Ändern“-Zugriff auf einzelne Ordner gewähren. In Outlook kann ein Kunde auch einen anderen Benutzer delegieren, um im Auftrag des Kunden zu handeln.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 76f54b5cc2db5395b9ca5e50611c4cea4f18b770
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917391"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="768cb-104">Abrufen von Outlook-Nachrichten in einem freigegebenen oder delegierten Ordner</span><span class="sxs-lookup"><span data-stu-id="768cb-104">Get Outlook messages in a shared or delegated folder</span></span>

<span data-ttu-id="768cb-105">In Outlook können Kunden E-Mail-Ordner für andere freigeben und „Lesen“-, „Erstellen“- oder „Ändern“-Zugriff auf einzelne Ordner gewähren.</span><span class="sxs-lookup"><span data-stu-id="768cb-105">Outlook lets customers share mail folders with one another and provide "read", "create", "modify", or "delete" access to individual folders.</span></span> <span data-ttu-id="768cb-106">In Outlook kann ein Kunde auch einen anderen Benutzer delegieren, im Auftrag des Kunden zu handeln und auf bestimmte E-Mail-Ordner oder das gesamte Kundenpostfach zugreifen. Dies wird in Outlook auch als „Delegierung“ bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="768cb-106">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="768cb-107">Programmgesteuert unterstützt Microsoft Graph das Abrufen von Nachrichten in E-Mail-Ordnern, die andere Benutzer freigegeben haben, sowie das Abrufen der freigegebenen Ordner selbst.</span><span class="sxs-lookup"><span data-stu-id="768cb-107">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="768cb-108">Die Unterstützung gilt auch für Ordner, die delegiert wurden.</span><span class="sxs-lookup"><span data-stu-id="768cb-108">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="768cb-109">Beispielsweise hat Garth John Lesezugriff auf den Posteingang von Garth erteilt.</span><span class="sxs-lookup"><span data-stu-id="768cb-109">As an example, Garth has shared with John and given read access to Garth's Inbox.</span></span> <span data-ttu-id="768cb-110">Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Mail.Read.Shared oder Mail.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Garths Mail und Posteingang zugreifen, wie nachstehend beschrieben.</span><span class="sxs-lookup"><span data-stu-id="768cb-110">If John has signed into your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

> <span data-ttu-id="768cb-111">**Hinweis** Mithilfe der Freigabeberechtigungen (Mail.Read.Shared oder Mail.ReadWrite.Shared) können Sie Ereignisse in einem freigegebenen oder delegierten Ordner lesen oder schreiben.</span><span class="sxs-lookup"><span data-stu-id="768cb-111">**Note** The sharing permissions (Mail.Read.Shared or Mail.ReadWrite.Shared) allow you to read or write messages in a shared or delegated folder.</span></span> <span data-ttu-id="768cb-112">[Das Abonnieren von Änderungsbenachrichtigungen](webhooks.md) wird für Elemente in solchen Ordnern nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="768cb-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="768cb-113">Verwenden Sie zum Einrichten von Änderungsbenachrichtigungsabonnements für Nachrichten in einem freigegebenen, delegierten oder einem Postfachordner eines anderen Benutzers im Mandanten die Berechtigung „Mail.Read“.</span><span class="sxs-lookup"><span data-stu-id="768cb-113">To set up change notification subscriptions on messages in a shared, delegated, or any other user's mail folder in the tenant, use the application permission, Mail.Read.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="768cb-114">Abrufen einer Nachricht im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="768cb-114">Get a message in the shared folder</span></span>

<span data-ttu-id="768cb-115">Sie können eine bestimmte Nachricht in Garths Posteingang abrufen:</span><span class="sxs-lookup"><span data-stu-id="768cb-115">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="768cb-116">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und die [message](/graph/api/resources/message?view=graph-rest-1.0)-Instanz mit der ID `{id}` aus Garths Posteingang.</span><span class="sxs-lookup"><span data-stu-id="768cb-116">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="768cb-117">Abrufen aller Nachrichten im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="768cb-117">Get all messages in the shared folder</span></span>

<span data-ttu-id="768cb-118">So rufen Sie alle Nachrichten in Garths Posteingang ab:</span><span class="sxs-lookup"><span data-stu-id="768cb-118">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="768cb-119">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine Sammlung der [message](/graph/api/resources/message?view=graph-rest-1.0)-Instanzen in Garths Posteingang.</span><span class="sxs-lookup"><span data-stu-id="768cb-119">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="768cb-120">Abrufen des freigegebenen Ordners</span><span class="sxs-lookup"><span data-stu-id="768cb-120">Get the shared folder</span></span>

<span data-ttu-id="768cb-121">Rufen Sie den Ordner (Posteingang) ab, den Garth für John freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="768cb-121">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="768cb-122">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)-Instanz, die den Ordner „Posteingang“ von Garth darstellt.</span><span class="sxs-lookup"><span data-stu-id="768cb-122">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="768cb-123">Dieselben GET-Funktionen würden gelten, wenn Garth an John weiteren Zugriff auf Garths Posteingang delegiert hätte oder wenn Garth sein gesamtes Postfach an John delegiert hätte.</span><span class="sxs-lookup"><span data-stu-id="768cb-123">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="768cb-124">Wenn Garth weder seinen Posteingang für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="768cb-124">If Garth has not shared his Inbox with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="768cb-125">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="768cb-125">Next steps</span></span>

<span data-ttu-id="768cb-126">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="768cb-126">Find out more about:</span></span>

- [<span data-ttu-id="768cb-127">Gründe für die Integration in Outlook-Mail</span><span class="sxs-lookup"><span data-stu-id="768cb-127">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="768cb-128">[Verwenden der Mail-API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) und [Anwendungsfälle](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) für diese in Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="768cb-128">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>
