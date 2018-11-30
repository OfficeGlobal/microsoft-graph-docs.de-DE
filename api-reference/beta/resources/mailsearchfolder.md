---
title: Ressourcentyp mailSearchFolder
description: Ein MailSearchFolder ist ein virtueller Ordner im Postfach des Benutzers, das alle angegebenen Suchkriterien e-Mail-Elemente enthält. MailSearchFolder erbt vom MailFolder.
ms.openlocfilehash: abce7c86e44fcee98042aecf753f0fdf4172365e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063208"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="cecf4-104">Ressourcentyp mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="cecf4-104">mailSearchFolder resource type</span></span>

> <span data-ttu-id="cecf4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cecf4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cecf4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cecf4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cecf4-107">Ein MailSearchFolder ist ein virtueller Ordner im Postfach des Benutzers, das alle angegebenen Suchkriterien e-Mail-Elemente enthält.</span><span class="sxs-lookup"><span data-stu-id="cecf4-107">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="cecf4-108">MailSearchFolder erbt vom [MailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="cecf4-108">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cecf4-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="cecf4-109">Methods</span></span>

| <span data-ttu-id="cecf4-110">Methode</span><span class="sxs-lookup"><span data-stu-id="cecf4-110">Method</span></span> | <span data-ttu-id="cecf4-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cecf4-111">Return Type</span></span>  | <span data-ttu-id="cecf4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cecf4-112">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="cecf4-113">Erstellen eines Suchordners</span><span class="sxs-lookup"><span data-stu-id="cecf4-113">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="cecf4-114">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="cecf4-114">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="cecf4-115">Erstellen eines Suchordners im Postfach des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="cecf4-115">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="cecf4-116">Liste Suchordner</span><span class="sxs-lookup"><span data-stu-id="cecf4-116">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="cecf4-117">[mailFolder](mailfolder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cecf4-117">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="cecf4-118">Listen Sie alle Ordner im Postfach dieses Benutzers, einschließlich Suchordner.</span><span class="sxs-lookup"><span data-stu-id="cecf4-118">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="cecf4-119">Abrufen von Ordnern suchen</span><span class="sxs-lookup"><span data-stu-id="cecf4-119">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="cecf4-120">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="cecf4-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="cecf4-121">Rufen Sie den angegebenen Suchordner.</span><span class="sxs-lookup"><span data-stu-id="cecf4-121">Get the specified search folder.</span></span> |
| [<span data-ttu-id="cecf4-122">Aktualisieren eines Suchordners</span><span class="sxs-lookup"><span data-stu-id="cecf4-122">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="cecf4-123">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="cecf4-123">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="cecf4-124">Aktualisieren Sie den angegebenen Suchordner.</span><span class="sxs-lookup"><span data-stu-id="cecf4-124">Update the specified search folder.</span></span> |
| [<span data-ttu-id="cecf4-125">Löschen eines Suchordners</span><span class="sxs-lookup"><span data-stu-id="cecf4-125">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="cecf4-126">Keines</span><span class="sxs-lookup"><span data-stu-id="cecf4-126">None</span></span> | <span data-ttu-id="cecf4-127">Löschen Sie den angegebenen Suchordner.</span><span class="sxs-lookup"><span data-stu-id="cecf4-127">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="cecf4-128">Listen Sie alle Nachrichten in einem Suchordner</span><span class="sxs-lookup"><span data-stu-id="cecf4-128">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="cecf4-129">[message](message.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cecf4-129">[message](message.md) collection</span></span> | <span data-ttu-id="cecf4-130">Listen Sie alle Nachrichten in den angegebenen Suchordner.</span><span class="sxs-lookup"><span data-stu-id="cecf4-130">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="cecf4-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cecf4-131">Properties</span></span>

| <span data-ttu-id="cecf4-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cecf4-132">Property</span></span> | <span data-ttu-id="cecf4-133">Typ</span><span class="sxs-lookup"><span data-stu-id="cecf4-133">Type</span></span> | <span data-ttu-id="cecf4-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cecf4-134">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="cecf4-135">isSupported</span><span class="sxs-lookup"><span data-stu-id="cecf4-135">isSupported</span></span> | <span data-ttu-id="cecf4-136">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cecf4-136">Boolean</span></span> | <span data-ttu-id="cecf4-137">Gibt an, ob ein Suchordner mithilfe von REST-APIs bearbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="cecf4-137">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="cecf4-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="cecf4-138">includeNestedFolders</span></span> | <span data-ttu-id="cecf4-139">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cecf4-139">Boolean</span></span> | <span data-ttu-id="cecf4-140">Gibt an, wie die Hierarchie der Postfach-Ordner durchlaufen werden soll.</span><span class="sxs-lookup"><span data-stu-id="cecf4-140">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="cecf4-141">`true`bedeutet, dass eine umfassende Suche sollte erledigen `false` bedeutet, dass eine flache Suche sollte stattdessen durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="cecf4-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="cecf4-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="cecf4-142">sourceFolderIDs</span></span> | <span data-ttu-id="cecf4-143">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="cecf4-143">String collection</span></span> | <span data-ttu-id="cecf4-144">Die Postfachordner, die durchsucht werden soll.</span><span class="sxs-lookup"><span data-stu-id="cecf4-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="cecf4-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="cecf4-145">filterQuery</span></span> | <span data-ttu-id="cecf4-146">String</span><span class="sxs-lookup"><span data-stu-id="cecf4-146">String</span></span> | <span data-ttu-id="cecf4-147">Der OData-Abfrage Nachrichten gefiltert werden soll.</span><span class="sxs-lookup"><span data-stu-id="cecf4-147">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cecf4-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cecf4-148">JSON representation</span></span>

<span data-ttu-id="cecf4-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cecf4-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
