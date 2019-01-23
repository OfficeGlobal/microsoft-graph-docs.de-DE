---
title: Ressourcentyp outOfBoxExperienceSettings
description: Erleben Sie die Einstellung im Lieferzustand
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d2b48fef00c9c3a291a0a2fdfe680b9f4e21030
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404603"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="528a2-103">Ressourcentyp outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="528a2-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="528a2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="528a2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="528a2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="528a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="528a2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="528a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="528a2-107">Erleben Sie die Einstellung im Lieferzustand</span><span class="sxs-lookup"><span data-stu-id="528a2-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="528a2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="528a2-108">Properties</span></span>
|<span data-ttu-id="528a2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="528a2-109">Property</span></span>|<span data-ttu-id="528a2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="528a2-110">Type</span></span>|<span data-ttu-id="528a2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="528a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="528a2-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="528a2-112">hidePrivacySettings</span></span>|<span data-ttu-id="528a2-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="528a2-113">Boolean</span></span>|<span data-ttu-id="528a2-114">Zeigen Sie an oder blenden Sie der datenschutzeinstellungen für Benutzer aus</span><span class="sxs-lookup"><span data-stu-id="528a2-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="528a2-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="528a2-115">hideEULA</span></span>|<span data-ttu-id="528a2-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="528a2-116">Boolean</span></span>|<span data-ttu-id="528a2-117">Anzeigen oder Ausblenden der Endbenutzer-Lizenzvertrag für Benutzer</span><span class="sxs-lookup"><span data-stu-id="528a2-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="528a2-118">userType</span><span class="sxs-lookup"><span data-stu-id="528a2-118">userType</span></span>|[<span data-ttu-id="528a2-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="528a2-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="528a2-120">Typ des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="528a2-120">Type of user.</span></span> <span data-ttu-id="528a2-121">Mögliche Werte sind: `administrator` und `standard`.</span><span class="sxs-lookup"><span data-stu-id="528a2-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="528a2-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="528a2-122">deviceUsageType</span></span>|[<span data-ttu-id="528a2-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="528a2-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="528a2-124">AAD Join-Authentifizierungstyp.</span><span class="sxs-lookup"><span data-stu-id="528a2-124">AAD join authentication type.</span></span> <span data-ttu-id="528a2-125">Mögliche Werte sind: `singleUser` und `shared`.</span><span class="sxs-lookup"><span data-stu-id="528a2-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="528a2-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="528a2-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="528a2-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="528a2-127">Boolean</span></span>|<span data-ttu-id="528a2-128">Wenn die Seite Set, und klicken Sie dann auf der Tastaturauswahl überspringen, wenn Sprache und Region festgelegt sind</span><span class="sxs-lookup"><span data-stu-id="528a2-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="528a2-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="528a2-129">hideEscapeLink</span></span>|<span data-ttu-id="528a2-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="528a2-130">Boolean</span></span>|<span data-ttu-id="528a2-131">Wenn auf True festgelegt, klicken Sie dann den Benutzer über mit anderen Konto auf Unternehmens-Anmeldung nicht gestartet werden kann</span><span class="sxs-lookup"><span data-stu-id="528a2-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="528a2-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="528a2-132">Relationships</span></span>
<span data-ttu-id="528a2-133">Keine</span><span class="sxs-lookup"><span data-stu-id="528a2-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="528a2-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="528a2-134">JSON Representation</span></span>
<span data-ttu-id="528a2-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="528a2-135">Here is a JSON representation of the resource.</span></span>
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




