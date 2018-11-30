---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
ms.openlocfilehash: 53f6a5559cb90142a88b839a996cb2eedfd1037a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="driverecipient-resource"></a><span data-ttu-id="04d21-102">DriveRecipient-Ressource</span><span class="sxs-lookup"><span data-stu-id="04d21-102">DriveRecipient resource type</span></span>

<span data-ttu-id="04d21-103">Die **DriveRecipient**-Ressource stellt eine Person, eine Gruppe oder einen anderen Empfänger für die Freigabe mit der [Einladen](../api/driveitem_invite.md)-Aktion dar.</span><span class="sxs-lookup"><span data-stu-id="04d21-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem_invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04d21-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="04d21-104">JSON representation</span></span>

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a><span data-ttu-id="04d21-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="04d21-105">Properties</span></span>
<span data-ttu-id="04d21-106">Die Empfängerressource besitzt die folgenden Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="04d21-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="04d21-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="04d21-107">Property name</span></span> | <span data-ttu-id="04d21-108">Typ</span><span class="sxs-lookup"><span data-stu-id="04d21-108">Type</span></span>   | <span data-ttu-id="04d21-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04d21-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="04d21-110">E-Mail</span><span class="sxs-lookup"><span data-stu-id="04d21-110">email</span></span>         | <span data-ttu-id="04d21-111">String</span><span class="sxs-lookup"><span data-stu-id="04d21-111">String</span></span> | <span data-ttu-id="04d21-112">Die E-Mail-Adresse des Empfängers, wenn der Empfänger eine zugehörige E-Mail-Adresse aufweist.</span><span class="sxs-lookup"><span data-stu-id="04d21-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="04d21-113">Alias</span><span class="sxs-lookup"><span data-stu-id="04d21-113">alias</span></span>         | <span data-ttu-id="04d21-114">String</span><span class="sxs-lookup"><span data-stu-id="04d21-114">String</span></span> | <span data-ttu-id="04d21-115">Der Alias des Domänenobjekts, für Fälle, in denen keine E-Mail-Adresse verfügbar ist (z. B. bei Sicherheitsgruppen).</span><span class="sxs-lookup"><span data-stu-id="04d21-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="04d21-116">objectId</span><span class="sxs-lookup"><span data-stu-id="04d21-116">objectId</span></span>      | <span data-ttu-id="04d21-117">String</span><span class="sxs-lookup"><span data-stu-id="04d21-117">String</span></span> | <span data-ttu-id="04d21-118">Der eindeutige Bezeichner für den Empfänger im Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="04d21-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="04d21-119">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="04d21-119">Remarks</span></span>

<span data-ttu-id="04d21-120">Bei Verwendung von [invite](../api/driveitem_invite.md) zum Hinzufügen von Berechtigungen kann im DriveRecipient **email**, **alias** oder **objectId** angegeben sein.</span><span class="sxs-lookup"><span data-stu-id="04d21-120">When using invite to add permissions, the DriveRecipient can specify email, alias, or objectId. Only one of these values is required.</span></span>
<span data-ttu-id="04d21-121">Nur einer dieser Werte ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04d21-121">Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
