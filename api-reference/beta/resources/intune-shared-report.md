---
title: report-Ressourcentyp
description: 'Gibt den Inhalt für den Kontext, einschließlich:'
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: dbad8a8808d40c2ae1f7769773b6b29ef65d680f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970647"
---
# <a name="report-resource-type"></a><span data-ttu-id="26a81-103">report-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="26a81-103">report resource type</span></span>

> <span data-ttu-id="26a81-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="26a81-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26a81-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26a81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26a81-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="26a81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26a81-107">Gibt den Inhalt für den Kontext, einschließlich:</span><span class="sxs-lookup"><span data-stu-id="26a81-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="26a81-108">Gerät Konfiguration Profil Verlauf von Berichten.</span><span class="sxs-lookup"><span data-stu-id="26a81-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="26a81-109">Registrierung Fehler Berichte.</span><span class="sxs-lookup"><span data-stu-id="26a81-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="26a81-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="26a81-110">Properties</span></span>
|<span data-ttu-id="26a81-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26a81-111">Property</span></span>|<span data-ttu-id="26a81-112">Typ</span><span class="sxs-lookup"><span data-stu-id="26a81-112">Type</span></span>|<span data-ttu-id="26a81-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26a81-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26a81-114">Inhalt</span><span class="sxs-lookup"><span data-stu-id="26a81-114">content</span></span>|<span data-ttu-id="26a81-115">Stream</span><span class="sxs-lookup"><span data-stu-id="26a81-115">Stream</span></span>|<span data-ttu-id="26a81-116">Berichtsinhalt; Details variieren je nach Typ des Berichts.</span><span class="sxs-lookup"><span data-stu-id="26a81-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26a81-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="26a81-117">Relationships</span></span>
<span data-ttu-id="26a81-118">Keine</span><span class="sxs-lookup"><span data-stu-id="26a81-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26a81-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="26a81-119">JSON Representation</span></span>
<span data-ttu-id="26a81-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="26a81-120">Here is a JSON representation of the resource.</span></span>
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



