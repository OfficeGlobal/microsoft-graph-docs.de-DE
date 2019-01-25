---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ecf3e600cc943d0c82da38928d8018e6c654fb4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525801"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="8dc17-102">DriveRecipient-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8dc17-102">DriveRecipient resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dc17-103">Die **DriveRecipient**-Ressource stellt eine Person, eine Gruppe oder einen anderen Empfänger für die Freigabe mit der [Einladen](../api/driveitem-invite.md)-Aktion dar.</span><span class="sxs-lookup"><span data-stu-id="8dc17-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dc17-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8dc17-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8dc17-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8dc17-105">Properties</span></span>
<span data-ttu-id="8dc17-106">Die Empfängerressource besitzt die folgenden Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="8dc17-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="8dc17-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="8dc17-107">Property name</span></span> | <span data-ttu-id="8dc17-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8dc17-108">Type</span></span>   | <span data-ttu-id="8dc17-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dc17-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8dc17-110">E-Mail</span><span class="sxs-lookup"><span data-stu-id="8dc17-110">email</span></span>         | <span data-ttu-id="8dc17-111">String</span><span class="sxs-lookup"><span data-stu-id="8dc17-111">String</span></span> | <span data-ttu-id="8dc17-112">Die E-Mail-Adresse des Empfängers, wenn der Empfänger eine zugehörige E-Mail-Adresse aufweist.</span><span class="sxs-lookup"><span data-stu-id="8dc17-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="8dc17-113">Alias</span><span class="sxs-lookup"><span data-stu-id="8dc17-113">alias</span></span>         | <span data-ttu-id="8dc17-114">String</span><span class="sxs-lookup"><span data-stu-id="8dc17-114">String</span></span> | <span data-ttu-id="8dc17-115">Der Alias des Domänenobjekts, für Fälle, in denen keine E-Mail-Adresse verfügbar ist (z. B. bei Sicherheitsgruppen).</span><span class="sxs-lookup"><span data-stu-id="8dc17-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="8dc17-116">objectId</span><span class="sxs-lookup"><span data-stu-id="8dc17-116">objectId</span></span>      | <span data-ttu-id="8dc17-117">String</span><span class="sxs-lookup"><span data-stu-id="8dc17-117">String</span></span> | <span data-ttu-id="8dc17-118">Der eindeutige Bezeichner für den Empfänger im Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="8dc17-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="8dc17-119">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="8dc17-119">Remarks</span></span>

<span data-ttu-id="8dc17-p101">Bei Verwendung von [invite](../api/driveitem-invite.md) zum Hinzufügen von Berechtigungen kann im DriveRecipient **email**, **alias** oder **objectId** angegeben sein. Nur einer dieser Werte ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8dc17-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": [
    "Error: /api-reference/beta/resources/driverecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
