---
title: Ressourcentyp typedEmailAddress
description: Stellt den Namen, e-Mail-Adressen und ihre entsprechenden e-Mail-Adresstyp eines Kontakts an.
ms.openlocfilehash: 3f40add32fbc219606b6d78041552fc108803d1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066073"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="42e0e-103">Ressourcentyp typedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="42e0e-103">typedEmailAddress resource type</span></span>

> <span data-ttu-id="42e0e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="42e0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42e0e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="42e0e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42e0e-106">Stellt den Namen, e-Mail-Adressen und ihre entsprechenden e-Mail-Adresstyp [wenden Sie sich an](contact.md).</span><span class="sxs-lookup"><span data-stu-id="42e0e-106">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="42e0e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="42e0e-107">Properties</span></span>
| <span data-ttu-id="42e0e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42e0e-108">Property</span></span>     | <span data-ttu-id="42e0e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="42e0e-109">Type</span></span>   |<span data-ttu-id="42e0e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42e0e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42e0e-111">address</span><span class="sxs-lookup"><span data-stu-id="42e0e-111">address</span></span>|<span data-ttu-id="42e0e-112">String</span><span class="sxs-lookup"><span data-stu-id="42e0e-112">String</span></span>|<span data-ttu-id="42e0e-113">Die e-Mail-Adresse eines Kontakts.</span><span class="sxs-lookup"><span data-stu-id="42e0e-113">The email address of a contact.</span></span>|
|<span data-ttu-id="42e0e-114">name</span><span class="sxs-lookup"><span data-stu-id="42e0e-114">name</span></span>|<span data-ttu-id="42e0e-115">String</span><span class="sxs-lookup"><span data-stu-id="42e0e-115">String</span></span>|<span data-ttu-id="42e0e-116">Der Anzeigename eines Kontakts.</span><span class="sxs-lookup"><span data-stu-id="42e0e-116">The display name of a contact.</span></span>|
|<span data-ttu-id="42e0e-117">Typ</span><span class="sxs-lookup"><span data-stu-id="42e0e-117">type</span></span> |<span data-ttu-id="42e0e-118">String</span><span class="sxs-lookup"><span data-stu-id="42e0e-118">String</span></span> |<span data-ttu-id="42e0e-119">Der Typ des e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="42e0e-119">The type of email address.</span></span> <span data-ttu-id="42e0e-120">Mögliche Werte sind: `unknown`, `work`, `personal`, `main` und `other`.</span><span class="sxs-lookup"><span data-stu-id="42e0e-120">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="42e0e-121">Der Standardwert ist `unknown`, d. h. **Adresse** wurde nicht als ein bestimmter Typ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="42e0e-121">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="42e0e-122">otherLabel</span><span class="sxs-lookup"><span data-stu-id="42e0e-122">otherLabel</span></span> |<span data-ttu-id="42e0e-123">String</span><span class="sxs-lookup"><span data-stu-id="42e0e-123">String</span></span>  |<span data-ttu-id="42e0e-124">Wenn Sie einen benutzerdefinierten Typ des e-Mail-Adresse angeben, legen Sie **Typ** auf `other`, und weisen Sie eine benutzerdefinierte Zeichenfolge **OtherLabel** .</span><span class="sxs-lookup"><span data-stu-id="42e0e-124">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="42e0e-125">Beispielsweise können Sie eine bestimmte e-Mail-Adresse für Ihre freiwillige Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="42e0e-125">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="42e0e-126">Legen Sie **Typ** `other`, und legen Sie **OtherLabel** auf eine benutzerdefinierte Zeichenfolge wie `Volunteer work`.</span><span class="sxs-lookup"><span data-stu-id="42e0e-126">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42e0e-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="42e0e-127">JSON representation</span></span>

<span data-ttu-id="42e0e-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="42e0e-128">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
