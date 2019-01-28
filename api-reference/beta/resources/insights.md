---
title: Ressourcentyp officeGraphInsights
description: Einblicke sind Beziehungen, die mithilfe erweiterter Analysetechniken und computergestützter Lerntechniken berechnet werden. Sie können z. B. OneDrive-Dokumente für Benutzer identifizieren.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: daded26bff88d611ea39754d98007fa3329d142b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572458"
---
# <a name="insights-resource-type"></a><span data-ttu-id="43d84-104">insights-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="43d84-104">insights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43d84-105">Einblicke sind Beziehungen, die mithilfe erweiterter Analysetechniken und computergestützter Lerntechniken berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="43d84-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="43d84-106">Sie können z. B. OneDrive-Dokumente für Benutzer identifizieren.</span><span class="sxs-lookup"><span data-stu-id="43d84-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="43d84-107">Einblicke werden von den folgenden APIs zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="43d84-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="43d84-108">[Trending](insights-trending.md): Gibt Dokumente von OneDrive- und SharePoint-Websites zurück, die bei einem Benutzer beliebt sind.</span><span class="sxs-lookup"><span data-stu-id="43d84-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="43d84-109">[Used](insights-used.md): Gibt die zuletzt von einem Benutzer angezeigten oder geänderten Dokumente zurück.</span><span class="sxs-lookup"><span data-stu-id="43d84-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="43d84-110">Umfasst Dokumente, die der Benutzer in OneDrive for Business und SharePoint verwendet und als E-Mail-Anlagen und als Linkanlagen von Quellen wie Box, DropBox and Google Drive geöffnet hat.</span><span class="sxs-lookup"><span data-stu-id="43d84-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="43d84-111">[Shared](insights-shared.md): Gibt Dokumente zurück, die für einen Benutzer freigegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="43d84-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="43d84-112">Dokumente können als E-Mail-Anlagen oder als OneDrive for Business-Links freigegeben werden, die in E-Mails gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="43d84-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="43d84-113">Jeder Einblick wird mit einem komplexen Werttyp von `resourceVisualization` und `resourceReference` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43d84-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="43d84-114">Der komplexe Werttyp „ResourceVisualization“ enthält Eigenschaften wie `title` und `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="43d84-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="43d84-115">Microsoft verwendet die Visualisierungseigenschaften, um die Dateien in Oberflächen wie Office Delve zu rendern.</span><span class="sxs-lookup"><span data-stu-id="43d84-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="43d84-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="43d84-116">Relationships</span></span>

| <span data-ttu-id="43d84-117">Beziehung</span><span class="sxs-lookup"><span data-stu-id="43d84-117">Relationship</span></span>      | <span data-ttu-id="43d84-118">Typ</span><span class="sxs-lookup"><span data-stu-id="43d84-118">Type</span></span>          | <span data-ttu-id="43d84-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43d84-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="43d84-120">trending</span><span class="sxs-lookup"><span data-stu-id="43d84-120">trending</span></span>      | <span data-ttu-id="43d84-121">[Trending](insights-trending.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="43d84-121">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="43d84-122">Berechnete Beziehung, die beliebte Dokumente identifiziert.</span><span class="sxs-lookup"><span data-stu-id="43d84-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="43d84-123">Beliebte Dokumente können auf OneDrive- oder auf SharePoint-Websites gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="43d84-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="43d84-124">used</span><span class="sxs-lookup"><span data-stu-id="43d84-124">used</span></span>      | <span data-ttu-id="43d84-125">[UsedInsight](insights-used.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="43d84-125">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="43d84-126">Berechnete Beziehung, die die von einem Benutzer angezeigten und geänderten Dokumente identifiziert.</span><span class="sxs-lookup"><span data-stu-id="43d84-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="43d84-127">Umfasst Dokumente, die der Benutzer in OneDrive for Business und SharePoint verwendet und als E-Mail-Anlagen und als Linkanlagen von Quellen wie Box, DropBox and Google Drive geöffnet hat.</span><span class="sxs-lookup"><span data-stu-id="43d84-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="43d84-128">shared</span><span class="sxs-lookup"><span data-stu-id="43d84-128">shared</span></span>        | <span data-ttu-id="43d84-129">[Shared](insights-shared.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="43d84-129">[shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="43d84-130">Berechnete Beziehung, die Dokumente identifiziert, die für einen Benutzer freigegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="43d84-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="43d84-131">Dokumente können als E-Mail-Anlagen oder als OneDrive for Business-Links freigegeben werden, die in E-Mails gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="43d84-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="43d84-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="43d84-132">JSON representation</span></span>

<span data-ttu-id="43d84-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="43d84-133">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.officeGraphInsights"
}-->

```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
