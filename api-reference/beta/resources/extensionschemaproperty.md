---
title: extensionSchemaProperty-Ressourcentyp
description: Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer schemaExtension-Definition zu definieren.
ms.openlocfilehash: f699ccebefc849a7bf9cacc6dbda61cbcbb9896d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059760"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="811d1-103">extensionSchemaProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="811d1-103">extensionSchemaProperty resource type</span></span>

> <span data-ttu-id="811d1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="811d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="811d1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="811d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="811d1-106">Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer [schemaExtension](schemaextension.md)-Definition zu definieren.</span><span class="sxs-lookup"><span data-stu-id="811d1-106">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="811d1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="811d1-107">Properties</span></span>
| <span data-ttu-id="811d1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="811d1-108">Property</span></span>     | <span data-ttu-id="811d1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="811d1-109">Type</span></span>   |<span data-ttu-id="811d1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="811d1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="811d1-111">name</span><span class="sxs-lookup"><span data-stu-id="811d1-111">name</span></span>|<span data-ttu-id="811d1-112">String</span><span class="sxs-lookup"><span data-stu-id="811d1-112">String</span></span>| <span data-ttu-id="811d1-113">Der Name der stark typisierten-Eigenschaft als Teil einer schemaerweiterung definiert.</span><span class="sxs-lookup"><span data-stu-id="811d1-113">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="811d1-114">Typ</span><span class="sxs-lookup"><span data-stu-id="811d1-114">type</span></span>|<span data-ttu-id="811d1-115">String</span><span class="sxs-lookup"><span data-stu-id="811d1-115">String</span></span>| <span data-ttu-id="811d1-p102">Der Typ der Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.  Zulässige Werte sind *Binary, Boolean, DateTime, Integer* oder *String*.  Weitere Einzelheiten finden Sie in der Tabelle unten.</span><span class="sxs-lookup"><span data-stu-id="811d1-p102">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="811d1-119">Unterstützte Datentypen für Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="811d1-119">Supported property data types</span></span> 
<span data-ttu-id="811d1-120">Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:</span><span class="sxs-lookup"><span data-stu-id="811d1-120">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="811d1-121">Eigenschaftentyp</span><span class="sxs-lookup"><span data-stu-id="811d1-121">Property Type</span></span> | <span data-ttu-id="811d1-122">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="811d1-122">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="811d1-123">Binär</span><span class="sxs-lookup"><span data-stu-id="811d1-123">Binary</span></span> | <span data-ttu-id="811d1-124">Maximal 256 Bytes.</span><span class="sxs-lookup"><span data-stu-id="811d1-124">256 bytes maximum.</span></span> |
| <span data-ttu-id="811d1-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="811d1-125">Boolean</span></span> | <span data-ttu-id="811d1-126">Nicht unterstützt für Nachrichten, Ereignisse und Beiträge.</span><span class="sxs-lookup"><span data-stu-id="811d1-126">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="811d1-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="811d1-127">DateTime</span></span> | <span data-ttu-id="811d1-p103">Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert.</span><span class="sxs-lookup"><span data-stu-id="811d1-p103">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="811d1-130">Ganze Zahl</span><span class="sxs-lookup"><span data-stu-id="811d1-130">Integer</span></span> | <span data-ttu-id="811d1-p104">32-Bit-Wert. Nicht unterstützt für Nachrichten, Ereignisse und Beiträge.</span><span class="sxs-lookup"><span data-stu-id="811d1-p104">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="811d1-133">String</span><span class="sxs-lookup"><span data-stu-id="811d1-133">String</span></span> | <span data-ttu-id="811d1-134">Maximal 256 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="811d1-134">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="811d1-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="811d1-135">JSON representation</span></span>
<span data-ttu-id="811d1-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="811d1-136">Here is a JSON representation of the resource.</span></span>

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