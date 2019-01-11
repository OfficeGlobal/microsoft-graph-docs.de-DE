---
title: Ressourcentyp educationFileSynchronizationVerificationMessage
description: Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum Starten der Synchronisierung für die CSV-basierte Schule datenprofile zurückgegeben. Die Ressource wird Fehler enthalten, die aus der Überprüfung. Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: ae09ec3f208adfee64a6392db9732841fc7a0808
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845514"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="9da92-105">Ressourcentyp educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="9da92-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="9da92-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9da92-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9da92-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9da92-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9da92-108">Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum [Starten Sie die Synchronisierung](../api/educationsynchronizationprofile-start.md) für Schule CSV-basierte datenprofile zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9da92-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="9da92-109">Die Ressource wird Fehler enthalten, die aus der Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="9da92-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="9da92-110">Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.</span><span class="sxs-lookup"><span data-stu-id="9da92-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="9da92-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9da92-111">Properties</span></span>

| <span data-ttu-id="9da92-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9da92-112">Property</span></span> | <span data-ttu-id="9da92-113">Typ</span><span class="sxs-lookup"><span data-stu-id="9da92-113">Type</span></span> | <span data-ttu-id="9da92-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9da92-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="9da92-115">**type**</span><span class="sxs-lookup"><span data-stu-id="9da92-115">**type**</span></span> | <span data-ttu-id="9da92-116">string</span><span class="sxs-lookup"><span data-stu-id="9da92-116">string</span></span> | <span data-ttu-id="9da92-117">Typ der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="9da92-117">Type of the message.</span></span> <span data-ttu-id="9da92-118">Mögliche Werte sind: `error`, `warning` und `information`.</span><span class="sxs-lookup"><span data-stu-id="9da92-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="9da92-119">**Dateiname**</span><span class="sxs-lookup"><span data-stu-id="9da92-119">**filename**</span></span> | <span data-ttu-id="9da92-120">string</span><span class="sxs-lookup"><span data-stu-id="9da92-120">string</span></span> | <span data-ttu-id="9da92-121">Quelldatei, die den Fehler enthält.</span><span class="sxs-lookup"><span data-stu-id="9da92-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="9da92-122">**description**</span><span class="sxs-lookup"><span data-stu-id="9da92-122">**description**</span></span> | <span data-ttu-id="9da92-123">string</span><span class="sxs-lookup"><span data-stu-id="9da92-123">string</span></span> | <span data-ttu-id="9da92-124">Ausführliche Informationen zu den Nachrichtentyp.</span><span class="sxs-lookup"><span data-stu-id="9da92-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9da92-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9da92-125">JSON representation</span></span>

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
