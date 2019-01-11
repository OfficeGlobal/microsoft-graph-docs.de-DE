---
title: Ressourcentyp Sicherheit
description: Die Sicherheitsressource ist der Einstiegspunkt für das Objektmodell Sicherheit. Es gibt eine Singleton Sicherheitsressource zurück. Es enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
ms.openlocfilehash: 2486bf9cae2ffad471c1bacb8b7ca01c6bef4ee7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827013"
---
# <a name="security-resource-type"></a><span data-ttu-id="46eaf-105">Ressourcentyp Sicherheit</span><span class="sxs-lookup"><span data-stu-id="46eaf-105">security resource type</span></span>

<span data-ttu-id="46eaf-106">Die Sicherheitsressource ist der Einstiegspunkt für das Objektmodell Sicherheit.</span><span class="sxs-lookup"><span data-stu-id="46eaf-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="46eaf-107">Es gibt eine Singleton Sicherheitsressource zurück.</span><span class="sxs-lookup"><span data-stu-id="46eaf-107">It returns a singleton security resource.</span></span> <span data-ttu-id="46eaf-108">Es enthält keine verwendbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="46eaf-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="46eaf-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="46eaf-109">Methods</span></span>

| <span data-ttu-id="46eaf-110">Methode</span><span class="sxs-lookup"><span data-stu-id="46eaf-110">Method</span></span>       | <span data-ttu-id="46eaf-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="46eaf-111">Return Type</span></span> | <span data-ttu-id="46eaf-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46eaf-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="46eaf-113">Warnungen auflisten</span><span class="sxs-lookup"><span data-stu-id="46eaf-113">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="46eaf-114">[Warnung](alert.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="46eaf-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="46eaf-115">Rufen Sie eine Auflistung der alert-Objekts.</span><span class="sxs-lookup"><span data-stu-id="46eaf-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="46eaf-116">Benachrichtigungen erhalten möchten</span><span class="sxs-lookup"><span data-stu-id="46eaf-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="46eaf-117">[Warnung](alert.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="46eaf-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="46eaf-118">Rufen Sie ein alert-Objekt.</span><span class="sxs-lookup"><span data-stu-id="46eaf-118">Get a alert object.</span></span> |
| [<span data-ttu-id="46eaf-119">Aktualisieren von Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="46eaf-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="46eaf-120">[Warnung](alert.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="46eaf-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="46eaf-121">Rufen Sie ein alert-Objekt.</span><span class="sxs-lookup"><span data-stu-id="46eaf-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="46eaf-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46eaf-122">Properties</span></span>
<span data-ttu-id="46eaf-123">Keine</span><span class="sxs-lookup"><span data-stu-id="46eaf-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="46eaf-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="46eaf-124">Relationships</span></span>
| <span data-ttu-id="46eaf-125">Beziehung</span><span class="sxs-lookup"><span data-stu-id="46eaf-125">Relationship</span></span> | <span data-ttu-id="46eaf-126">Typ</span><span class="sxs-lookup"><span data-stu-id="46eaf-126">Type</span></span>        | <span data-ttu-id="46eaf-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46eaf-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46eaf-128">alerts</span><span class="sxs-lookup"><span data-stu-id="46eaf-128">alerts</span></span>|<span data-ttu-id="46eaf-129">[Warnung](alert.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="46eaf-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="46eaf-p103">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="46eaf-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="46eaf-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46eaf-132">JSON representation</span></span>
<span data-ttu-id="46eaf-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46eaf-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="46eaf-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46eaf-134">Example</span></span>

<span data-ttu-id="46eaf-135">**Die Sicherheitsressource** steht im Stamm des Diagramms.</span><span class="sxs-lookup"><span data-stu-id="46eaf-135">The **security** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
