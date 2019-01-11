---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive-API
localization_priority: Normal
ms.openlocfilehash: 0f2a161b9b43a8d372b90530b1b9d9244f77d8e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857344"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="ad644-102">Ressourcentyp ItemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="ad644-102">ItemPreviewInfo resource type</span></span>

> <span data-ttu-id="ad644-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ad644-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad644-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad644-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad644-105">Die Ressource **ItemPreviewInfo** enthält Informationen dazu, wie eine Vorschau einer [DriveItem](driveitem.md)einbetten.</span><span class="sxs-lookup"><span data-stu-id="ad644-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad644-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad644-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="ad644-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad644-107">Properties</span></span>

| <span data-ttu-id="ad644-108">Name</span><span class="sxs-lookup"><span data-stu-id="ad644-108">Name</span></span>           | <span data-ttu-id="ad644-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ad644-109">Type</span></span>   | <span data-ttu-id="ad644-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad644-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="ad644-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="ad644-111">getUrl</span></span>         | <span data-ttu-id="ad644-112">string</span><span class="sxs-lookup"><span data-stu-id="ad644-112">string</span></span> | <span data-ttu-id="ad644-113">URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet</span><span class="sxs-lookup"><span data-stu-id="ad644-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="ad644-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="ad644-114">postUrl</span></span>        | <span data-ttu-id="ad644-115">string</span><span class="sxs-lookup"><span data-stu-id="ad644-115">string</span></span> | <span data-ttu-id="ad644-116">URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)</span><span class="sxs-lookup"><span data-stu-id="ad644-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="ad644-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="ad644-117">postParameters</span></span> | <span data-ttu-id="ad644-118">string</span><span class="sxs-lookup"><span data-stu-id="ad644-118">string</span></span> | <span data-ttu-id="ad644-119">POST-Parameter einschließen, wenn PostUrl verwenden</span><span class="sxs-lookup"><span data-stu-id="ad644-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="ad644-120">GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status der Unterstützung für den angegebenen Optionen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad644-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="ad644-121">PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ad644-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="ad644-122">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ad644-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="ad644-123">Die Formate der URLs und Parametern sollten nicht transparent berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="ad644-123">The formats of URLs and parameters should be considered opaque.</span></span>
