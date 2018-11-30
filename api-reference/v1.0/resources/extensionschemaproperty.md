---
title: extensionSchemaProperty-Ressourcentyp
description: Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer schemaExtension-Definition zu definieren.
ms.openlocfilehash: 1ea2fca1812765aab49d548dd3cd3ed0575e30aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016664"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="30f8b-103">extensionSchemaProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="30f8b-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="30f8b-104">Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer [schemaExtension](schemaextension.md)-Definition zu definieren.</span><span class="sxs-lookup"><span data-stu-id="30f8b-104">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="30f8b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="30f8b-105">Properties</span></span>
| <span data-ttu-id="30f8b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30f8b-106">Property</span></span>     | <span data-ttu-id="30f8b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="30f8b-107">Type</span></span>   |<span data-ttu-id="30f8b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30f8b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30f8b-109">name</span><span class="sxs-lookup"><span data-stu-id="30f8b-109">name</span></span>|<span data-ttu-id="30f8b-110">String</span><span class="sxs-lookup"><span data-stu-id="30f8b-110">String</span></span>| <span data-ttu-id="30f8b-111">Der Name der stark typisierten Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.</span><span class="sxs-lookup"><span data-stu-id="30f8b-111">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="30f8b-112">type</span><span class="sxs-lookup"><span data-stu-id="30f8b-112">type</span></span>|<span data-ttu-id="30f8b-113">String</span><span class="sxs-lookup"><span data-stu-id="30f8b-113">String</span></span>| <span data-ttu-id="30f8b-p101">Der Typ der Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.  Zulässige Werte sind *Binary, Boolean, DateTime, Integer* oder *String*.  Weitere Einzelheiten finden Sie in der Tabelle unten.</span><span class="sxs-lookup"><span data-stu-id="30f8b-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="30f8b-117">Unterstützte Datentypen für Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="30f8b-117">Supported property data types</span></span> 
<span data-ttu-id="30f8b-118">Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:</span><span class="sxs-lookup"><span data-stu-id="30f8b-118">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="30f8b-119">Eigenschaftentyp</span><span class="sxs-lookup"><span data-stu-id="30f8b-119">Property Type</span></span> | <span data-ttu-id="30f8b-120">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="30f8b-120">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="30f8b-121">Binär</span><span class="sxs-lookup"><span data-stu-id="30f8b-121">Binary</span></span> | <span data-ttu-id="30f8b-122">Maximal 256 Bytes.</span><span class="sxs-lookup"><span data-stu-id="30f8b-122">256 bytes maximum.</span></span> |
| <span data-ttu-id="30f8b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f8b-123">Boolean</span></span> | <span data-ttu-id="30f8b-124">Nicht unterstützt für Kontakte, Nachrichten, Ereignisse und Beiträge.</span><span class="sxs-lookup"><span data-stu-id="30f8b-124">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="30f8b-125">DateTime</span><span class="sxs-lookup"><span data-stu-id="30f8b-125">DateTime</span></span> | <span data-ttu-id="30f8b-p102">Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert.</span><span class="sxs-lookup"><span data-stu-id="30f8b-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="30f8b-128">Ganze Zahl</span><span class="sxs-lookup"><span data-stu-id="30f8b-128">Integer</span></span> | <span data-ttu-id="30f8b-129">32-Bit-Wert.</span><span class="sxs-lookup"><span data-stu-id="30f8b-129">32-bit value.</span></span> <span data-ttu-id="30f8b-130">Nicht unterstützt für Kontakte, Nachrichten, Ereignisse und Beiträge.</span><span class="sxs-lookup"><span data-stu-id="30f8b-130">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="30f8b-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="30f8b-131">String</span></span> | <span data-ttu-id="30f8b-132">Maximal 256 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="30f8b-132">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="30f8b-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="30f8b-133">JSON representation</span></span>
<span data-ttu-id="30f8b-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="30f8b-134">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
