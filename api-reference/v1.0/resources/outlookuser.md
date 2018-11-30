---
title: outlookUser-Ressourcentyp
description: Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.
ms.openlocfilehash: 63bbabccc540046961d31c91fe7b1fb9afaaf4f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019327"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="d3e6a-103">outlookUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d3e6a-103">outlookUser resource type</span></span>


<span data-ttu-id="d3e6a-104">Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.</span><span class="sxs-lookup"><span data-stu-id="d3e6a-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="d3e6a-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d3e6a-105">Methods</span></span>

| <span data-ttu-id="d3e6a-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d3e6a-106">Method</span></span>           | <span data-ttu-id="d3e6a-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d3e6a-107">Return Type</span></span>    |<span data-ttu-id="d3e6a-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3e6a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3e6a-109">Kategorie erstellen</span><span class="sxs-lookup"><span data-stu-id="d3e6a-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="d3e6a-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="d3e6a-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="d3e6a-111">Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="d3e6a-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="d3e6a-112">Kategorien auflisten</span><span class="sxs-lookup"><span data-stu-id="d3e6a-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="d3e6a-113">[outlookCategory](outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d3e6a-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="d3e6a-114">Ruft alle Kategorien ab, die für den Benutzer definiert wurden.</span><span class="sxs-lookup"><span data-stu-id="d3e6a-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="d3e6a-115">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="d3e6a-115">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="d3e6a-116">[localeInfo](localeinfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d3e6a-116">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="d3e6a-117">Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="d3e6a-117">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="d3e6a-118">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="d3e6a-118">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="d3e6a-119">[timeZoneInformation](timezoneinformation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d3e6a-119">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="d3e6a-120">Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="d3e6a-120">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="d3e6a-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d3e6a-121">Properties</span></span>
<span data-ttu-id="d3e6a-122">Keine</span><span class="sxs-lookup"><span data-stu-id="d3e6a-122">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d3e6a-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d3e6a-123">Relationships</span></span>
| <span data-ttu-id="d3e6a-124">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d3e6a-124">Relationship</span></span> | <span data-ttu-id="d3e6a-125">Typ</span><span class="sxs-lookup"><span data-stu-id="d3e6a-125">Type</span></span>   |<span data-ttu-id="d3e6a-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3e6a-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3e6a-127">masterCategories</span><span class="sxs-lookup"><span data-stu-id="d3e6a-127">masterCategories</span></span>|<span data-ttu-id="d3e6a-128">[outlookCategory](../resources/outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d3e6a-128">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="d3e6a-129">Eine Liste von Kategorien, die für den Benutzer definiert sind.</span><span class="sxs-lookup"><span data-stu-id="d3e6a-129">A list of categories defined for the user.</span></span> | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->