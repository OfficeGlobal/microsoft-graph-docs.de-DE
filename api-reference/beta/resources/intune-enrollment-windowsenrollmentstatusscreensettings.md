---
title: Ressourcentyp windowsEnrollmentStatusScreenSettings
description: Registrierung Status Bildschirm Einstellung
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ffb2827988b80b4d6563d8a92c9ccea7ac9828
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399934"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="13f9a-103">Ressourcentyp windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="13f9a-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="13f9a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="13f9a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13f9a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13f9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13f9a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13f9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13f9a-107">Registrierung Status Bildschirm Einstellung</span><span class="sxs-lookup"><span data-stu-id="13f9a-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="13f9a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13f9a-108">Properties</span></span>
|<span data-ttu-id="13f9a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13f9a-109">Property</span></span>|<span data-ttu-id="13f9a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="13f9a-110">Type</span></span>|<span data-ttu-id="13f9a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13f9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13f9a-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="13f9a-112">hideInstallationProgress</span></span>|<span data-ttu-id="13f9a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f9a-113">Boolean</span></span>|<span data-ttu-id="13f9a-114">Zeigen Sie an oder blenden Sie des installationsfortschritts für Benutzer aus</span><span class="sxs-lookup"><span data-stu-id="13f9a-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="13f9a-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="13f9a-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="13f9a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f9a-116">Boolean</span></span>|<span data-ttu-id="13f9a-117">Zulassen Sie oder blockieren Sie Benutzer für die Verwendung von Gerät vor dem Profil- und app-Installation abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="13f9a-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="13f9a-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="13f9a-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="13f9a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f9a-119">Boolean</span></span>|<span data-ttu-id="13f9a-120">Ermöglicht es dem Benutzer, das von Setup auf Installationsfehler wiederholen</span><span class="sxs-lookup"><span data-stu-id="13f9a-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="13f9a-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="13f9a-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="13f9a-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f9a-122">Boolean</span></span>|<span data-ttu-id="13f9a-123">Zulassen Sie oder blockieren Sie Log-Auflistung auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="13f9a-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="13f9a-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="13f9a-124">customErrorMessage</span></span>|<span data-ttu-id="13f9a-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13f9a-125">String</span></span>|<span data-ttu-id="13f9a-126">Legen Sie benutzerdefinierte Fehlermeldung nach einem Installationsfehler anzeigen</span><span class="sxs-lookup"><span data-stu-id="13f9a-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="13f9a-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="13f9a-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="13f9a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="13f9a-128">Int32</span></span>|<span data-ttu-id="13f9a-129">Legen Sie die Installation des Fortschritts Timeout in Minuten</span><span class="sxs-lookup"><span data-stu-id="13f9a-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="13f9a-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="13f9a-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="13f9a-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f9a-131">Boolean</span></span>|<span data-ttu-id="13f9a-132">Ermöglicht es dem Benutzer weiterhin verwenden das Gerät auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="13f9a-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="13f9a-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="13f9a-133">Relationships</span></span>
<span data-ttu-id="13f9a-134">Keine</span><span class="sxs-lookup"><span data-stu-id="13f9a-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13f9a-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13f9a-135">JSON Representation</span></span>
<span data-ttu-id="13f9a-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13f9a-136">Here is a JSON representation of the resource.</span></span>
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




