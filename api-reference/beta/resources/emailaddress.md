---
title: emailAddress-Ressourcentyp
description: Stellt den Namen und die SMTP-Adresse einer Instanz einer Entität, beispielsweise eine Nachricht Empfänger oder Kalender Besitzer.
ms.openlocfilehash: f607fe4ce01b9a3c3f5e7af5aa1638fef3840177
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059178"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="e82db-103">emailAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e82db-103">emailAddress resource type</span></span>

> <span data-ttu-id="e82db-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e82db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e82db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e82db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e82db-106">Stellt den Namen und die SMTP-Adresse einer Instanz einer Entität, beispielsweise eine Nachricht Empfänger oder Kalender Besitzer.</span><span class="sxs-lookup"><span data-stu-id="e82db-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="e82db-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e82db-107">Properties</span></span>
| <span data-ttu-id="e82db-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e82db-108">Property</span></span>     | <span data-ttu-id="e82db-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e82db-109">Type</span></span>   |<span data-ttu-id="e82db-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e82db-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e82db-111">address</span><span class="sxs-lookup"><span data-stu-id="e82db-111">address</span></span>|<span data-ttu-id="e82db-112">String</span><span class="sxs-lookup"><span data-stu-id="e82db-112">String</span></span>|<span data-ttu-id="e82db-113">Die e-Mail-Adresse einer Instanz einer Entität.</span><span class="sxs-lookup"><span data-stu-id="e82db-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="e82db-114">name</span><span class="sxs-lookup"><span data-stu-id="e82db-114">name</span></span>|<span data-ttu-id="e82db-115">String</span><span class="sxs-lookup"><span data-stu-id="e82db-115">String</span></span>|<span data-ttu-id="e82db-116">Der Anzeigename einer Instanz einer Entität.</span><span class="sxs-lookup"><span data-stu-id="e82db-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e82db-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e82db-117">JSON representation</span></span>

<span data-ttu-id="e82db-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e82db-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
