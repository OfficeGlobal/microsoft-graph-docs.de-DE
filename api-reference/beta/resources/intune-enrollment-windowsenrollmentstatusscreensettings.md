---
title: windowsEnrollmentStatusScreenSettings-Ressourcentyp
description: Einstellung für den Registrierungsstatus
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5684a447b82f285784eda1bf71c13f35d766a570
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148685"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="fe509-103">windowsEnrollmentStatusScreenSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fe509-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="fe509-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe509-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe509-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fe509-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe509-106">Einstellung für den Registrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="fe509-106">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="fe509-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fe509-107">Properties</span></span>
|<span data-ttu-id="fe509-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fe509-108">Property</span></span>|<span data-ttu-id="fe509-109">Typ</span><span class="sxs-lookup"><span data-stu-id="fe509-109">Type</span></span>|<span data-ttu-id="fe509-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe509-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe509-111">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="fe509-111">hideInstallationProgress</span></span>|<span data-ttu-id="fe509-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fe509-112">Boolean</span></span>|<span data-ttu-id="fe509-113">Anzeigen oder Ausblenden des Installationsfortschritts für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="fe509-113">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="fe509-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="fe509-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="fe509-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fe509-115">Boolean</span></span>|<span data-ttu-id="fe509-116">Zulassen oder Blockieren des Benutzergeräts vor der vollständigen Profil-und App-Installation</span><span class="sxs-lookup"><span data-stu-id="fe509-116">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="fe509-117">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="fe509-117">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="fe509-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fe509-118">Boolean</span></span>|<span data-ttu-id="fe509-119">Wiederholen des Setups bei Installationsfehlers für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="fe509-119">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="fe509-120">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="fe509-120">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="fe509-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fe509-121">Boolean</span></span>|<span data-ttu-id="fe509-122">Zulassen oder Blockieren der Protokollsammlung bei Installations Ausfällen</span><span class="sxs-lookup"><span data-stu-id="fe509-122">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="fe509-123">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="fe509-123">customErrorMessage</span></span>|<span data-ttu-id="fe509-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe509-124">String</span></span>|<span data-ttu-id="fe509-125">Festlegen der benutzerdefinierten Fehlermeldung beim Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="fe509-125">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="fe509-126">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="fe509-126">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="fe509-127">Int32</span><span class="sxs-lookup"><span data-stu-id="fe509-127">Int32</span></span>|<span data-ttu-id="fe509-128">Festlegen des Installationsfortschritts-Timeouts in Minuten</span><span class="sxs-lookup"><span data-stu-id="fe509-128">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="fe509-129">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="fe509-129">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="fe509-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fe509-130">Boolean</span></span>|<span data-ttu-id="fe509-131">Zulassen, dass der Benutzer das Gerät bei der Installation weiterhin verwendet</span><span class="sxs-lookup"><span data-stu-id="fe509-131">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe509-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fe509-132">Relationships</span></span>
<span data-ttu-id="fe509-133">Keine</span><span class="sxs-lookup"><span data-stu-id="fe509-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe509-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fe509-134">JSON Representation</span></span>
<span data-ttu-id="fe509-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fe509-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```




