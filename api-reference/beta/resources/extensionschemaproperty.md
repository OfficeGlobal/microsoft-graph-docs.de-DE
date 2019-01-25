---
title: extensionSchemaProperty-Ressourcentyp
description: Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer schemaExtension-Definition zu definieren.
localization_priority: Normal
ms.openlocfilehash: bb044aa2f85ea5accdba4ed43a1a5b1c856a209d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511506"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="b214c-103">extensionSchemaProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b214c-103">extensionSchemaProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b214c-104">Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer [schemaExtension](schemaextension.md)-Definition zu definieren.</span><span class="sxs-lookup"><span data-stu-id="b214c-104">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="b214c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b214c-105">Properties</span></span>
| <span data-ttu-id="b214c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b214c-106">Property</span></span>     | <span data-ttu-id="b214c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b214c-107">Type</span></span>   |<span data-ttu-id="b214c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b214c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b214c-109">name</span><span class="sxs-lookup"><span data-stu-id="b214c-109">name</span></span>|<span data-ttu-id="b214c-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b214c-110">String</span></span>| <span data-ttu-id="b214c-111">Der Name der stark typisierten-Eigenschaft als Teil einer schemaerweiterung definiert.</span><span class="sxs-lookup"><span data-stu-id="b214c-111">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="b214c-112">type</span><span class="sxs-lookup"><span data-stu-id="b214c-112">type</span></span>|<span data-ttu-id="b214c-113">String</span><span class="sxs-lookup"><span data-stu-id="b214c-113">String</span></span>| <span data-ttu-id="b214c-p101">Der Typ der Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.  Zulässige Werte sind *Binary, Boolean, DateTime, Integer* oder *String*.  Weitere Einzelheiten finden Sie in der Tabelle unten.</span><span class="sxs-lookup"><span data-stu-id="b214c-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="b214c-117">Unterstützte Datentypen für Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b214c-117">Supported property data types</span></span> 
<span data-ttu-id="b214c-118">Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b214c-118">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="b214c-119">Eigenschaftentyp</span><span class="sxs-lookup"><span data-stu-id="b214c-119">Property Type</span></span> | <span data-ttu-id="b214c-120">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="b214c-120">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="b214c-121">Binär</span><span class="sxs-lookup"><span data-stu-id="b214c-121">Binary</span></span> | <span data-ttu-id="b214c-122">Maximal 256 Bytes.</span><span class="sxs-lookup"><span data-stu-id="b214c-122">256 bytes maximum.</span></span> |
| <span data-ttu-id="b214c-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b214c-123">Boolean</span></span> | <span data-ttu-id="b214c-124">Nicht unterstützt für Nachrichten, Ereignisse und Beiträge.</span><span class="sxs-lookup"><span data-stu-id="b214c-124">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="b214c-125">DateTime</span><span class="sxs-lookup"><span data-stu-id="b214c-125">DateTime</span></span> | <span data-ttu-id="b214c-p102">Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert.</span><span class="sxs-lookup"><span data-stu-id="b214c-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="b214c-128">Ganze Zahl</span><span class="sxs-lookup"><span data-stu-id="b214c-128">Integer</span></span> | <span data-ttu-id="b214c-p103">32-Bit-Wert. Nicht unterstützt für Nachrichten, Ereignisse und Beiträge.</span><span class="sxs-lookup"><span data-stu-id="b214c-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="b214c-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b214c-131">String</span></span> | <span data-ttu-id="b214c-132">Maximal 256 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="b214c-132">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b214c-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b214c-133">JSON representation</span></span>
<span data-ttu-id="b214c-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b214c-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/extensionschemaproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
