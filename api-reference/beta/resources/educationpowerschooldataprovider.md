---
title: EducationPowerSchoolDataProvider-Ressource
description: Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn PowerSchool als Eingabe Quelle verwendet wird.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510463"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="87637-103">EducationPowerSchoolDataProvider-Ressource</span><span class="sxs-lookup"><span data-stu-id="87637-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87637-104">Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) als Eingabe Quelle verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="87637-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="87637-105">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="87637-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="87637-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="87637-106">Properties</span></span>

| <span data-ttu-id="87637-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87637-107">Property</span></span> | <span data-ttu-id="87637-108">Typ</span><span class="sxs-lookup"><span data-stu-id="87637-108">Type</span></span> | <span data-ttu-id="87637-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87637-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="87637-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="87637-110">**connectionUrl**</span></span> | <span data-ttu-id="87637-111">String</span><span class="sxs-lookup"><span data-stu-id="87637-111">String</span></span> | <span data-ttu-id="87637-112">Die Verbindungs-URL für die PowerSchool-Instanz.</span><span class="sxs-lookup"><span data-stu-id="87637-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="87637-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="87637-113">**clientId**</span></span> | <span data-ttu-id="87637-114">String</span><span class="sxs-lookup"><span data-stu-id="87637-114">String</span></span> |  <span data-ttu-id="87637-115">Die Client-ID, die zum Verbinden mit PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="87637-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="87637-116">client_secret</span><span class="sxs-lookup"><span data-stu-id="87637-116">**clientSecret**</span></span> | <span data-ttu-id="87637-117">String</span><span class="sxs-lookup"><span data-stu-id="87637-117">String</span></span> |  <span data-ttu-id="87637-118">Der geheime Clientschlüssel zum Authentifizieren der Verbindungs zu der Instanz PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="87637-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="87637-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="87637-119">**schoolsIds**</span></span> | <span data-ttu-id="87637-120">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="87637-120">String collection</span></span> |  <span data-ttu-id="87637-121">Die Liste der Schulen synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="87637-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="87637-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="87637-122">**schoolYear**</span></span> | <span data-ttu-id="87637-123">String</span><span class="sxs-lookup"><span data-stu-id="87637-123">String</span></span> |  <span data-ttu-id="87637-124">Das Jahr Schule synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="87637-124">The school year to sync.</span></span> |
| <span data-ttu-id="87637-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="87637-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="87637-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="87637-126">Boolean</span></span> |  <span data-ttu-id="87637-127">Gibt an, ob die Quelle mehrere Bezeichner für eine einzelne Student oder Lehrer verfügt.</span><span class="sxs-lookup"><span data-stu-id="87637-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="87637-128">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="87637-128">**customizations**</span></span> | [<span data-ttu-id="87637-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="87637-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="87637-130">Optional Anpassung der Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="87637-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87637-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="87637-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerschooldataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
