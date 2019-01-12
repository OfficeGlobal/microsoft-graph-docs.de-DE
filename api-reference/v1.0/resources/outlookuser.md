---
title: outlookUser-Ressourcentyp
description: Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 32d621b71770d220487b60b4573fb34cdf28d526
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982820"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="9e6e9-103">outlookUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e6e9-103">outlookUser resource type</span></span>


<span data-ttu-id="9e6e9-104">Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.</span><span class="sxs-lookup"><span data-stu-id="9e6e9-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="9e6e9-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="9e6e9-105">Methods</span></span>

| <span data-ttu-id="9e6e9-106">Methode</span><span class="sxs-lookup"><span data-stu-id="9e6e9-106">Method</span></span>           | <span data-ttu-id="9e6e9-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9e6e9-107">Return Type</span></span>    |<span data-ttu-id="9e6e9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e6e9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e6e9-109">Kategorie erstellen</span><span class="sxs-lookup"><span data-stu-id="9e6e9-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="9e6e9-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="9e6e9-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="9e6e9-111">Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="9e6e9-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="9e6e9-112">Kategorien auflisten</span><span class="sxs-lookup"><span data-stu-id="9e6e9-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="9e6e9-113">[outlookCategory](outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9e6e9-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="9e6e9-114">Ruft alle Kategorien ab, die für den Benutzer definiert wurden.</span><span class="sxs-lookup"><span data-stu-id="9e6e9-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="9e6e9-115">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="9e6e9-115">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="9e6e9-116">[localeInfo](localeinfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9e6e9-116">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="9e6e9-117">Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="9e6e9-117">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="9e6e9-118">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="9e6e9-118">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="9e6e9-119">[timeZoneInformation](timezoneinformation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9e6e9-119">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="9e6e9-120">Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="9e6e9-120">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="9e6e9-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e6e9-121">Properties</span></span>
<span data-ttu-id="9e6e9-122">Keine</span><span class="sxs-lookup"><span data-stu-id="9e6e9-122">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9e6e9-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e6e9-123">Relationships</span></span>
| <span data-ttu-id="9e6e9-124">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9e6e9-124">Relationship</span></span> | <span data-ttu-id="9e6e9-125">Typ</span><span class="sxs-lookup"><span data-stu-id="9e6e9-125">Type</span></span>   |<span data-ttu-id="9e6e9-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e6e9-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e6e9-127">masterCategories</span><span class="sxs-lookup"><span data-stu-id="9e6e9-127">masterCategories</span></span>|<span data-ttu-id="9e6e9-128">[outlookCategory](../resources/outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9e6e9-128">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="9e6e9-129">Eine Liste von Kategorien, die für den Benutzer definiert sind.</span><span class="sxs-lookup"><span data-stu-id="9e6e9-129">A list of categories defined for the user.</span></span> | 

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
