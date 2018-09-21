# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="2518b-101">Abrufen von Outlook-Kontakten in einem freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="2518b-101">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="2518b-102">Mit Outlook können Benutzer Ordner freigeben und den Zugriff auf einzelne Kontaktordner "lesen", "erstellen", "ändern" oder "löschen" aktivieren.</span><span class="sxs-lookup"><span data-stu-id="2518b-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="2518b-103">Outlook ermöglicht es einem Kunden auch, einen anderen Benutzer zu delegieren, um im Auftrag des Kunden zu handeln und auf bestimmte Ordner oder das gesamte Postfach des Kunden zuzugreifen. Dies wird in Outlook auch als "Delegierung" bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="2518b-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="2518b-104">Programmgesteuert unterstützt Microsoft Graph das Abrufen von Kontakten in Kontaktordnern, die von anderen Benutzern freigegeben wurden, sowie das Abrufen der freigegebenen Ordner selbst.</span><span class="sxs-lookup"><span data-stu-id="2518b-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="2518b-105">Der Support gilt auch für Ordner in einem delegierten Postfach.</span><span class="sxs-lookup"><span data-stu-id="2518b-105">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="2518b-106">Als Beispiel hat Garth mit John einen benutzerdefinierten Kontaktordner geteilt und John Lesezugriff gewährt.</span><span class="sxs-lookup"><span data-stu-id="2518b-106">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="2518b-107">Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Contacts.Read.Shared oder Contacts.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf den benutzerdefinierten Kontaktordner und die Kontakte von Garth in diesem Ordner zugreifen, wie nachfolgend beschrieben.</span><span class="sxs-lookup"><span data-stu-id="2518b-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="2518b-108">Abrufen eines Kontakts in den freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="2518b-108">Get a message in the shared folder</span></span>

<span data-ttu-id="2518b-109">Sie können einen bestimmten Kontakt in dem benutzerdefinierten Kontaktordner abrufen, den Garth mit John geteilt hat:</span><span class="sxs-lookup"><span data-stu-id="2518b-109">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="2518b-110">Nach erfolgreichem Abschluss erhalten Sie HTTP 200 OK und die [ Kontakt](../api-reference/v1.0/resources/contact.md) -Instanz, die von`{id}`   aus dem gemeinsamen Kontaktordner von Garth identifiziert wurde.</span><span class="sxs-lookup"><span data-stu-id="2518b-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/contact.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="2518b-111">Abrufen aller Kontakte in dem freigegebenen Ordner</span><span class="sxs-lookup"><span data-stu-id="2518b-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="2518b-112">Abrufen aller Kontakte in Garths freigegebenem Kontaktordner:</span><span class="sxs-lookup"><span data-stu-id="2518b-112">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="2518b-113">Nach erfolgreichem Abschluss erhalten Sie HTTP 200 OK und eine Sammlung von [Kontakt](../api-reference/v1.0/resources/contact.md) Instanzen im gemeinsamen Kontaktordner von Garth.</span><span class="sxs-lookup"><span data-stu-id="2518b-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/contact.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="2518b-114">Abrufen des freigegebenen Ordners</span><span class="sxs-lookup"><span data-stu-id="2518b-114">Get the shared folder</span></span>

<span data-ttu-id="2518b-115">Abrufen des Kontaktordners, den Garth mit John geteilt hat.</span><span class="sxs-lookup"><span data-stu-id="2518b-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="2518b-116">Nach erfolgreichem Abschluss erhalten Sie HTTP 200 OK und eine [contactFolder](../api-reference/v1.0/resources/contactfolder.md) Instanz, die Garths gemeinsamen Kontaktordner darstellt.</span><span class="sxs-lookup"><span data-stu-id="2518b-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/contactfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="2518b-117">Die gleichen GET-Fähigkeiten gelten, wenn Garth John sein gesamtes Postfach übertragen hat.</span><span class="sxs-lookup"><span data-stu-id="2518b-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="2518b-118">Wenn Garth den Kontaktordner nicht mit John geteilt hat oder sein Postfach an John übertragen hat, gibt die Angabe der Benutzer-ID oder des Benutzernamens von Garth in diesen GET-Operationen einen Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="2518b-118">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="2518b-119">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="2518b-119">Next steps</span></span>

<span data-ttu-id="2518b-120">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="2518b-120">Find out more about:</span></span>

- [<span data-ttu-id="2518b-121">Warum persönliche Kontakte in Outlook integrieren?</span><span class="sxs-lookup"><span data-stu-id="2518b-121">Why integrate with Outlook personal contacts?</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="2518b-122">Die [Kontakte API](../api-reference/v1.0/resources/contact.md) in Microsoft Graph v1. 0.</span><span class="sxs-lookup"><span data-stu-id="2518b-122">The [contacts API](../api-reference/v1.0/resources/contact.md) in Microsoft Graph v1.0.</span></span>