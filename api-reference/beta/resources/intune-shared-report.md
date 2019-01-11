---
title: report-Ressourcentyp
description: 'Gibt den Inhalt für den Kontext, einschließlich:'
localization_priority: Normal
ms.openlocfilehash: b44d03c12b788b10ca332c868083bc28decc4947
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875726"
---
# <a name="report-resource-type"></a><span data-ttu-id="5cfc3-103">report-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5cfc3-103">report resource type</span></span>

> <span data-ttu-id="5cfc3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5cfc3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cfc3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5cfc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cfc3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5cfc3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cfc3-107">Gibt den Inhalt für den Kontext, einschließlich:</span><span class="sxs-lookup"><span data-stu-id="5cfc3-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="5cfc3-108">Gerät Konfiguration Profil Verlauf von Berichten.</span><span class="sxs-lookup"><span data-stu-id="5cfc3-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="5cfc3-109">Registrierung Fehler Berichte.</span><span class="sxs-lookup"><span data-stu-id="5cfc3-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="5cfc3-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5cfc3-110">Properties</span></span>
|<span data-ttu-id="5cfc3-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5cfc3-111">Property</span></span>|<span data-ttu-id="5cfc3-112">Typ</span><span class="sxs-lookup"><span data-stu-id="5cfc3-112">Type</span></span>|<span data-ttu-id="5cfc3-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5cfc3-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cfc3-114">Inhalt</span><span class="sxs-lookup"><span data-stu-id="5cfc3-114">content</span></span>|<span data-ttu-id="5cfc3-115">Stream</span><span class="sxs-lookup"><span data-stu-id="5cfc3-115">Stream</span></span>|<span data-ttu-id="5cfc3-116">Berichtsinhalt; Details variieren je nach Typ des Berichts.</span><span class="sxs-lookup"><span data-stu-id="5cfc3-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cfc3-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5cfc3-117">Relationships</span></span>
<span data-ttu-id="5cfc3-118">Keine</span><span class="sxs-lookup"><span data-stu-id="5cfc3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cfc3-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5cfc3-119">JSON Representation</span></span>
<span data-ttu-id="5cfc3-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5cfc3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



