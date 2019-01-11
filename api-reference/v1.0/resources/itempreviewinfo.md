---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
ms.openlocfilehash: e7df636f9c406a499baa5ef3be1748273920cac4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885477"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="2090f-102">Ressourcentyp itemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="2090f-102">itemPreviewInfo resource type</span></span>

<span data-ttu-id="2090f-103">Die Ressource **ItemPreviewInfo** enthält Informationen dazu, wie eine Vorschau einer [DriveItem](driveitem.md)einbetten.</span><span class="sxs-lookup"><span data-stu-id="2090f-103">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2090f-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2090f-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="2090f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2090f-105">Properties</span></span>

| <span data-ttu-id="2090f-106">Name</span><span class="sxs-lookup"><span data-stu-id="2090f-106">Name</span></span>           | <span data-ttu-id="2090f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2090f-107">Type</span></span>   | <span data-ttu-id="2090f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2090f-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="2090f-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="2090f-109">getUrl</span></span>         | <span data-ttu-id="2090f-110">string</span><span class="sxs-lookup"><span data-stu-id="2090f-110">string</span></span> | <span data-ttu-id="2090f-111">URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet</span><span class="sxs-lookup"><span data-stu-id="2090f-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="2090f-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="2090f-112">postUrl</span></span>        | <span data-ttu-id="2090f-113">string</span><span class="sxs-lookup"><span data-stu-id="2090f-113">string</span></span> | <span data-ttu-id="2090f-114">URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)</span><span class="sxs-lookup"><span data-stu-id="2090f-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="2090f-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="2090f-115">postParameters</span></span> | <span data-ttu-id="2090f-116">string</span><span class="sxs-lookup"><span data-stu-id="2090f-116">string</span></span> | <span data-ttu-id="2090f-117">POST-Parameter einschließen, wenn PostUrl verwenden</span><span class="sxs-lookup"><span data-stu-id="2090f-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="2090f-118">GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status der Unterstützung für den angegebenen Optionen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2090f-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="2090f-119">PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2090f-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="2090f-120">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="2090f-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="2090f-121">Die Formate der URLs und Parametern sollten nicht transparent berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="2090f-121">The formats of URLs and parameters should be considered opaque.</span></span>
