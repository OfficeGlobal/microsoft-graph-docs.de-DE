---
title: Ressourcentyp typedEmailAddress
description: Stellt den Namen, e-Mail-Adressen und ihre entsprechenden e-Mail-Adresstyp eines Kontakts an.
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510708"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="83a63-103">Ressourcentyp typedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="83a63-103">typedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83a63-104">Stellt den Namen, e-Mail-Adressen und ihre entsprechenden e-Mail-Adresstyp [wenden Sie sich an](contact.md).</span><span class="sxs-lookup"><span data-stu-id="83a63-104">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="83a63-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83a63-105">Properties</span></span>
| <span data-ttu-id="83a63-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83a63-106">Property</span></span>     | <span data-ttu-id="83a63-107">Typ</span><span class="sxs-lookup"><span data-stu-id="83a63-107">Type</span></span>   |<span data-ttu-id="83a63-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83a63-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83a63-109">address</span><span class="sxs-lookup"><span data-stu-id="83a63-109">address</span></span>|<span data-ttu-id="83a63-110">String</span><span class="sxs-lookup"><span data-stu-id="83a63-110">String</span></span>|<span data-ttu-id="83a63-111">Die e-Mail-Adresse eines Kontakts.</span><span class="sxs-lookup"><span data-stu-id="83a63-111">The email address of a contact.</span></span>|
|<span data-ttu-id="83a63-112">name</span><span class="sxs-lookup"><span data-stu-id="83a63-112">name</span></span>|<span data-ttu-id="83a63-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83a63-113">String</span></span>|<span data-ttu-id="83a63-114">Der Anzeigename eines Kontakts.</span><span class="sxs-lookup"><span data-stu-id="83a63-114">The display name of a contact.</span></span>|
|<span data-ttu-id="83a63-115">type</span><span class="sxs-lookup"><span data-stu-id="83a63-115">type</span></span> |<span data-ttu-id="83a63-116">String</span><span class="sxs-lookup"><span data-stu-id="83a63-116">String</span></span> |<span data-ttu-id="83a63-117">Der Typ des e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="83a63-117">The type of email address.</span></span> <span data-ttu-id="83a63-118">Mögliche Werte sind: `unknown`, `work`, `personal`, `main` und `other`.</span><span class="sxs-lookup"><span data-stu-id="83a63-118">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="83a63-119">Der Standardwert ist `unknown`, d. h. **Adresse** wurde nicht als ein bestimmter Typ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="83a63-119">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="83a63-120">otherLabel</span><span class="sxs-lookup"><span data-stu-id="83a63-120">otherLabel</span></span> |<span data-ttu-id="83a63-121">String</span><span class="sxs-lookup"><span data-stu-id="83a63-121">String</span></span>  |<span data-ttu-id="83a63-122">Wenn Sie einen benutzerdefinierten Typ des e-Mail-Adresse angeben, legen Sie **Typ** auf `other`, und weisen Sie eine benutzerdefinierte Zeichenfolge **OtherLabel** .</span><span class="sxs-lookup"><span data-stu-id="83a63-122">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="83a63-123">Beispielsweise können Sie eine bestimmte e-Mail-Adresse für Ihre freiwillige Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="83a63-123">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="83a63-124">Legen Sie **Typ** `other`, und legen Sie **OtherLabel** auf eine benutzerdefinierte Zeichenfolge wie `Volunteer work`.</span><span class="sxs-lookup"><span data-stu-id="83a63-124">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="83a63-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83a63-125">JSON representation</span></span>

<span data-ttu-id="83a63-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="83a63-126">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
