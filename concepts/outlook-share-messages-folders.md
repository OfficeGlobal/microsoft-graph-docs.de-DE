---
title: Abrufen von Outlook-Nachrichten in einem freigegebenen oder delegierten Ordner
description: Diese Themen haben auch ähnliche Abschnitte – Ereignisse auflisten, Ereignis abrufen, Kontakte auflisten, Kontakt abrufen, Kontaktordner abrufen.
ms.openlocfilehash: d9e04527879cb32f14dc8d74a814a54150c5b2d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092250"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="32e71-103">Abrufen von Outlook-Nachrichten in einem freigegebenen oder delegierten Ordner</span><span class="sxs-lookup"><span data-stu-id="32e71-103">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="32e71-104">In Outlook können Kunden E-Mail-Ordner für andere freigeben und „Lesen“-, „Erstellen“- oder „Ändern“-Zugriff auf einzelne Ordner gewähren.</span><span class="sxs-lookup"><span data-stu-id="32e71-104">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="32e71-105">In Outlook kann ein Kunde auch einen anderen Benutzer delegieren, im Auftrag des Kunden zu handeln und auf bestimmte E-Mail-Ordner oder das gesamte Kundenpostfach zugreifen. Dies wird in Outlook auch als „Delegierung“ bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="32e71-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="32e71-106">Programmgesteuert unterstützt Microsoft Graph das Abrufen von Nachrichten in E-Mail-Ordnern, die andere Benutzer freigegeben haben, sowie das Abrufen der freigegebenen Ordner selbst.</span><span class="sxs-lookup"><span data-stu-id="32e71-106">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="32e71-107">Die Unterstützung gilt auch für Ordner, die delegiert wurden.</span><span class="sxs-lookup"><span data-stu-id="32e71-107">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="32e71-108">Beispielsweise hat Garth John Lesezugriff auf den Posteingang von Garth erteilt.</span><span class="sxs-lookup"><span data-stu-id="32e71-108">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="32e71-109">Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Mail.Read.Shared oder Mail.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Garths Mail und Posteingang zugreifen, wie nachstehend beschrieben.</span><span class="sxs-lookup"><span data-stu-id="32e71-109">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="32e71-110">Abrufen einer Nachricht im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="32e71-110">Get a message in the shared folder</span></span>

<span data-ttu-id="32e71-111">Sie können eine bestimmte Nachricht in Garths Posteingang abrufen:</span><span class="sxs-lookup"><span data-stu-id="32e71-111">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="32e71-112">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und die [message](/graph/api/resources/message?view=graph-rest-1.0)-Instanz mit der ID `{id}` aus Garths Posteingang.</span><span class="sxs-lookup"><span data-stu-id="32e71-112">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="32e71-113">Abrufen aller Nachrichten im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="32e71-113">Get all messages in the shared folder</span></span>

<span data-ttu-id="32e71-114">So rufen Sie alle Nachrichten in Garths Posteingang ab:</span><span class="sxs-lookup"><span data-stu-id="32e71-114">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="32e71-115">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine Sammlung der [message](/graph/api/resources/message?view=graph-rest-1.0)-Instanzen in Garths Posteingang.</span><span class="sxs-lookup"><span data-stu-id="32e71-115">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="32e71-116">Abrufen des freigegebenen Ordners</span><span class="sxs-lookup"><span data-stu-id="32e71-116">Get the shared folder</span></span>

<span data-ttu-id="32e71-117">Rufen Sie den Ordner (Posteingang) ab, den Garth für John freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="32e71-117">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="32e71-118">Nach erfolgreichem Abschluss erhalten Sie „HTTP 200 OK“ und eine [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)-Instanz, die den Ordner „Posteingang“ von Garth darstellt.</span><span class="sxs-lookup"><span data-stu-id="32e71-118">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="32e71-119">Dieselben GET-Funktionen würden gelten, wenn Garth an John weiteren Zugriff auf Garths Posteingang delegiert hätte oder wenn Garth sein gesamtes Postfach an John delegiert hätte.</span><span class="sxs-lookup"><span data-stu-id="32e71-119">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="32e71-120">Wenn Garth weder seinen Posteingang für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32e71-120">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="32e71-121">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="32e71-121">Next steps</span></span>

<span data-ttu-id="32e71-122">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="32e71-122">Find out more about:</span></span>

- [<span data-ttu-id="32e71-123">Gründe für die Integration in Outlook-Mail</span><span class="sxs-lookup"><span data-stu-id="32e71-123">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="32e71-124">[Verwenden der Mail-API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) und [Anwendungsfälle](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) für diese in Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="32e71-124">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>