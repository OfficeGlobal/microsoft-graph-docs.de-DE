---
title: mailFolder-Ressoucentyp
description: Ein mailFolder-Element im Postfach eines Benutzers, wie z. B. Posteingang und Entwürfe. Mailordner können Nachrichten, andere Outlook-Elemente und untergeordnete E-Mail-Ordner enthalten.
ms.openlocfilehash: 96e2b6cf2af9ffbe6a6c66d41efe174d1706074d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017388"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="6f16d-104">mailFolder-Ressoucentyp</span><span class="sxs-lookup"><span data-stu-id="6f16d-104">mailFolder resource type</span></span>

<span data-ttu-id="6f16d-105">Ein mailFolder-Element im Postfach eines Benutzers, wie z. B. Posteingang und Entwürfe.</span><span class="sxs-lookup"><span data-stu-id="6f16d-105">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="6f16d-106">Mailordner können Nachrichten, andere Outlook-Elemente und untergeordnete E-Mail-Ordner enthalten.</span><span class="sxs-lookup"><span data-stu-id="6f16d-106">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="6f16d-107">Diese Ressource unterstützt die Verwendung einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen einer [delta](../api/mailfolder-delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="6f16d-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="6f16d-108">**Bekannte Ordnernamen**</span><span class="sxs-lookup"><span data-stu-id="6f16d-108">**Well-known folder names**</span></span>

<span data-ttu-id="6f16d-109">Outlook erstellt standardmäßig bestimmte Ordner für Benutzer.</span><span class="sxs-lookup"><span data-stu-id="6f16d-109">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="6f16d-110">Statt des **ID-** Werts des entsprechenden Ordner für zu diesem Zweck können Sie die bekannte Ordnernamen aus der folgenden Tabelle beim Zugriff auf diese Ordner.</span><span class="sxs-lookup"><span data-stu-id="6f16d-110">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="6f16d-111">Beispielsweise können Sie den Ordner "Entwürfe" unter Verwendung seines bekannte namens mit der folgenden Abfrage abrufen.</span><span class="sxs-lookup"><span data-stu-id="6f16d-111">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="6f16d-112">Bekannte Namen arbeiten unabhängig von dem Gebietsschema des Postfach des Benutzers, der oben genannten Abfrage immer Ordner "Entwürfe" des Benutzers, unabhängig davon, wie heißt zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="6f16d-112">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="6f16d-113">Bekannte Ordnername</span><span class="sxs-lookup"><span data-stu-id="6f16d-113">Well-known folder name</span></span> | <span data-ttu-id="6f16d-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f16d-114">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="6f16d-115">Archiv</span><span class="sxs-lookup"><span data-stu-id="6f16d-115">archive</span></span> | <span data-ttu-id="6f16d-116">Bei Verwendung von One_Click Archiv-Features in Outlook-Clients, die dies unterstützen, werden die Nachrichten archivieren Ordner an gesendet.</span><span class="sxs-lookup"><span data-stu-id="6f16d-116">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="6f16d-117">**Hinweis:** Dies ist nicht das gleiche wie das Archivpostfach Feature von Exchange online.</span><span class="sxs-lookup"><span data-stu-id="6f16d-117">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="6f16d-118">Unübersichtlichkeit</span><span class="sxs-lookup"><span data-stu-id="6f16d-118">clutter</span></span> | <span data-ttu-id="6f16d-119">Die Unübersichtlichkeit Ordner niedriger Priorität Nachrichten werden in verschoben, beim Verwenden des Features Unübersichtlichkeit.</span><span class="sxs-lookup"><span data-stu-id="6f16d-119">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="6f16d-120">Konflikte</span><span class="sxs-lookup"><span data-stu-id="6f16d-120">conflicts</span></span> | <span data-ttu-id="6f16d-121">Der Ordner, der miteinander in Konflikt stehende Elemente im Postfach enthält.</span><span class="sxs-lookup"><span data-stu-id="6f16d-121">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="6f16d-122">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="6f16d-122">conversationhistory</span></span> | <span data-ttu-id="6f16d-123">Der Ordner, in dem Skype Sofortnachrichtenunterhaltungen speichert (falls Skype dazu konfiguriert ist).</span><span class="sxs-lookup"><span data-stu-id="6f16d-123">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="6f16d-124">deleteditems</span><span class="sxs-lookup"><span data-stu-id="6f16d-124">deleteditems</span></span> | <span data-ttu-id="6f16d-125">Der Ordnerelemente werden in verschoben, wenn sie gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="6f16d-125">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="6f16d-126">Entwürfe</span><span class="sxs-lookup"><span data-stu-id="6f16d-126">drafts</span></span> | <span data-ttu-id="6f16d-127">Der Ordner, der nicht gesendete Nachrichten enthält.</span><span class="sxs-lookup"><span data-stu-id="6f16d-127">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="6f16d-128">Posteingang</span><span class="sxs-lookup"><span data-stu-id="6f16d-128">inbox</span></span> | <span data-ttu-id="6f16d-129">Der Posteingangsordner.</span><span class="sxs-lookup"><span data-stu-id="6f16d-129">The inbox folder.</span></span> |
| <span data-ttu-id="6f16d-130">junkemail</span><span class="sxs-lookup"><span data-stu-id="6f16d-130">junkemail</span></span> | <span data-ttu-id="6f16d-131">Der junk-e-Mail-Ordner.</span><span class="sxs-lookup"><span data-stu-id="6f16d-131">The junk email folder.</span></span> |
| <span data-ttu-id="6f16d-132">localfailures</span><span class="sxs-lookup"><span data-stu-id="6f16d-132">localfailures</span></span> | <span data-ttu-id="6f16d-133">Der Ordner, der Elemente enthält, die auf dem lokalen Client vorhanden, jedoch nicht auf den Server hochgeladen werden konnte.</span><span class="sxs-lookup"><span data-stu-id="6f16d-133">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="6f16d-134">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="6f16d-134">msgfolderroot</span></span> | <span data-ttu-id="6f16d-135">Der Ordner "Oberste Ebene des Informationsspeichers".</span><span class="sxs-lookup"><span data-stu-id="6f16d-135">The "Top of Information Store" folder.</span></span> <span data-ttu-id="6f16d-136">Dieser Ordner ist des übergeordneten Ordners für Ordner, in der normalen e-Mail-Clients, wie beispielsweise dem Posteingang angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="6f16d-136">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="6f16d-137">Postausgang</span><span class="sxs-lookup"><span data-stu-id="6f16d-137">outbox</span></span> | <span data-ttu-id="6f16d-138">Der Ordner Postausgang.</span><span class="sxs-lookup"><span data-stu-id="6f16d-138">The outbox folder.</span></span> |
| <span data-ttu-id="6f16d-139">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="6f16d-139">recoverableitemsdeletions</span></span> | <span data-ttu-id="6f16d-140">Der Ordner, das vorläufig gelöschte Elemente enthält: gelöscht, aus dem Ordner Gelöschte Objekte oder durch Drücken von UMSCHALT + ENTF in Outlook.</span><span class="sxs-lookup"><span data-stu-id="6f16d-140">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="6f16d-141">Dieser Ordner ist nicht sichtbar, alle Outlook-e-Mail-Client, jedoch können Endbenutzer über das Feature **Gelöschte Elemente wiederherstellen, vom Server** in Outlook oder Outlook im Web mit ihm interagieren.</span><span class="sxs-lookup"><span data-stu-id="6f16d-141">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="6f16d-142">Geplant</span><span class="sxs-lookup"><span data-stu-id="6f16d-142">scheduled</span></span> | <span data-ttu-id="6f16d-143">Der Ordner, der Nachrichten enthält, die im Posteingang mit der Zeitplan in Outlook für iOS eingeblendet geplant werden.</span><span class="sxs-lookup"><span data-stu-id="6f16d-143">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="6f16d-144">SearchFolders</span><span class="sxs-lookup"><span data-stu-id="6f16d-144">searchfolders</span></span> | <span data-ttu-id="6f16d-145">Der übergeordnete Ordner für alle im Postfach des Benutzers definierten Suchordner.</span><span class="sxs-lookup"><span data-stu-id="6f16d-145">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="6f16d-146">Gesendete Elemente</span><span class="sxs-lookup"><span data-stu-id="6f16d-146">sentitems</span></span> | <span data-ttu-id="6f16d-147">Ordner "Gesendete Elemente".</span><span class="sxs-lookup"><span data-stu-id="6f16d-147">The sent items folder.</span></span> |
| <span data-ttu-id="6f16d-148">serverfailures</span><span class="sxs-lookup"><span data-stu-id="6f16d-148">serverfailures</span></span> | <span data-ttu-id="6f16d-149">Der Ordner, der Elemente enthält, die auf dem Server vorhanden, aber konnte nicht auf dem lokalen Client synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="6f16d-149">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="6f16d-150">syncissues</span><span class="sxs-lookup"><span data-stu-id="6f16d-150">syncissues</span></span> | <span data-ttu-id="6f16d-151">Der Ordner, der von Outlook erstellten Synchronisierungsprotokolle enthält.</span><span class="sxs-lookup"><span data-stu-id="6f16d-151">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="6f16d-152">Methoden</span><span class="sxs-lookup"><span data-stu-id="6f16d-152">Methods</span></span>

| <span data-ttu-id="6f16d-153">Methode</span><span class="sxs-lookup"><span data-stu-id="6f16d-153">Method</span></span> | <span data-ttu-id="6f16d-154">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6f16d-154">Return Type</span></span> | <span data-ttu-id="6f16d-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f16d-155">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="6f16d-156">Get mailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-156">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="6f16d-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-157">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="6f16d-158">Dient zum Lesen der Eigenschaften und der Beziehungen des mailFolder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f16d-158">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="6f16d-159">Create MailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-159">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="6f16d-160">MailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-160">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="6f16d-161">Dient zum Erstellen eines neuen mailFolder-Elements unter dem aktuellen durch die Veröffentlichung der childFolders-Sammlung.</span><span class="sxs-lookup"><span data-stu-id="6f16d-161">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="6f16d-162">List childFolders</span><span class="sxs-lookup"><span data-stu-id="6f16d-162">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="6f16d-163">[MailFolder](mailfolder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f16d-163">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="6f16d-p107">Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.</span><span class="sxs-lookup"><span data-stu-id="6f16d-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="6f16d-166">Create Message</span><span class="sxs-lookup"><span data-stu-id="6f16d-166">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="6f16d-167">Nachricht</span><span class="sxs-lookup"><span data-stu-id="6f16d-167">Message</span></span>](message.md)| <span data-ttu-id="6f16d-168">Dient zum Erstellen einer neuen Nachricht in dem aktuellen mailFolder-Element durch die Veröffentlichung in der Nachrichtensammlung.</span><span class="sxs-lookup"><span data-stu-id="6f16d-168">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="6f16d-169">List messages</span><span class="sxs-lookup"><span data-stu-id="6f16d-169">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="6f16d-170">[Nachrichten](message.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f16d-170">[Message](message.md) collection</span></span>| <span data-ttu-id="6f16d-171">Dient zum Abrufen aller Nachrichten im Postfach des angemeldeten Benutzers oder Nachrichten in einen bestimmten Ordner im Postfach.</span><span class="sxs-lookup"><span data-stu-id="6f16d-171">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="6f16d-172">Update</span><span class="sxs-lookup"><span data-stu-id="6f16d-172">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="6f16d-173">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-173">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="6f16d-174">Dient zum Aktualisieren des angegebenen mailFolder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f16d-174">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="6f16d-175">Delete</span><span class="sxs-lookup"><span data-stu-id="6f16d-175">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="6f16d-176">Keine</span><span class="sxs-lookup"><span data-stu-id="6f16d-176">None</span></span> |<span data-ttu-id="6f16d-177">Dient zum Löschen des angegebenen mailFolder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f16d-177">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="6f16d-178">copy</span><span class="sxs-lookup"><span data-stu-id="6f16d-178">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="6f16d-179">MailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-179">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="6f16d-180">Dient zum Kopieren eines mailFolder-Elements und seiner Inhalte in ein anderes mailFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6f16d-180">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="6f16d-181">delta</span><span class="sxs-lookup"><span data-stu-id="6f16d-181">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="6f16d-182">[mailFolder](mailfolder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f16d-182">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="6f16d-183">Dient zum Abrufen eines Satzes von E-Mail-Ordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.</span><span class="sxs-lookup"><span data-stu-id="6f16d-183">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="6f16d-184">move</span><span class="sxs-lookup"><span data-stu-id="6f16d-184">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="6f16d-185">MailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-185">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="6f16d-186">Dient zum Verschieben eines mailFolder-Elements und seiner Inhalte in ein anderes mailFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6f16d-186">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="6f16d-187">**Erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="6f16d-187">**Extended properties**</span></span>| | |
|[<span data-ttu-id="6f16d-188">Create single-value extended property</span><span class="sxs-lookup"><span data-stu-id="6f16d-188">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="6f16d-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-189">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="6f16d-190">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen mailFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6f16d-190">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="6f16d-191">Get mailFolder with single-value extended property</span><span class="sxs-lookup"><span data-stu-id="6f16d-191">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="6f16d-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-192">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="6f16d-193">Dient zum Abrufen von mailFolders-Elementen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6f16d-193">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="6f16d-194">Create multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="6f16d-194">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="6f16d-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-195">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="6f16d-196">Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen mailFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6f16d-196">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="6f16d-197">Get mailFolder with multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="6f16d-197">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="6f16d-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6f16d-198">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="6f16d-199">Dient zum Abrufen eines mailFolders-Elements mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="6f16d-199">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="6f16d-200">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6f16d-200">Properties</span></span>

| <span data-ttu-id="6f16d-201">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f16d-201">Property</span></span> | <span data-ttu-id="6f16d-202">Typ</span><span class="sxs-lookup"><span data-stu-id="6f16d-202">Type</span></span> | <span data-ttu-id="6f16d-203">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f16d-203">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="6f16d-204">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="6f16d-204">childFolderCount</span></span>|<span data-ttu-id="6f16d-205">Int32</span><span class="sxs-lookup"><span data-stu-id="6f16d-205">Int32</span></span>|<span data-ttu-id="6f16d-206">Die Anzahl der unmittelbar untergeordneten mailFolders-Elemente in dem aktuellen mailFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6f16d-206">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="6f16d-207">displayName</span><span class="sxs-lookup"><span data-stu-id="6f16d-207">displayName</span></span>|<span data-ttu-id="6f16d-208">String</span><span class="sxs-lookup"><span data-stu-id="6f16d-208">String</span></span>|<span data-ttu-id="6f16d-209">Der Anzeigename des mailFolder-Elements.</span><span class="sxs-lookup"><span data-stu-id="6f16d-209">The mailFolder's display name.</span></span>|
|<span data-ttu-id="6f16d-210">id</span><span class="sxs-lookup"><span data-stu-id="6f16d-210">id</span></span>|<span data-ttu-id="6f16d-211">String</span><span class="sxs-lookup"><span data-stu-id="6f16d-211">String</span></span>|<span data-ttu-id="6f16d-212">Eindeutiger Bezeichner der MailFolder.</span><span class="sxs-lookup"><span data-stu-id="6f16d-212">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="6f16d-213">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="6f16d-213">parentFolderId</span></span>|<span data-ttu-id="6f16d-214">String</span><span class="sxs-lookup"><span data-stu-id="6f16d-214">String</span></span>|<span data-ttu-id="6f16d-215">Die eindeutige ID für das übergeordnete mailFolder-Element des mailFolder-Elements.</span><span class="sxs-lookup"><span data-stu-id="6f16d-215">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="6f16d-216">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="6f16d-216">totalItemCount</span></span>|<span data-ttu-id="6f16d-217">Int32</span><span class="sxs-lookup"><span data-stu-id="6f16d-217">Int32</span></span>|<span data-ttu-id="6f16d-218">Anzahl der Elemente im mailFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6f16d-218">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="6f16d-219">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="6f16d-219">unreadItemCount</span></span>|<span data-ttu-id="6f16d-220">Int32</span><span class="sxs-lookup"><span data-stu-id="6f16d-220">Int32</span></span>|<span data-ttu-id="6f16d-221">Die Anzahl der Elemente im mailFolder-Element, die als „Ungelesen“ markiert sind.</span><span class="sxs-lookup"><span data-stu-id="6f16d-221">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="6f16d-222">**Effizientes Ermitteln der Anzahl von Elementen**</span><span class="sxs-lookup"><span data-stu-id="6f16d-222">**Access item counts efficiently**</span></span>

<span data-ttu-id="6f16d-223">Die `TotalItemCount` und `UnreadItemCount` Eigenschaften eines Ordners können Sie bequem die Anzahl der gelesenen Elemente im Ordner zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="6f16d-223">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="6f16d-224">Sie können Sie die Abfragen wie folgt zu vermeiden, die erhebliche Wartezeiten auftreten kann:</span><span class="sxs-lookup"><span data-stu-id="6f16d-224">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="6f16d-225">E-Mail-Ordner in Outlook können mehrere Typen von Elementen enthalten, beispielsweise der Posteingang enthalten kann Anforderung Besprechungselemente vom e-Mail-Elemente darstellen.</span><span class="sxs-lookup"><span data-stu-id="6f16d-225">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="6f16d-226">`TotalItemCount`und `UnreadItemCount` Elemente in einem e-Mail-Ordner unabhängig von deren Elementtypen einschließen.</span><span class="sxs-lookup"><span data-stu-id="6f16d-226">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="6f16d-227">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6f16d-227">Relationships</span></span>

| <span data-ttu-id="6f16d-228">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6f16d-228">Relationship</span></span> | <span data-ttu-id="6f16d-229">Typ</span><span class="sxs-lookup"><span data-stu-id="6f16d-229">Type</span></span> | <span data-ttu-id="6f16d-230">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f16d-230">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="6f16d-231">childFolders</span><span class="sxs-lookup"><span data-stu-id="6f16d-231">childFolders</span></span>|<span data-ttu-id="6f16d-232">[MailFolder](mailfolder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f16d-232">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="6f16d-233">Die Sammlung der untergeordneten Ordner in dem mailFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6f16d-233">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="6f16d-234">messageRules</span><span class="sxs-lookup"><span data-stu-id="6f16d-234">messageRules</span></span> | <span data-ttu-id="6f16d-235">[messageRule](messagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f16d-235">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="6f16d-236">Die Sammlung von Regeln, die für den Posteingangsordner des Benutzers gelten.</span><span class="sxs-lookup"><span data-stu-id="6f16d-236">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="6f16d-237">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="6f16d-237">messages</span></span>|<span data-ttu-id="6f16d-238">[Nachrichten](message.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f16d-238">[Message](message.md) collection</span></span>|<span data-ttu-id="6f16d-239">Die Sammlung der Nachrichten in dem mailFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6f16d-239">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="6f16d-240">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="6f16d-240">multiValueExtendedProperties</span></span>|<span data-ttu-id="6f16d-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f16d-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6f16d-p110">Die Sammlung erweiterter mehrwertiger Eigenschaften, die für das mailFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6f16d-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6f16d-245">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="6f16d-245">singleValueExtendedProperties</span></span>|<span data-ttu-id="6f16d-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f16d-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6f16d-p111">Die Sammlung erweiterter einwertiger Eigenschaften, die für das mailFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6f16d-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f16d-250">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6f16d-250">JSON representation</span></span>

<span data-ttu-id="6f16d-251">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6f16d-251">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="6f16d-252">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6f16d-252">See also</span></span>

- [<span data-ttu-id="6f16d-253">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="6f16d-253">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="6f16d-254">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="6f16d-254">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
