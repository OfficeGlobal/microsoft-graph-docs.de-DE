---
title: Einblicke in die Ressourcentyp
description: Einblicke in die sind Beziehungen mit erweiterten Analyse- und Techniken erlernen Computer berechnet. Sie können, zum Beispiel OneDrive Dokumente, um Benutzer Trend identifizieren.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 38f7afb40c1618a8a7cf9d585c99633e2bb8d940
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938314"
---
# <a name="insights-resource-type"></a><span data-ttu-id="51488-104">Einblicke in die Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="51488-104">insights resource type</span></span>

> <span data-ttu-id="51488-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51488-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51488-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51488-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51488-107">Einblicke in die sind Beziehungen mit erweiterten Analyse- und Techniken erlernen Computer berechnet.</span><span class="sxs-lookup"><span data-stu-id="51488-107">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="51488-108">Sie können, zum Beispiel OneDrive Dokumente, um Benutzer Trend identifizieren.</span><span class="sxs-lookup"><span data-stu-id="51488-108">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="51488-109">Einblicke in die werden durch die folgenden APIs zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="51488-109">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="51488-110">[Trending](insights-trending.md) - gibt Dokumente aus OneDrive und aus SharePoint-Websites, um einen Benutzer Trend zurück.</span><span class="sxs-lookup"><span data-stu-id="51488-110">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="51488-111">[Used](insights-used.md) - gibt Dokumente angezeigt und geändert werden, von einem Benutzer zurück.</span><span class="sxs-lookup"><span data-stu-id="51488-111">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="51488-112">Enthält Dokumente, die der Benutzer verwendet in OneDrive für Unternehmen, SharePoint, als e-Mail-Anlagen und als Link Anlagen aus Quellen wie Feld, Ablage und Google Laufwerk geöffnet wurde.</span><span class="sxs-lookup"><span data-stu-id="51488-112">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="51488-113">[Shared](insights-shared.md) - gibt mit einem Benutzer freigegebene Dokumente zurück.</span><span class="sxs-lookup"><span data-stu-id="51488-113">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="51488-114">Dokumente können als e-Mail-Anlage oder als OneDrive freigegeben werden for Business in gesendete e-Mails verknüpft.</span><span class="sxs-lookup"><span data-stu-id="51488-114">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="51488-115">Jede Erkenntnisse wird zurückgegeben, mit einer `resourceVisualization` und `resourceReference` komplexe Werttyp (CVT).</span><span class="sxs-lookup"><span data-stu-id="51488-115">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="51488-116">Die ResourceVisualization CVT enthält Eigenschaften wie `title` und `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="51488-116">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="51488-117">Microsoft verwendet die Visualisierungseigenschaften zum Rendern von Dateien im Erfahrungen wie Office ausführlicher behandelt.</span><span class="sxs-lookup"><span data-stu-id="51488-117">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="51488-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="51488-118">Relationships</span></span>

| <span data-ttu-id="51488-119">Beziehung</span><span class="sxs-lookup"><span data-stu-id="51488-119">Relationship</span></span>      | <span data-ttu-id="51488-120">Typ</span><span class="sxs-lookup"><span data-stu-id="51488-120">Type</span></span>          | <span data-ttu-id="51488-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51488-121">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="51488-122">Trend</span><span class="sxs-lookup"><span data-stu-id="51488-122">trending</span></span>      | <span data-ttu-id="51488-123">[Trending](insights-trending.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="51488-123">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="51488-124">Berechnete Beziehung Identifizieren von Trend Dokumenten.</span><span class="sxs-lookup"><span data-stu-id="51488-124">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="51488-125">Trend Dokumente können in OneDrive oder in SharePoint-Websites gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="51488-125">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="51488-126">verwendet</span><span class="sxs-lookup"><span data-stu-id="51488-126">used</span></span>      | <span data-ttu-id="51488-127">[Used](insights-used.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="51488-127">[Used](insights-used.md) collection</span></span>       | <span data-ttu-id="51488-128">Identifizieren von Dokumenten angezeigt und geändert werden, von einem Benutzer Beziehung berechnet.</span><span class="sxs-lookup"><span data-stu-id="51488-128">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="51488-129">Enthält Dokumente, die der Benutzer verwendet in OneDrive für Unternehmen, SharePoint, als e-Mail-Anlagen und als Link Anlagen aus Quellen wie Feld, Ablage und Google Laufwerk geöffnet wurde.</span><span class="sxs-lookup"><span data-stu-id="51488-129">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="51488-130">shared</span><span class="sxs-lookup"><span data-stu-id="51488-130">shared</span></span>        | <span data-ttu-id="51488-131">[Shared](insights-shared.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="51488-131">[Shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="51488-132">Berechnete Beziehung Identifizieren von Dokumenten, die ein Benutzer freigegeben.</span><span class="sxs-lookup"><span data-stu-id="51488-132">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="51488-133">Dokumente können als e-Mail-Anlage oder als OneDrive freigegeben werden for Business in gesendete e-Mails verknüpft.</span><span class="sxs-lookup"><span data-stu-id="51488-133">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="51488-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="51488-134">JSON representation</span></span>

<span data-ttu-id="51488-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="51488-135">Here is a JSON representation of the resource</span></span>
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
