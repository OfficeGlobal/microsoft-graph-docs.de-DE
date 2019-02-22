---
title: reportRoot-Ressourcentyp
description: Die Ressource, die eine Instanz eines Geräts oder Problem Behandlungs Berichts darstellt, je nach Kontext.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a2e41d9b17ca7acafa98dad65db5d2ff5ce30925
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151296"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="6ba09-103">reportRoot-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6ba09-103">reportRoot resource type</span></span>

> <span data-ttu-id="6ba09-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ba09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ba09-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6ba09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ba09-106">Die Ressource, die eine Instanz eines Geräts oder Problem Behandlungs Berichts darstellt, je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="6ba09-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="6ba09-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="6ba09-107">Methods</span></span>
|<span data-ttu-id="6ba09-108">Methode</span><span class="sxs-lookup"><span data-stu-id="6ba09-108">Method</span></span>|<span data-ttu-id="6ba09-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6ba09-109">Return Type</span></span>|<span data-ttu-id="6ba09-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ba09-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ba09-111">reportRoot abrufen</span><span class="sxs-lookup"><span data-stu-id="6ba09-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="6ba09-112">Lesen von Eigenschaften und Beziehungen des [reportRoot](../resources/intune-shared-reportroot.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ba09-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="6ba09-113">reportRoot aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6ba09-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="6ba09-114">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="6ba09-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="6ba09-115">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="6ba09-115">**Device configuration**</span></span>|
|[<span data-ttu-id="6ba09-116">deviceConfigurationUserActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="6ba09-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="6ba09-117">Metadaten für den Gerätekonfigurations-Benutzeraktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="6ba09-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="6ba09-118">deviceConfigurationDeviceActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="6ba09-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="6ba09-119">Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="6ba09-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="6ba09-120">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="6ba09-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="6ba09-121">managedDeviceEnrollmentAbandonmentDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="6ba09-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="6ba09-122">report</span><span class="sxs-lookup"><span data-stu-id="6ba09-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="6ba09-123">Metadaten für den Bericht über Registrierungs Verzichts Details</span><span class="sxs-lookup"><span data-stu-id="6ba09-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="6ba09-124">managedDeviceEnrollmentAbandonmentSummary-Funktion</span><span class="sxs-lookup"><span data-stu-id="6ba09-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="6ba09-125">report</span><span class="sxs-lookup"><span data-stu-id="6ba09-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="6ba09-126">Zusammenfassungsbericht zu Metadaten für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="6ba09-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="6ba09-127">managedDeviceEnrollmentFailureDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="6ba09-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="6ba09-128">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6ba09-128">Not yet documented</span></span>|
|[<span data-ttu-id="6ba09-129">managedDeviceEnrollmentFailureTrends-Funktion</span><span class="sxs-lookup"><span data-stu-id="6ba09-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="6ba09-130">Metadaten für den Bericht über Registrierungs Fehlermeldungen</span><span class="sxs-lookup"><span data-stu-id="6ba09-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="6ba09-131">managedDeviceEnrollmentTopFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="6ba09-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="6ba09-132">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6ba09-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6ba09-133">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ba09-133">Properties</span></span>
|<span data-ttu-id="6ba09-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ba09-134">Property</span></span>|<span data-ttu-id="6ba09-135">Typ</span><span class="sxs-lookup"><span data-stu-id="6ba09-135">Type</span></span>|<span data-ttu-id="6ba09-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ba09-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ba09-137">id</span><span class="sxs-lookup"><span data-stu-id="6ba09-137">id</span></span>|<span data-ttu-id="6ba09-138">String</span><span class="sxs-lookup"><span data-stu-id="6ba09-138">String</span></span>|<span data-ttu-id="6ba09-139">Der eindeutige Bezeichner für die Entität.</span><span class="sxs-lookup"><span data-stu-id="6ba09-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ba09-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ba09-140">Relationships</span></span>
<span data-ttu-id="6ba09-141">Keine</span><span class="sxs-lookup"><span data-stu-id="6ba09-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ba09-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ba09-142">JSON Representation</span></span>
<span data-ttu-id="6ba09-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ba09-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



