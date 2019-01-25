---
title: Ressourcentyp educationFileResource
description: Eine Unterklasse der EducationResource, die ein File-Objekt darstellt, die die Zuordnung oder die Übermittlung zugeordnet ist.  In diesem Fall wird die Datei ist nicht die speziellen Dateien (Word, Excel usw.), jedoch ist eine Datei, die keine besondere Behandlung innerhalb des Systems verfügt. File-Ressource muss in der **Ressourcefolder** gespeichert werden, die die Zuordnung oder die Übermittlung, diese Ressource zugeordnet ist, zugeordnet ist.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 15ca31576618f15e64b85d860077785160c25989
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520795"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="a8f03-105">Ressourcentyp educationFileResource</span><span class="sxs-lookup"><span data-stu-id="a8f03-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8f03-106">Eine Unterklasse der [EducationResource](educationresource.md) , die ein File-Objekt darstellt, die die Zuordnung oder die Übermittlung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="a8f03-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="a8f03-107">In diesem Fall wird die Datei ist nicht die speziellen Dateien (Word, Excel usw.), jedoch ist eine Datei, die keine besondere Behandlung innerhalb des Systems verfügt.</span><span class="sxs-lookup"><span data-stu-id="a8f03-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="a8f03-108">File-Ressource muss in der **Ressourcefolder** gespeichert werden, die die Zuordnung oder die Übermittlung, diese Ressource zugeordnet ist, zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="a8f03-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="a8f03-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8f03-109">Properties</span></span>
| <span data-ttu-id="a8f03-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8f03-110">Property</span></span>     | <span data-ttu-id="a8f03-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a8f03-111">Type</span></span>   |<span data-ttu-id="a8f03-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8f03-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8f03-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="a8f03-113">fileUrl</span></span>|<span data-ttu-id="a8f03-114">String</span><span class="sxs-lookup"><span data-stu-id="a8f03-114">String</span></span>|<span data-ttu-id="a8f03-115">Speicherort auf dem Datenträger den File-Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8f03-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8f03-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8f03-116">JSON representation</span></span>

<span data-ttu-id="a8f03-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8f03-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfileresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
