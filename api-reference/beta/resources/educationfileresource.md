---
title: Ressourcentyp educationFileResource
description: Eine Unterklasse der EducationResource, die ein File-Objekt darstellt, die die Zuordnung oder die Übermittlung zugeordnet ist.  In diesem Fall wird die Datei ist nicht die speziellen Dateien (Word, Excel usw.), jedoch ist eine Datei, die keine besondere Behandlung innerhalb des Systems verfügt. File-Ressource muss in der **Ressourcefolder** gespeichert werden, die die Zuordnung oder die Übermittlung, diese Ressource zugeordnet ist, zugeordnet ist.
ms.openlocfilehash: b3ba77b6b9243d987ad1137afe6d2206e47dadaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062217"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="f7ff2-105">Ressourcentyp educationFileResource</span><span class="sxs-lookup"><span data-stu-id="f7ff2-105">educationFileResource resource type</span></span>

> <span data-ttu-id="f7ff2-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7ff2-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7ff2-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7ff2-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7ff2-108">Eine Unterklasse der [EducationResource](educationresource.md) , die ein File-Objekt darstellt, die die Zuordnung oder die Übermittlung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="f7ff2-108">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="f7ff2-109">In diesem Fall wird die Datei ist nicht die speziellen Dateien (Word, Excel usw.), jedoch ist eine Datei, die keine besondere Behandlung innerhalb des Systems verfügt.</span><span class="sxs-lookup"><span data-stu-id="f7ff2-109">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="f7ff2-110">File-Ressource muss in der **Ressourcefolder** gespeichert werden, die die Zuordnung oder die Übermittlung, diese Ressource zugeordnet ist, zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="f7ff2-110">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="f7ff2-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7ff2-111">Properties</span></span>
| <span data-ttu-id="f7ff2-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7ff2-112">Property</span></span>     | <span data-ttu-id="f7ff2-113">Typ</span><span class="sxs-lookup"><span data-stu-id="f7ff2-113">Type</span></span>   |<span data-ttu-id="f7ff2-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7ff2-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7ff2-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="f7ff2-115">fileUrl</span></span>|<span data-ttu-id="f7ff2-116">String</span><span class="sxs-lookup"><span data-stu-id="f7ff2-116">String</span></span>|<span data-ttu-id="f7ff2-117">Speicherort auf dem Datenträger den File-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7ff2-117">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7ff2-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7ff2-118">JSON representation</span></span>

<span data-ttu-id="f7ff2-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7ff2-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->