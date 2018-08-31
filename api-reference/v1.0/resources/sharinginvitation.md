---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 9237c401fd83a7b30303f147402262c022b820a7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265855"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="7508e-102">SharingInvitation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7508e-102">SharingInvitation resource type</span></span>

<span data-ttu-id="7508e-103">Die **SharingInvitation**-Ressource gruppiert Datenelemente im Zusammenhang mit einer Einladung in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="7508e-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7508e-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7508e-104">JSON representation</span></span>

<span data-ttu-id="7508e-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7508e-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}
```

## <a name="properties"></a><span data-ttu-id="7508e-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7508e-106">Properties</span></span>

| <span data-ttu-id="7508e-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="7508e-107">Property Name</span></span>  | <span data-ttu-id="7508e-108">Typ</span><span class="sxs-lookup"><span data-stu-id="7508e-108">Type</span></span>            | <span data-ttu-id="7508e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7508e-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="7508e-110">E-Mail</span><span class="sxs-lookup"><span data-stu-id="7508e-110">email</span></span>          | <span data-ttu-id="7508e-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7508e-111">String</span></span>          | <span data-ttu-id="7508e-p101">Die für den Empfänger der Freigabeeinladung angegebene E-Mail-Adresse. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7508e-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="7508e-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="7508e-114">invitedBy</span></span>      | <span data-ttu-id="7508e-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7508e-115">[identitySet][]</span></span> | <span data-ttu-id="7508e-p102">Stellt Informationen zum Absender der Einladung bereit, der diese Berechtigung erstellt hat, wenn diese Informationen verfügbar sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7508e-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="7508e-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="7508e-118">signInRequired</span></span> | <span data-ttu-id="7508e-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7508e-119">Boolean</span></span>         | <span data-ttu-id="7508e-p103">Bei `true` muss sich der Empfänger der Einladung anmelden, um auf das freigegebene Element zugreifen zu können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7508e-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="7508e-122">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="7508e-122">Remarks</span></span>

<span data-ttu-id="7508e-123">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7508e-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveItem.md
[IdentitySet]: identitySet.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
