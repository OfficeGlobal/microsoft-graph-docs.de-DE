---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.openlocfilehash: 8b8f7a962e237cc20a42503efd31f083996ad715
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018452"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="23177-102">Ressourcentyp itemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="23177-102">itemPreviewInfo resource type</span></span>

<span data-ttu-id="23177-103">Die Ressource **ItemPreviewInfo** enthält Informationen dazu, wie eine Vorschau einer [DriveItem](driveitem.md)einbetten.</span><span class="sxs-lookup"><span data-stu-id="23177-103">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="23177-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23177-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="23177-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23177-105">Properties</span></span>

| <span data-ttu-id="23177-106">Name</span><span class="sxs-lookup"><span data-stu-id="23177-106">Name</span></span>           | <span data-ttu-id="23177-107">Typ</span><span class="sxs-lookup"><span data-stu-id="23177-107">Type</span></span>   | <span data-ttu-id="23177-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23177-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="23177-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="23177-109">getUrl</span></span>         | <span data-ttu-id="23177-110">string</span><span class="sxs-lookup"><span data-stu-id="23177-110">string</span></span> | <span data-ttu-id="23177-111">URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet</span><span class="sxs-lookup"><span data-stu-id="23177-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="23177-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="23177-112">postUrl</span></span>        | <span data-ttu-id="23177-113">string</span><span class="sxs-lookup"><span data-stu-id="23177-113">string</span></span> | <span data-ttu-id="23177-114">URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)</span><span class="sxs-lookup"><span data-stu-id="23177-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="23177-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="23177-115">postParameters</span></span> | <span data-ttu-id="23177-116">string</span><span class="sxs-lookup"><span data-stu-id="23177-116">string</span></span> | <span data-ttu-id="23177-117">POST-Parameter einschließen, wenn PostUrl verwenden</span><span class="sxs-lookup"><span data-stu-id="23177-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="23177-118">GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status der Unterstützung für den angegebenen Optionen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23177-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="23177-119">PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="23177-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="23177-120">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="23177-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="23177-121">Die Formate der URLs und Parametern sollten nicht transparent berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="23177-121">The formats of URLs and parameters should be considered opaque.</span></span>
