---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: fileSystemInfo
ms.openlocfilehash: 2a2e31754e64d18f8fce873212d7c582e6611e60
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019043"
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="ec08c-102">FileSystemInfo-Facet</span><span class="sxs-lookup"><span data-stu-id="ec08c-102">FileSystemInfo facet</span></span>

<span data-ttu-id="ec08c-p101">Die Ressource **FileSystemInfo** enthält Eigenschaften, die vom lokalen Dateisystem des Geräts für die lokale Version eines Elements gemeldet werden. Diese Facet kann zum Angeben des letzten Änderungsdatums oder des Erstellungsdatums des Elements verwendet werden, wie es auf dem lokalen Gerät gespeichert war.</span><span class="sxs-lookup"><span data-stu-id="ec08c-p101">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="ec08c-105">Das Facet ist verfügbar für die Eigenschaft „fileSystemInfo“ von Ressourcen des Typs [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="ec08c-105">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec08c-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ec08c-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime" : "datetime",
  "lastAccessedDateTime": "datetime",
  "lastModifiedDateTime" : "datetime"
}
```

## <a name="properties"></a><span data-ttu-id="ec08c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ec08c-107">Properties</span></span>

| <span data-ttu-id="ec08c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec08c-108">Property</span></span>                 | <span data-ttu-id="ec08c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ec08c-109">Type</span></span>           | <span data-ttu-id="ec08c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec08c-110">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ec08c-111">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ec08c-111">**createdDateTime**</span></span>      | <span data-ttu-id="ec08c-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec08c-112">DateTimeOffset</span></span> | <span data-ttu-id="ec08c-113">Das UTC-Datum und die UTC-Uhrzeit der Erstellung der Datei auf einem Client.</span><span class="sxs-lookup"><span data-stu-id="ec08c-113">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="ec08c-114">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ec08c-114">**lastAccessedDateTime**</span></span> | <span data-ttu-id="ec08c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec08c-115">DateTimeOffset</span></span> | <span data-ttu-id="ec08c-p102">Das UTC-Datum und die UTC-Uhrzeit des letzten Zugriffs auf die Datei. Nur für die [Liste der zuletzt verwendeten Dateien](../api/drive-recent.md) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ec08c-p102">The UTC date and time the file was last accessed. Available for the [recent file list](../api/drive-recent.md) only.</span></span> |
| <span data-ttu-id="ec08c-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ec08c-118">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ec08c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec08c-119">DateTimeOffset</span></span> | <span data-ttu-id="ec08c-120">Das UTC-Datum und die UTC-Uhrzeit der letzten Änderung der Datei auf einem Client.</span><span class="sxs-lookup"><span data-stu-id="ec08c-120">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="ec08c-121">Anmerkungen</span><span class="sxs-lookup"><span data-stu-id="ec08c-121">Notes</span></span>

<span data-ttu-id="ec08c-p103">Werte für **createdDateTime** und **lastModifiedDateTime** unterscheiden sich von den gleichen Eigenschaften auf der Ressource [DriveItem](driveitem.md). Die Werte für die Ressource DriveItem sind Erstellungsdatum und -uhrzeit, wie sie vom Dienst erfasst werden. Die in der Ressource **FileSystemInfo** gespeicherten Werte werden vom Client bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="ec08c-p103">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource. The values on the DriveItem resource are the created and modified date and time as seen from the service. The values stored in the **FileSystemInfo** resource are provided by the client.</span></span>

<span data-ttu-id="ec08c-p104">Beispiel: Wenn eine Datei am Montag auf dem Gerät erstellt wurde, aber erst am Dienstag in den Dienst hochgeladen wurde, muss der Client, der die Datei hochlädt, die Facet `fileSystemInfo` schreiben, um das Erstellungsdatum am Montag einzubeziehen. Wenn die Metadaten des Elements abgerufen werden, wird als Erstellungsdatum für das Element Dienstag angegeben. Die Facet `fileSystemInfo` zeigt jedoch das ursprüngliche Erstellungsdatum am Montag an.</span><span class="sxs-lookup"><span data-stu-id="ec08c-p104">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="ec08c-p105">Diese Eigenschaften sind lese- und schreibgeschützt. Wenn Sie eine Datei hochladen und die lokalen Client-Werte für diese Felder kennen, sollten Sie diese bei der Anfrage einbeziehen.</span><span class="sxs-lookup"><span data-stu-id="ec08c-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="ec08c-129">Wenn der Inhalt der Datei aktualisiert wird und diese Eigenschaften nicht angegeben werden, wird **lastModifiedDateTime** automatisch auf die aktuelle Uhrzeit zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="ec08c-129">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="ec08c-130">Hinweise</span><span class="sxs-lookup"><span data-stu-id="ec08c-130">Remarks</span></span>

* <span data-ttu-id="ec08c-131">**lastAccessedDateTime** ist für Elemente in SharePoint Online oder OneDrive for Business nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ec08c-131">**lastAccessedDateTime** is not available for items in SharePoint online or OneDrive for Business.</span></span>

<span data-ttu-id="ec08c-132">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ec08c-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
