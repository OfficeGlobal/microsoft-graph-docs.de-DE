---
title: Ressourcentyp educationSynchronizationDataProvider
description: 'SIS Quellschema darstellt. Dadurch wird das System wissen, wie Sie die eingehenden Daten das Schema Azure Active Directory (AD Azure) zuordnen. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515496"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="f7748-104">Ressourcentyp educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="f7748-104">educationSynchronizationDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7748-105">SIS Quellschema darstellt.</span><span class="sxs-lookup"><span data-stu-id="f7748-105">Represents the source SIS schema.</span></span> <span data-ttu-id="f7748-106">Dadurch wird das System wissen, wie Sie die eingehenden Daten das Schema Azure Active Directory (AD Azure) zuordnen.</span><span class="sxs-lookup"><span data-stu-id="f7748-106">This allows the system to know how to map the incoming data to the Azure Active Directory (Azure AD) schema.</span></span>

> <span data-ttu-id="f7748-107">**Hinweis:** Dieser komplexe Typ ist abstrakt.</span><span class="sxs-lookup"><span data-stu-id="f7748-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="f7748-108">Verweisen Sie auf bestimmten Typen von Datenprovidern aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="f7748-108">Refer to the specific types of data providers listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="f7748-109">Abgeleitete Typen</span><span class="sxs-lookup"><span data-stu-id="f7748-109">Derived types</span></span>
| <span data-ttu-id="f7748-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f7748-110">Type</span></span> | <span data-ttu-id="f7748-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7748-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="f7748-112">educationcsvdataprovider</span><span class="sxs-lookup"><span data-stu-id="f7748-112">educationcsvdataprovider</span></span>](educationcsvdataprovider.md) | <span data-ttu-id="f7748-113">Mit CSV-Dateien verwendet als Eingabe Quelle.</span><span class="sxs-lookup"><span data-stu-id="f7748-113">Used with CSV files as the input source.</span></span> |
| [<span data-ttu-id="f7748-114">educationpowerschooldataprovider</span><span class="sxs-lookup"><span data-stu-id="f7748-114">educationpowerschooldataprovider</span></span>](educationpowerschooldataprovider.md) | <span data-ttu-id="f7748-115">Mit PowerSchool verwendet als Eingabe Quelle.</span><span class="sxs-lookup"><span data-stu-id="f7748-115">Used with PowerSchool as the input source.</span></span> |
| [<span data-ttu-id="f7748-116">educationonerosterapidataprovider</span><span class="sxs-lookup"><span data-stu-id="f7748-116">educationonerosterapidataprovider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="f7748-117">Als Eingabe Quelle verwendet mit OneRoster-API.</span><span class="sxs-lookup"><span data-stu-id="f7748-117">Used with OneRoster API as the input source.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7748-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7748-118">Properties</span></span>

<span data-ttu-id="f7748-119">Keine Eigenschaften werden von diesem Typ verfügbar gemacht.</span><span class="sxs-lookup"><span data-stu-id="f7748-119">No properties are exposed by this type.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
