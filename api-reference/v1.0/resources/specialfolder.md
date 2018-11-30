---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SpecialFolder
ms.openlocfilehash: bbf12aa0bf127116fd5f1250717c19f3f053f751
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27015971"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="1a853-102">SpecialFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1a853-102">SpecialFolder resource type</span></span>

<span data-ttu-id="1a853-103">Die **SpecialFolder**-Ressource gruppiert ordnerbezogene Datenelement in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="1a853-103">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="1a853-104">Wenn ein **DriveItem** über ein **specialFolder**-Facet ungleich Null verfügt, stellt das Element einen speziellen (benannten) Ordner dar.</span><span class="sxs-lookup"><span data-stu-id="1a853-104">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="1a853-105">Auf spezielle Ordner können Sie direkt über die [Sammlung spezieller Ordner](../api/drive-get-specialfolder.md) zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1a853-105">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="1a853-p102">Spezielle Ordner bieten einfache Aliase für den Zugriff auf bekannte Ordner, ohne dass der Ordner anhand des Pfads nachgeschlagen werden muss (wofür eine Lokalisierung erforderlich wäre) oder anhand einer ID auf den Ordner verwiesen werden muss. Wenn ein spezieller Ordner umbenannt oder an eine andere Position innerhalb des Laufwerks verschoben wird, kann mit dieser Syntax weiterhin dieser Ordner zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="1a853-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="1a853-p103">Spezielle Ordner werden automatisch erstellt, wenn eine Anwendung das erste Mal versucht, einen Ordner zu schreiben, wenn noch keiner vorhanden ist. Wenn ein Benutzer einen speziellen Ordner löscht, wird dieser neu erstellt, wenn erneut in den Ordner geschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="1a853-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="1a853-110">**Hinweis:** Wenn Ihre App nur den **Files.Read**-Bereich angefordert hat und einen speziellen Ordner anfordert, der nicht vorhanden ist, wird als Antwort der Fehler `403 Forbidden` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a853-110">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a853-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1a853-111">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="1a853-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1a853-112">Properties</span></span>

| <span data-ttu-id="1a853-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a853-113">Property</span></span>  | <span data-ttu-id="1a853-114">Typ</span><span class="sxs-lookup"><span data-stu-id="1a853-114">Type</span></span>   | <span data-ttu-id="1a853-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a853-115">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="1a853-116">name</span><span class="sxs-lookup"><span data-stu-id="1a853-116">name</span></span>      | <span data-ttu-id="1a853-117">string</span><span class="sxs-lookup"><span data-stu-id="1a853-117">string</span></span> | <span data-ttu-id="1a853-118">Der eindeutige Bezeichner für dieses Element in der `/drive/special`-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1a853-118">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="1a853-119">Spezielle Ordner</span><span class="sxs-lookup"><span data-stu-id="1a853-119">Special folders</span></span>

<span data-ttu-id="1a853-120">Im Folgenden sind spezielle Ordner aufgelistet, die in OneDrive Personal und OneDrive for Business zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="1a853-120">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="1a853-121">Name</span><span class="sxs-lookup"><span data-stu-id="1a853-121">Name</span></span>        | <span data-ttu-id="1a853-122">Ordner-ID</span><span class="sxs-lookup"><span data-stu-id="1a853-122">Folder id</span></span>    | <span data-ttu-id="1a853-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a853-123">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="1a853-124">Anwendungsstamm</span><span class="sxs-lookup"><span data-stu-id="1a853-124">App Root</span></span>    | `approot`    | <span data-ttu-id="1a853-p104">Der persönliche Ordner der Anwendung. In der Regel unter `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="1a853-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="1a853-127">Eigene Aufnahmen</span><span class="sxs-lookup"><span data-stu-id="1a853-127">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="1a853-p105">Der Sicherungsordner für Eigene Aufnahmen. In OneDrive for Business nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="1a853-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="1a853-130">Dokumente</span><span class="sxs-lookup"><span data-stu-id="1a853-130">Documents</span></span>   | `documents`  | <span data-ttu-id="1a853-131">Der Ordner „Dokumente“.</span><span class="sxs-lookup"><span data-stu-id="1a853-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="1a853-132">Musik</span><span class="sxs-lookup"><span data-stu-id="1a853-132">Music</span></span>       | `music`      | <span data-ttu-id="1a853-p106">Der Ordner „Musik“. In OneDrive for Business nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="1a853-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="1a853-135">Fotos</span><span class="sxs-lookup"><span data-stu-id="1a853-135">Photos</span></span>      | `photos`     | <span data-ttu-id="1a853-136">Der Ordner „Fotos“.</span><span class="sxs-lookup"><span data-stu-id="1a853-136">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="1a853-137">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="1a853-137">Remarks</span></span> 

<span data-ttu-id="1a853-138">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1a853-138">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->
