---
title: EducationPowerSchoolDataProvider-Ressource
description: Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn PowerSchool als Eingabe Quelle verwendet wird.
author: mmast-msft
ms.openlocfilehash: 714866d03c70aae8ea03a27b63fb3efbb4fa5ba4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312803"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="d7d7b-103">EducationPowerSchoolDataProvider-Ressource</span><span class="sxs-lookup"><span data-stu-id="d7d7b-103">educationPowerSchoolDataProvider resource</span></span>

> <span data-ttu-id="d7d7b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7d7b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7d7b-106">Verwendet, um die Synchronisierung Schule Datenprofil einrichten, wenn [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) als Eingabe Quelle verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-106">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="d7d7b-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d7d7b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d7d7b-108">Properties</span></span>

| <span data-ttu-id="d7d7b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d7d7b-109">Property</span></span> | <span data-ttu-id="d7d7b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d7d7b-110">Type</span></span> | <span data-ttu-id="d7d7b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7d7b-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d7d7b-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="d7d7b-112">**connectionUrl**</span></span> | <span data-ttu-id="d7d7b-113">String</span><span class="sxs-lookup"><span data-stu-id="d7d7b-113">String</span></span> | <span data-ttu-id="d7d7b-114">Die Verbindungs-URL für die PowerSchool-Instanz.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-114">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="d7d7b-115">**clientId**</span><span class="sxs-lookup"><span data-stu-id="d7d7b-115">**clientId**</span></span> | <span data-ttu-id="d7d7b-116">String</span><span class="sxs-lookup"><span data-stu-id="d7d7b-116">String</span></span> |  <span data-ttu-id="d7d7b-117">Die Client-ID, die zum Verbinden mit PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-117">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="d7d7b-118">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="d7d7b-118">**clientSecret**</span></span> | <span data-ttu-id="d7d7b-119">String</span><span class="sxs-lookup"><span data-stu-id="d7d7b-119">String</span></span> |  <span data-ttu-id="d7d7b-120">Der geheime Clientschlüssel zum Authentifizieren der Verbindungs zu der Instanz PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-120">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="d7d7b-121">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="d7d7b-121">**schoolsIds**</span></span> | <span data-ttu-id="d7d7b-122">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d7d7b-122">String collection</span></span> |  <span data-ttu-id="d7d7b-123">Die Liste der Schulen synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-123">The list of schools to sync.</span></span> |
| <span data-ttu-id="d7d7b-124">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="d7d7b-124">**schoolYear**</span></span> | <span data-ttu-id="d7d7b-125">String</span><span class="sxs-lookup"><span data-stu-id="d7d7b-125">String</span></span> |  <span data-ttu-id="d7d7b-126">Das Jahr Schule synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-126">The school year to sync.</span></span> |
| <span data-ttu-id="d7d7b-127">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="d7d7b-127">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="d7d7b-128">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d7d7b-128">Boolean</span></span> |  <span data-ttu-id="d7d7b-129">Gibt an, ob die Quelle mehrere Bezeichner für eine einzelne Student oder Lehrer verfügt.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-129">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="d7d7b-130">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="d7d7b-130">**customizations**</span></span> | [<span data-ttu-id="d7d7b-131">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="d7d7b-131">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="d7d7b-132">Optional Anpassung der Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d7d7b-132">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7d7b-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d7d7b-133">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
