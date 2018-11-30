---
title: Ressourcentyp educationFileSynchronizationVerificationMessage
description: Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum Starten der Synchronisierung für die CSV-basierte Schule datenprofile zurückgegeben. Die Ressource wird Fehler enthalten, die aus der Überprüfung. Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.
ms.openlocfilehash: cf685e0619c5600340df68ba86ecaef11a8a435d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058527"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="49239-105">Ressourcentyp educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="49239-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="49239-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="49239-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49239-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49239-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49239-108">Stellt einen Fehler an den Client als Antwort auf eine Anforderung zum [Starten Sie die Synchronisierung](../api/educationsynchronizationprofile-start.md) für Schule CSV-basierte datenprofile zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49239-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="49239-109">Die Ressource wird Fehler enthalten, die aus der Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="49239-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="49239-110">Benutzer müssen die Quelldaten beheben, bevor Sie die Anforderung für die Synchronisierung mit Azure Active Directory (AD Azure) neu starten.</span><span class="sxs-lookup"><span data-stu-id="49239-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="49239-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="49239-111">Properties</span></span>

| <span data-ttu-id="49239-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49239-112">Property</span></span> | <span data-ttu-id="49239-113">Typ</span><span class="sxs-lookup"><span data-stu-id="49239-113">Type</span></span> | <span data-ttu-id="49239-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49239-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="49239-115">**type**</span><span class="sxs-lookup"><span data-stu-id="49239-115">**type**</span></span> | <span data-ttu-id="49239-116">string</span><span class="sxs-lookup"><span data-stu-id="49239-116">string</span></span> | <span data-ttu-id="49239-117">Typ der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="49239-117">Type of the message.</span></span> <span data-ttu-id="49239-118">Mögliche Werte sind: `error`, `warning` und `information`.</span><span class="sxs-lookup"><span data-stu-id="49239-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="49239-119">**Dateiname**</span><span class="sxs-lookup"><span data-stu-id="49239-119">**filename**</span></span> | <span data-ttu-id="49239-120">string</span><span class="sxs-lookup"><span data-stu-id="49239-120">string</span></span> | <span data-ttu-id="49239-121">Quelldatei, die den Fehler enthält.</span><span class="sxs-lookup"><span data-stu-id="49239-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="49239-122">**description**</span><span class="sxs-lookup"><span data-stu-id="49239-122">**description**</span></span> | <span data-ttu-id="49239-123">string</span><span class="sxs-lookup"><span data-stu-id="49239-123">string</span></span> | <span data-ttu-id="49239-124">Ausführliche Informationen zu den Nachrichtentyp.</span><span class="sxs-lookup"><span data-stu-id="49239-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="49239-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="49239-125">JSON representation</span></span>

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