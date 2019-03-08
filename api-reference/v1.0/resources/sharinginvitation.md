---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 0cb09136f4093b290f37ee851cb7d2d0ca10c1bf
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480544"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="d226b-102">SharingInvitation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d226b-102">SharingInvitation resource type</span></span>

<span data-ttu-id="d226b-103">Die **SharingInvitation** -Ressource gruppiert Einladungs bezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="d226b-103">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d226b-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d226b-104">JSON representation</span></span>

<span data-ttu-id="d226b-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d226b-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d226b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d226b-106">Properties</span></span>

| <span data-ttu-id="d226b-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d226b-107">Property Name</span></span>  | <span data-ttu-id="d226b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d226b-108">Type</span></span>            | <span data-ttu-id="d226b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d226b-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="d226b-110">E-Mail</span><span class="sxs-lookup"><span data-stu-id="d226b-110">email</span></span>          | <span data-ttu-id="d226b-111">String</span><span class="sxs-lookup"><span data-stu-id="d226b-111">String</span></span>          | <span data-ttu-id="d226b-p101">Die für den Empfänger der Freigabeeinladung angegebene E-Mail-Adresse. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d226b-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="d226b-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="d226b-114">invitedBy</span></span>      | <span data-ttu-id="d226b-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d226b-115">[identitySet][]</span></span> | <span data-ttu-id="d226b-p102">Stellt Informationen zum Absender der Einladung bereit, der diese Berechtigung erstellt hat, wenn diese Informationen verfügbar sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d226b-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="d226b-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="d226b-118">signInRequired</span></span> | <span data-ttu-id="d226b-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d226b-119">Boolean</span></span>         | <span data-ttu-id="d226b-p103">Bei `true` muss sich der Empfänger der Einladung anmelden, um auf das freigegebene Element zugreifen zu können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d226b-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="d226b-122">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="d226b-122">Remarks</span></span>

<span data-ttu-id="d226b-123">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d226b-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
