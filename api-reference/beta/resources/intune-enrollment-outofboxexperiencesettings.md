---
title: Ressourcentyp outOfBoxExperienceSettings
description: Erleben Sie die Einstellung im Lieferzustand
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af276dd520df9ee3b257650e703813de355bed9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882733"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="6a57a-103">Ressourcentyp outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="6a57a-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="6a57a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6a57a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a57a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a57a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a57a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6a57a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a57a-107">Erleben Sie die Einstellung im Lieferzustand</span><span class="sxs-lookup"><span data-stu-id="6a57a-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="6a57a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6a57a-108">Properties</span></span>
|<span data-ttu-id="6a57a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a57a-109">Property</span></span>|<span data-ttu-id="6a57a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6a57a-110">Type</span></span>|<span data-ttu-id="6a57a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a57a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a57a-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="6a57a-112">hidePrivacySettings</span></span>|<span data-ttu-id="6a57a-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a57a-113">Boolean</span></span>|<span data-ttu-id="6a57a-114">Zeigen Sie an oder blenden Sie der datenschutzeinstellungen für Benutzer aus</span><span class="sxs-lookup"><span data-stu-id="6a57a-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="6a57a-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="6a57a-115">hideEULA</span></span>|<span data-ttu-id="6a57a-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a57a-116">Boolean</span></span>|<span data-ttu-id="6a57a-117">Anzeigen oder Ausblenden der Endbenutzer-Lizenzvertrag für Benutzer</span><span class="sxs-lookup"><span data-stu-id="6a57a-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="6a57a-118">userType</span><span class="sxs-lookup"><span data-stu-id="6a57a-118">userType</span></span>|[<span data-ttu-id="6a57a-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="6a57a-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="6a57a-120">Typ des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6a57a-120">Type of user.</span></span> <span data-ttu-id="6a57a-121">Mögliche Werte sind: `administrator` und `standard`.</span><span class="sxs-lookup"><span data-stu-id="6a57a-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="6a57a-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="6a57a-122">deviceUsageType</span></span>|[<span data-ttu-id="6a57a-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="6a57a-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="6a57a-124">AAD Join-Authentifizierungstyp.</span><span class="sxs-lookup"><span data-stu-id="6a57a-124">AAD join authentication type.</span></span> <span data-ttu-id="6a57a-125">Mögliche Werte sind: `singleUser` und `shared`.</span><span class="sxs-lookup"><span data-stu-id="6a57a-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="6a57a-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="6a57a-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="6a57a-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a57a-127">Boolean</span></span>|<span data-ttu-id="6a57a-128">Wenn die Seite Set, und klicken Sie dann auf der Tastaturauswahl überspringen, wenn Sprache und Region festgelegt sind</span><span class="sxs-lookup"><span data-stu-id="6a57a-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="6a57a-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="6a57a-129">hideEscapeLink</span></span>|<span data-ttu-id="6a57a-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a57a-130">Boolean</span></span>|<span data-ttu-id="6a57a-131">Wenn auf True festgelegt, klicken Sie dann den Benutzer über mit anderen Konto auf Unternehmens-Anmeldung nicht gestartet werden kann</span><span class="sxs-lookup"><span data-stu-id="6a57a-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a57a-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6a57a-132">Relationships</span></span>
<span data-ttu-id="6a57a-133">Keine</span><span class="sxs-lookup"><span data-stu-id="6a57a-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6a57a-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6a57a-134">JSON Representation</span></span>
<span data-ttu-id="6a57a-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6a57a-135">Here is a JSON representation of the resource.</span></span>
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





