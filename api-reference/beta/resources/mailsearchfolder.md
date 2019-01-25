---
title: Ressourcentyp mailSearchFolder
description: Ein MailSearchFolder ist ein virtueller Ordner im Postfach des Benutzers, das alle angegebenen Suchkriterien e-Mail-Elemente enthält. MailSearchFolder erbt vom MailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba76029b69d91be39c9d63ca755e8a4603aec0b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520984"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="26ea1-104">Ressourcentyp mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="26ea1-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26ea1-105">Ein MailSearchFolder ist ein virtueller Ordner im Postfach des Benutzers, das alle angegebenen Suchkriterien e-Mail-Elemente enthält.</span><span class="sxs-lookup"><span data-stu-id="26ea1-105">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="26ea1-106">MailSearchFolder erbt vom [MailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="26ea1-106">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="26ea1-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="26ea1-107">Methods</span></span>

| <span data-ttu-id="26ea1-108">Methode</span><span class="sxs-lookup"><span data-stu-id="26ea1-108">Method</span></span> | <span data-ttu-id="26ea1-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="26ea1-109">Return Type</span></span>  | <span data-ttu-id="26ea1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26ea1-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="26ea1-111">Erstellen eines Suchordners</span><span class="sxs-lookup"><span data-stu-id="26ea1-111">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="26ea1-112">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="26ea1-112">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="26ea1-113">Erstellen eines Suchordners im Postfach des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="26ea1-113">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="26ea1-114">Liste Suchordner</span><span class="sxs-lookup"><span data-stu-id="26ea1-114">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="26ea1-115">[mailFolder](mailfolder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="26ea1-115">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="26ea1-116">Listen Sie alle Ordner im Postfach dieses Benutzers, einschließlich Suchordner.</span><span class="sxs-lookup"><span data-stu-id="26ea1-116">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="26ea1-117">Abrufen von Ordnern suchen</span><span class="sxs-lookup"><span data-stu-id="26ea1-117">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="26ea1-118">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="26ea1-118">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="26ea1-119">Rufen Sie den angegebenen Suchordner.</span><span class="sxs-lookup"><span data-stu-id="26ea1-119">Get the specified search folder.</span></span> |
| [<span data-ttu-id="26ea1-120">Aktualisieren eines Suchordners</span><span class="sxs-lookup"><span data-stu-id="26ea1-120">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="26ea1-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="26ea1-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="26ea1-122">Aktualisieren Sie den angegebenen Suchordner.</span><span class="sxs-lookup"><span data-stu-id="26ea1-122">Update the specified search folder.</span></span> |
| [<span data-ttu-id="26ea1-123">Löschen eines Suchordners</span><span class="sxs-lookup"><span data-stu-id="26ea1-123">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="26ea1-124">Keine</span><span class="sxs-lookup"><span data-stu-id="26ea1-124">None</span></span> | <span data-ttu-id="26ea1-125">Löschen Sie den angegebenen Suchordner.</span><span class="sxs-lookup"><span data-stu-id="26ea1-125">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="26ea1-126">Listen Sie alle Nachrichten in einem Suchordner</span><span class="sxs-lookup"><span data-stu-id="26ea1-126">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="26ea1-127">[message](message.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="26ea1-127">[message](message.md) collection</span></span> | <span data-ttu-id="26ea1-128">Listen Sie alle Nachrichten in den angegebenen Suchordner.</span><span class="sxs-lookup"><span data-stu-id="26ea1-128">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="26ea1-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="26ea1-129">Properties</span></span>

| <span data-ttu-id="26ea1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26ea1-130">Property</span></span> | <span data-ttu-id="26ea1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="26ea1-131">Type</span></span> | <span data-ttu-id="26ea1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26ea1-132">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="26ea1-133">isSupported</span><span class="sxs-lookup"><span data-stu-id="26ea1-133">isSupported</span></span> | <span data-ttu-id="26ea1-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="26ea1-134">Boolean</span></span> | <span data-ttu-id="26ea1-135">Gibt an, ob ein Suchordner mithilfe von REST-APIs bearbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="26ea1-135">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="26ea1-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="26ea1-136">includeNestedFolders</span></span> | <span data-ttu-id="26ea1-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="26ea1-137">Boolean</span></span> | <span data-ttu-id="26ea1-138">Gibt an, wie die Hierarchie der Postfach-Ordner durchlaufen werden soll.</span><span class="sxs-lookup"><span data-stu-id="26ea1-138">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="26ea1-139">`true`bedeutet, dass eine umfassende Suche sollte erledigen `false` bedeutet, dass eine flache Suche sollte stattdessen durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="26ea1-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="26ea1-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="26ea1-140">sourceFolderIDs</span></span> | <span data-ttu-id="26ea1-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="26ea1-141">String collection</span></span> | <span data-ttu-id="26ea1-142">Die Postfachordner, die durchsucht werden soll.</span><span class="sxs-lookup"><span data-stu-id="26ea1-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="26ea1-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="26ea1-143">filterQuery</span></span> | <span data-ttu-id="26ea1-144">String</span><span class="sxs-lookup"><span data-stu-id="26ea1-144">String</span></span> | <span data-ttu-id="26ea1-145">Der OData-Abfrage Nachrichten gefiltert werden soll.</span><span class="sxs-lookup"><span data-stu-id="26ea1-145">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26ea1-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="26ea1-146">JSON representation</span></span>

<span data-ttu-id="26ea1-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="26ea1-147">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailsearchfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
