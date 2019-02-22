---
title: Dem outofboxexperiencesettings-Ressourcentyp
description: Einstellung für die Out-of-Box-Erfahrung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1148ba609a6533dcc6cedb9abd50e9191dceb5d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145528"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="35596-103">Dem outofboxexperiencesettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="35596-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="35596-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35596-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35596-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="35596-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35596-106">Einstellung für die Out-of-Box-Erfahrung</span><span class="sxs-lookup"><span data-stu-id="35596-106">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="35596-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="35596-107">Properties</span></span>
|<span data-ttu-id="35596-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35596-108">Property</span></span>|<span data-ttu-id="35596-109">Typ</span><span class="sxs-lookup"><span data-stu-id="35596-109">Type</span></span>|<span data-ttu-id="35596-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35596-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35596-111">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="35596-111">hidePrivacySettings</span></span>|<span data-ttu-id="35596-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="35596-112">Boolean</span></span>|<span data-ttu-id="35596-113">Ein-oder Ausblenden von Datenschutzeinstellungen für Benutzer</span><span class="sxs-lookup"><span data-stu-id="35596-113">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="35596-114">hideEULA</span><span class="sxs-lookup"><span data-stu-id="35596-114">hideEULA</span></span>|<span data-ttu-id="35596-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="35596-115">Boolean</span></span>|<span data-ttu-id="35596-116">Ein-oder Ausblenden des EULAs für Benutzer</span><span class="sxs-lookup"><span data-stu-id="35596-116">Show or hide EULA to user</span></span>|
|<span data-ttu-id="35596-117">userType</span><span class="sxs-lookup"><span data-stu-id="35596-117">userType</span></span>|[<span data-ttu-id="35596-118">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="35596-118">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="35596-119">Benutzertyp.</span><span class="sxs-lookup"><span data-stu-id="35596-119">Type of user.</span></span> <span data-ttu-id="35596-120">Mögliche Werte sind: `administrator` und `standard`.</span><span class="sxs-lookup"><span data-stu-id="35596-120">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="35596-121">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="35596-121">deviceUsageType</span></span>|[<span data-ttu-id="35596-122">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="35596-122">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="35596-123">AAD-Join-Authentifizierungstyp.</span><span class="sxs-lookup"><span data-stu-id="35596-123">AAD join authentication type.</span></span> <span data-ttu-id="35596-124">Mögliche Werte sind: `singleUser` und `shared`.</span><span class="sxs-lookup"><span data-stu-id="35596-124">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="35596-125">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="35596-125">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="35596-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="35596-126">Boolean</span></span>|<span data-ttu-id="35596-127">Wenn diese Einstellung festgelegt ist, überspringen Sie die Seite mit der Tastaturauswahl, wenn Sprache und Region festgelegt sind.</span><span class="sxs-lookup"><span data-stu-id="35596-127">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="35596-128">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="35596-128">hideEscapeLink</span></span>|<span data-ttu-id="35596-129">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="35596-129">Boolean</span></span>|<span data-ttu-id="35596-130">Wenn dieser Wert auf "true" festgelegt ist, kann der Benutzer nicht mit einem anderen Konto als bei der Unternehmensanmeldung beginnen.</span><span class="sxs-lookup"><span data-stu-id="35596-130">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="35596-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="35596-131">Relationships</span></span>
<span data-ttu-id="35596-132">Keine</span><span class="sxs-lookup"><span data-stu-id="35596-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35596-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="35596-133">JSON Representation</span></span>
<span data-ttu-id="35596-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="35596-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```




