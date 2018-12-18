---
title: Ressourcentyp windowsEnrollmentStatusScreenSettings
description: Registrierung Status Bildschirm Einstellung
author: tfitzmac
ms.openlocfilehash: 8ccf2565d722a09de5f08ebe7333436729ce1b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346928"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="b5d41-103">Ressourcentyp windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="b5d41-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="b5d41-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b5d41-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5d41-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5d41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5d41-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5d41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5d41-107">Registrierung Status Bildschirm Einstellung</span><span class="sxs-lookup"><span data-stu-id="b5d41-107">Enrollment status screen setting</span></span>
## <a name="properties"></a><span data-ttu-id="b5d41-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5d41-108">Properties</span></span>
|<span data-ttu-id="b5d41-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5d41-109">Property</span></span>|<span data-ttu-id="b5d41-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b5d41-110">Type</span></span>|<span data-ttu-id="b5d41-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5d41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5d41-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="b5d41-112">hideInstallationProgress</span></span>|<span data-ttu-id="b5d41-113">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b5d41-113">Boolean</span></span>|<span data-ttu-id="b5d41-114">Zeigen Sie an oder blenden Sie des installationsfortschritts für Benutzer aus</span><span class="sxs-lookup"><span data-stu-id="b5d41-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="b5d41-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="b5d41-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="b5d41-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b5d41-116">Boolean</span></span>|<span data-ttu-id="b5d41-117">Zulassen Sie oder blockieren Sie Benutzer für die Verwendung von Gerät vor dem Profil- und app-Installation abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="b5d41-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="b5d41-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="b5d41-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="b5d41-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b5d41-119">Boolean</span></span>|<span data-ttu-id="b5d41-120">Ermöglicht es dem Benutzer, das von Setup auf Installationsfehler wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5d41-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="b5d41-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="b5d41-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="b5d41-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b5d41-122">Boolean</span></span>|<span data-ttu-id="b5d41-123">Zulassen Sie oder blockieren Sie Log-Auflistung auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="b5d41-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="b5d41-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="b5d41-124">customErrorMessage</span></span>|<span data-ttu-id="b5d41-125">String</span><span class="sxs-lookup"><span data-stu-id="b5d41-125">String</span></span>|<span data-ttu-id="b5d41-126">Legen Sie benutzerdefinierte Fehlermeldung nach einem Installationsfehler anzeigen</span><span class="sxs-lookup"><span data-stu-id="b5d41-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="b5d41-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b5d41-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="b5d41-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b5d41-128">Int32</span></span>|<span data-ttu-id="b5d41-129">Legen Sie die Installation des Fortschritts Timeout in Minuten</span><span class="sxs-lookup"><span data-stu-id="b5d41-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="b5d41-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="b5d41-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="b5d41-131">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b5d41-131">Boolean</span></span>|<span data-ttu-id="b5d41-132">Ermöglicht es dem Benutzer weiterhin verwenden das Gerät auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="b5d41-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5d41-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b5d41-133">Relationships</span></span>
<span data-ttu-id="b5d41-134">Keine</span><span class="sxs-lookup"><span data-stu-id="b5d41-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5d41-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b5d41-135">JSON Representation</span></span>
<span data-ttu-id="b5d41-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b5d41-136">Here is a JSON representation of the resource.</span></span>
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





