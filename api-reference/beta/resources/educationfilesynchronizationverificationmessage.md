---
title: Ressourcentyp educationFileSynchronizationVerificationMessage
description: Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum Starten der Synchronisierung für die CSV-basierte Schule datenprofile zurückgegeben. Die Ressource wird Fehler enthalten, die aus der Überprüfung. Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529894"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="c2070-105">Ressourcentyp educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="c2070-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2070-106">Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum [Starten Sie die Synchronisierung](../api/educationsynchronizationprofile-start.md) für Schule CSV-basierte datenprofile zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2070-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="c2070-107">Die Ressource wird Fehler enthalten, die aus der Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="c2070-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="c2070-108">Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.</span><span class="sxs-lookup"><span data-stu-id="c2070-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="c2070-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c2070-109">Properties</span></span>

| <span data-ttu-id="c2070-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c2070-110">Property</span></span> | <span data-ttu-id="c2070-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c2070-111">Type</span></span> | <span data-ttu-id="c2070-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2070-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c2070-113">**type**</span><span class="sxs-lookup"><span data-stu-id="c2070-113">**type**</span></span> | <span data-ttu-id="c2070-114">string</span><span class="sxs-lookup"><span data-stu-id="c2070-114">string</span></span> | <span data-ttu-id="c2070-115">Typ der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="c2070-115">Type of the message.</span></span> <span data-ttu-id="c2070-116">Mögliche Werte sind: `error`, `warning` und `information`.</span><span class="sxs-lookup"><span data-stu-id="c2070-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="c2070-117">**fileName**</span><span class="sxs-lookup"><span data-stu-id="c2070-117">**filename**</span></span> | <span data-ttu-id="c2070-118">string</span><span class="sxs-lookup"><span data-stu-id="c2070-118">string</span></span> | <span data-ttu-id="c2070-119">Quelldatei, die den Fehler enthält.</span><span class="sxs-lookup"><span data-stu-id="c2070-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="c2070-120">**description**</span><span class="sxs-lookup"><span data-stu-id="c2070-120">**description**</span></span> | <span data-ttu-id="c2070-121">string</span><span class="sxs-lookup"><span data-stu-id="c2070-121">string</span></span> | <span data-ttu-id="c2070-122">Ausführliche Informationen zu den Nachrichtentyp.</span><span class="sxs-lookup"><span data-stu-id="c2070-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c2070-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c2070-123">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfilesynchronizationverificationmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
