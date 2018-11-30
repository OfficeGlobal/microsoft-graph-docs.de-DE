---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: ba909158ce0ba28b6af20b8dbff858c65f07cbe9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064190"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="ba5fd-102">SharingInvitation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ba5fd-102">SharingInvitation resource type</span></span>

> <span data-ttu-id="ba5fd-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ba5fd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba5fd-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba5fd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba5fd-105">Die **SharingInvitation**-Ressource gruppiert Datenelemente im Zusammenhang mit einer Einladung in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="ba5fd-105">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba5fd-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ba5fd-106">JSON representation</span></span>

<span data-ttu-id="ba5fd-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ba5fd-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="ba5fd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ba5fd-108">Properties</span></span>

| <span data-ttu-id="ba5fd-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="ba5fd-109">Property Name</span></span>  | <span data-ttu-id="ba5fd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ba5fd-110">Type</span></span>                          | <span data-ttu-id="ba5fd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba5fd-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ba5fd-112">E-Mail</span><span class="sxs-lookup"><span data-stu-id="ba5fd-112">email</span></span>          | <span data-ttu-id="ba5fd-113">String</span><span class="sxs-lookup"><span data-stu-id="ba5fd-113">String</span></span>                        | <span data-ttu-id="ba5fd-p102">Die für den Empfänger der Freigabeeinladung angegebene E-Mail-Adresse. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ba5fd-p102">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="ba5fd-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="ba5fd-116">invitedBy</span></span>      | [<span data-ttu-id="ba5fd-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="ba5fd-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="ba5fd-p103">Stellt Informationen zum Absender der Einladung bereit, der diese Berechtigung erstellt hat, wenn diese Informationen verfügbar sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ba5fd-p103">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="ba5fd-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="ba5fd-120">signInRequired</span></span> | <span data-ttu-id="ba5fd-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5fd-121">Boolean</span></span>                       | <span data-ttu-id="ba5fd-p104">Bei `true` muss sich der Empfänger der Einladung anmelden, um auf das freigegebene Element zugreifen zu können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ba5fd-p104">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="ba5fd-124">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="ba5fd-124">Remarks</span></span> 

<span data-ttu-id="ba5fd-125">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ba5fd-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": ""
}-->
