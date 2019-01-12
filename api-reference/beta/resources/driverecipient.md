---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 85def7dd812d2046e02f814cf63e9f82b28d2781
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919687"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="d71b3-102">DriveRecipient-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d71b3-102">DriveRecipient resource</span></span>

> <span data-ttu-id="d71b3-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d71b3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d71b3-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d71b3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d71b3-105">Die **DriveRecipient**-Ressource stellt eine Person, eine Gruppe oder einen anderen Empfänger für die Freigabe mit der [Einladen](../api/driveitem-invite.md)-Aktion dar.</span><span class="sxs-lookup"><span data-stu-id="d71b3-105">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d71b3-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d71b3-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d71b3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d71b3-107">Properties</span></span>
<span data-ttu-id="d71b3-108">Die Empfängerressource besitzt die folgenden Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="d71b3-108">The recipients resource has these properties.</span></span>

| <span data-ttu-id="d71b3-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d71b3-109">Property name</span></span> | <span data-ttu-id="d71b3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d71b3-110">Type</span></span>   | <span data-ttu-id="d71b3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d71b3-111">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d71b3-112">E-Mail</span><span class="sxs-lookup"><span data-stu-id="d71b3-112">email</span></span>         | <span data-ttu-id="d71b3-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d71b3-113">String</span></span> | <span data-ttu-id="d71b3-114">Die E-Mail-Adresse des Empfängers, wenn der Empfänger eine zugehörige E-Mail-Adresse aufweist.</span><span class="sxs-lookup"><span data-stu-id="d71b3-114">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="d71b3-115">Alias</span><span class="sxs-lookup"><span data-stu-id="d71b3-115">alias</span></span>         | <span data-ttu-id="d71b3-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d71b3-116">String</span></span> | <span data-ttu-id="d71b3-117">Der Alias des Domänenobjekts, für Fälle, in denen keine E-Mail-Adresse verfügbar ist (z. B. bei Sicherheitsgruppen).</span><span class="sxs-lookup"><span data-stu-id="d71b3-117">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="d71b3-118">objectId</span><span class="sxs-lookup"><span data-stu-id="d71b3-118">objectId</span></span>      | <span data-ttu-id="d71b3-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d71b3-119">String</span></span> | <span data-ttu-id="d71b3-120">Der eindeutige Bezeichner für den Empfänger im Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="d71b3-120">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="d71b3-121">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="d71b3-121">Remarks</span></span>

<span data-ttu-id="d71b3-p102">Bei Verwendung von [invite](../api/driveitem-invite.md) zum Hinzufügen von Berechtigungen kann im DriveRecipient **email**, **alias** oder **objectId** angegeben sein. Nur einer dieser Werte ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d71b3-p102">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
