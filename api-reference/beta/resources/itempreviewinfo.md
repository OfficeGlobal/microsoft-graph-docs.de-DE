---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive-API
ms.openlocfilehash: 3fa9d10ae3aade7be96e81168b34df84698da1c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059802"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="a7a18-102">Ressourcentyp ItemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="a7a18-102">ItemPreviewInfo resource type</span></span>

> <span data-ttu-id="a7a18-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a7a18-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7a18-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a7a18-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7a18-105">Die Ressource **ItemPreviewInfo** enthält Informationen dazu, wie eine Vorschau einer [DriveItem](driveitem.md)einbetten.</span><span class="sxs-lookup"><span data-stu-id="a7a18-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7a18-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a7a18-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="a7a18-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a7a18-107">Properties</span></span>

| <span data-ttu-id="a7a18-108">Name</span><span class="sxs-lookup"><span data-stu-id="a7a18-108">Name</span></span>           | <span data-ttu-id="a7a18-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a7a18-109">Type</span></span>   | <span data-ttu-id="a7a18-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7a18-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="a7a18-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="a7a18-111">getUrl</span></span>         | <span data-ttu-id="a7a18-112">string</span><span class="sxs-lookup"><span data-stu-id="a7a18-112">string</span></span> | <span data-ttu-id="a7a18-113">URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet</span><span class="sxs-lookup"><span data-stu-id="a7a18-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="a7a18-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="a7a18-114">postUrl</span></span>        | <span data-ttu-id="a7a18-115">string</span><span class="sxs-lookup"><span data-stu-id="a7a18-115">string</span></span> | <span data-ttu-id="a7a18-116">URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)</span><span class="sxs-lookup"><span data-stu-id="a7a18-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="a7a18-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="a7a18-117">postParameters</span></span> | <span data-ttu-id="a7a18-118">string</span><span class="sxs-lookup"><span data-stu-id="a7a18-118">string</span></span> | <span data-ttu-id="a7a18-119">POST-Parameter einschließen, wenn PostUrl verwenden</span><span class="sxs-lookup"><span data-stu-id="a7a18-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="a7a18-120">GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status der Unterstützung für den angegebenen Optionen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a7a18-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="a7a18-121">PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a7a18-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="a7a18-122">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="a7a18-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="a7a18-123">Die Formate der URLs und Parametern sollten nicht transparent berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="a7a18-123">The formats of URLs and parameters should be considered opaque.</span></span>