---
title: Abrufen von Outlook-Kontakten in einem freigegebenen Ordner
description: " es gibt außerdem "
author: angelgolfer-ms
ms.openlocfilehash: a3dd8cff5cac88d3ef273b63f40bc8af87910aa1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315176"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="40c26-103">Abrufen von Outlook-Kontakten in einem freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="40c26-103">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="40c26-104">In Outlook können Kunden Ordner für andere freigeben und den Zugriff zum Lesen, Erstellen oder Ändern auf einzelne Kontaktordner erteilen.</span><span class="sxs-lookup"><span data-stu-id="40c26-104">Outlook lets customers share folders with one another and provide "read", "create", "modify", or "delete" access to individual contact folders.</span></span> <span data-ttu-id="40c26-105">In Outlook kann ein Kunde auch einen anderen Benutzer delegieren, im Auftrag des Kunden zu handeln und auf bestimmte Ordner oder das gesamte Kundenpostfach zugreifen. Dies wird in Outlook auch als "Delegierung" bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="40c26-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="40c26-106">Programmgesteuert unterstützt Microsoft Graph das Abrufen von Kontakten in Kontaktordnern, die andere Benutzer freigegeben haben, sowie das Abrufen der freigegebenen Ordner selbst.</span><span class="sxs-lookup"><span data-stu-id="40c26-106">Programmatically, Microsoft Graph supports getting contacts in contact folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="40c26-107">Die Unterstützung gilt auch für Ordner in einem delegierten Postfach.</span><span class="sxs-lookup"><span data-stu-id="40c26-107">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="40c26-108">Beispielsweise hat Adrian für John einen benutzerdefinierten Kontaktordner freigegeben und John Lesezugriff erteilt.</span><span class="sxs-lookup"><span data-stu-id="40c26-108">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="40c26-109">Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Contacts.Read.Shared oder Contacts.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Adrians benutzerdefinierten Kontaktordner und auf die Kontakte in diesem Ordner zugreifen, wie nachstehend beschrieben.</span><span class="sxs-lookup"><span data-stu-id="40c26-109">If John has signed into your app and provided delegated permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared), your app will be able to access Garth's custom contact folder and contacts in that folder as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="40c26-110">Abrufen eines Kontakts im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="40c26-110">Get a contact in the shared folder</span></span>

<span data-ttu-id="40c26-111">Sie können einen bestimmten Kontakt im benutzerdefinierten Kontaktordner abrufen, den Adrian für John freigegeben hat:</span><span class="sxs-lookup"><span data-stu-id="40c26-111">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="40c26-112">Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und die [contact](/graph/api/resources/contact?view=graph-rest-1.0)-Instanz mit der ID `{id}` aus Adrians freigegebenem Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="40c26-112">On successful completion, you'll get HTTP 200 OK and the [contact](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's shared contact folder.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="40c26-113">Abrufen aller Kontakte im freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="40c26-113">Get all contacts in the shared folder</span></span>

<span data-ttu-id="40c26-114">Abrufen aller Kontakte in Adrians freigegebenem Kontaktordner:</span><span class="sxs-lookup"><span data-stu-id="40c26-114">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="40c26-115">Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine Sammlung der [contact](/graph/api/resources/contact?view=graph-rest-1.0)-Instanzen in Adrians freigegebenem Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="40c26-115">On successful completion, you'll get HTTP 200 OK and a collection of [contact](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's shared contact folder.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="40c26-116">Abrufen des freigegebenen Ordners</span><span class="sxs-lookup"><span data-stu-id="40c26-116">Get the shared folder</span></span>

<span data-ttu-id="40c26-117">Abrufen des Kontaktordners, den Adrian für John freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="40c26-117">Get the contact folder that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="40c26-118">Nach erfolgreichem Abschluss erhalten Sie "HTTP 200 OK" und eine [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)-Instanz, die Adrians freigegebenen Kontaktordner darstellt.</span><span class="sxs-lookup"><span data-stu-id="40c26-118">On successful completion, you'll get HTTP 200 OK and a [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's shared contact folder.</span></span>

<span data-ttu-id="40c26-119">Die gleichen GET-Funktionen würden ebenfalls gelten, wenn Adrian sein gesamtes Postfach an John delegiert hätte.</span><span class="sxs-lookup"><span data-stu-id="40c26-119">The same GET capabilities apply if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="40c26-120">Wenn Adrian weder den Kontaktordner für John freigegeben noch sein Postfach an John delegiert hat, wird bei der Angabe von Adrians Benutzer-ID oder seines Benutzerprinzipalnamens bei diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40c26-120">If Garth has not shared the contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="40c26-121">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="40c26-121">Next steps</span></span>

<span data-ttu-id="40c26-122">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="40c26-122">Find out more about:</span></span>

- [<span data-ttu-id="40c26-123">Warum persönliche Kontakte in Outlook integrieren?</span><span class="sxs-lookup"><span data-stu-id="40c26-123">Why integrate with Outlook personal contacts</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="40c26-124">Die [Kontakte-API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="40c26-124">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>