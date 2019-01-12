---
title: Ressourcentyp educationFileSynchronizationVerificationMessage
description: Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum Starten der Synchronisierung für die CSV-basierte Schule datenprofile zurückgegeben. Die Ressource wird Fehler enthalten, die aus der Überprüfung. Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cda1d5d3ac56c50cdeb94ada091e8ae2975b8813
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914479"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="b1c9d-105">Ressourcentyp educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="b1c9d-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="b1c9d-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1c9d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1c9d-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1c9d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1c9d-108">Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum [Starten Sie die Synchronisierung](../api/educationsynchronizationprofile-start.md) für Schule CSV-basierte datenprofile zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1c9d-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="b1c9d-109">Die Ressource wird Fehler enthalten, die aus der Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="b1c9d-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="b1c9d-110">Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.</span><span class="sxs-lookup"><span data-stu-id="b1c9d-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="b1c9d-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b1c9d-111">Properties</span></span>

| <span data-ttu-id="b1c9d-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1c9d-112">Property</span></span> | <span data-ttu-id="b1c9d-113">Typ</span><span class="sxs-lookup"><span data-stu-id="b1c9d-113">Type</span></span> | <span data-ttu-id="b1c9d-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1c9d-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b1c9d-115">**type**</span><span class="sxs-lookup"><span data-stu-id="b1c9d-115">**type**</span></span> | <span data-ttu-id="b1c9d-116">string</span><span class="sxs-lookup"><span data-stu-id="b1c9d-116">string</span></span> | <span data-ttu-id="b1c9d-117">Typ der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="b1c9d-117">Type of the message.</span></span> <span data-ttu-id="b1c9d-118">Mögliche Werte sind: `error`, `warning` und `information`.</span><span class="sxs-lookup"><span data-stu-id="b1c9d-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="b1c9d-119">**Dateiname**</span><span class="sxs-lookup"><span data-stu-id="b1c9d-119">**filename**</span></span> | <span data-ttu-id="b1c9d-120">string</span><span class="sxs-lookup"><span data-stu-id="b1c9d-120">string</span></span> | <span data-ttu-id="b1c9d-121">Quelldatei, die den Fehler enthält.</span><span class="sxs-lookup"><span data-stu-id="b1c9d-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="b1c9d-122">**description**</span><span class="sxs-lookup"><span data-stu-id="b1c9d-122">**description**</span></span> | <span data-ttu-id="b1c9d-123">string</span><span class="sxs-lookup"><span data-stu-id="b1c9d-123">string</span></span> | <span data-ttu-id="b1c9d-124">Ausführliche Informationen zu den Nachrichtentyp.</span><span class="sxs-lookup"><span data-stu-id="b1c9d-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b1c9d-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b1c9d-125">JSON representation</span></span>

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
