---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FileSystemInfo
localization_priority: Normal
ms.openlocfilehash: 65bbd2e371c856a6ffbd2c55ecba88c1635ce41c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480285"
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="33c33-102">FileSystemInfo-Facet</span><span class="sxs-lookup"><span data-stu-id="33c33-102">FileSystemInfo facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33c33-p101">Die Ressource **FileSystemInfo** enthält Eigenschaften, die vom lokalen Dateisystem des Geräts für die lokale Version eines Elements gemeldet werden. Diese Facet kann zum Angeben des letzten Änderungsdatums oder des Erstellungsdatums des Elements verwendet werden, wie es auf dem lokalen Gerät gespeichert war.</span><span class="sxs-lookup"><span data-stu-id="33c33-p101">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="33c33-105">Das Facet ist verfügbar für die Eigenschaft „fileSystemInfo“ von Ressourcen des Typs [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="33c33-105">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="33c33-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="33c33-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="33c33-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="33c33-107">Properties</span></span>

| <span data-ttu-id="33c33-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33c33-108">Property</span></span>                 | <span data-ttu-id="33c33-109">Typ</span><span class="sxs-lookup"><span data-stu-id="33c33-109">Type</span></span>           | <span data-ttu-id="33c33-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33c33-110">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="33c33-111">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="33c33-111">**createdDateTime**</span></span>      | <span data-ttu-id="33c33-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33c33-112">DateTimeOffset</span></span> | <span data-ttu-id="33c33-113">Das UTC-Datum und die UTC-Uhrzeit der Erstellung der Datei auf einem Client.</span><span class="sxs-lookup"><span data-stu-id="33c33-113">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="33c33-114">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="33c33-114">**lastAccessedDateTime**</span></span> | <span data-ttu-id="33c33-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33c33-115">DateTimeOffset</span></span> | <span data-ttu-id="33c33-116">Das UTC-Datum und die UTC-Uhrzeit des letzten Zugriffs auf die Datei.</span><span class="sxs-lookup"><span data-stu-id="33c33-116">The UTC date and time the file was last accessed.</span></span> <span data-ttu-id="33c33-117">Nur für die [Liste der zuletzt verwendeten Dateien](../api/drive-recent.md) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="33c33-117">Available for the [recent file list](../api/drive-recent.md) only.</span></span> |
| <span data-ttu-id="33c33-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="33c33-118">**lastModifiedDateTime**</span></span> | <span data-ttu-id="33c33-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33c33-119">DateTimeOffset</span></span> | <span data-ttu-id="33c33-120">Das UTC-Datum und die UTC-Uhrzeit der letzten Änderung der Datei auf einem Client.</span><span class="sxs-lookup"><span data-stu-id="33c33-120">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="33c33-121">Anmerkungen</span><span class="sxs-lookup"><span data-stu-id="33c33-121">Notes</span></span>

<span data-ttu-id="33c33-p103">Werte für **createdDateTime** und **lastModifiedDateTime** unterscheiden sich von den gleichen Eigenschaften auf der Ressource [DriveItem](driveitem.md). Die Werte für die Ressource DriveItem sind Erstellungsdatum und -uhrzeit, wie sie vom Dienst erfasst werden. Die in der Ressource **FileSystemInfo** gespeicherten Werte werden vom Client bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="33c33-p103">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource. The values on the DriveItem resource are the created and modified date and time as seen from the service. The values stored in the **FileSystemInfo** resource are provided by the client.</span></span>

<span data-ttu-id="33c33-p104">Beispiel: Wenn eine Datei am Montag auf dem Gerät erstellt wurde, aber erst am Dienstag in den Dienst hochgeladen wurde, muss der Client, der die Datei hochlädt, die Facet `fileSystemInfo` schreiben, um das Erstellungsdatum am Montag einzubeziehen. Wenn die Metadaten des Elements abgerufen werden, wird als Erstellungsdatum für das Element Dienstag angegeben. Die Facet `fileSystemInfo` zeigt jedoch das ursprüngliche Erstellungsdatum am Montag an.</span><span class="sxs-lookup"><span data-stu-id="33c33-p104">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="33c33-p105">Diese Eigenschaften sind lese- und schreibgeschützt. Wenn Sie eine Datei hochladen und die lokalen Client-Werte für diese Felder kennen, sollten Sie diese bei der Anfrage einbeziehen.</span><span class="sxs-lookup"><span data-stu-id="33c33-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="33c33-129">Wenn der Inhalt der Datei aktualisiert wird und diese Eigenschaften nicht angegeben werden, wird **lastModifiedDateTime** automatisch auf die aktuelle Uhrzeit zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="33c33-129">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="33c33-130">Hinweise</span><span class="sxs-lookup"><span data-stu-id="33c33-130">Remarks</span></span>

* <span data-ttu-id="33c33-131">**lastAccessedDateTime** ist für Elemente in SharePoint Online oder OneDrive for Business nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="33c33-131">**lastAccessedDateTime** is not available for items in SharePoint online or OneDrive for Business.</span></span>

<span data-ttu-id="33c33-132">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="33c33-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo",
  "suppressions": [
    "Error: /api-reference/beta/resources/filesysteminfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
