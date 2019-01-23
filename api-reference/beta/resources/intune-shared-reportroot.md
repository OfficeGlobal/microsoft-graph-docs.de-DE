---
title: reportRoot-Ressourcentyp
description: Die Ressource, die eine Instanz eines Geräts oder zur Problembehandlung Bericht, je nach Kontext darstellt.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 378f1758773bfcffda5d9039d3b60d4ac4bd5cc5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421333"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="f5582-103">reportRoot-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f5582-103">reportRoot resource type</span></span>

> <span data-ttu-id="f5582-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f5582-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5582-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5582-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5582-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5582-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5582-107">Die Ressource, die eine Instanz eines Geräts oder zur Problembehandlung Bericht, je nach Kontext darstellt.</span><span class="sxs-lookup"><span data-stu-id="f5582-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="f5582-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="f5582-108">Methods</span></span>
|<span data-ttu-id="f5582-109">Methode</span><span class="sxs-lookup"><span data-stu-id="f5582-109">Method</span></span>|<span data-ttu-id="f5582-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f5582-110">Return Type</span></span>|<span data-ttu-id="f5582-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5582-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f5582-112">reportRoot abrufen</span><span class="sxs-lookup"><span data-stu-id="f5582-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="f5582-113">Lesen von Eigenschaften und Beziehungen des [reportRoot](../resources/intune-shared-reportroot.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f5582-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="f5582-114">reportRoot aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f5582-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="f5582-115">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="f5582-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="f5582-116">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="f5582-116">**Device configuration**</span></span>|
|[<span data-ttu-id="f5582-117">deviceConfigurationUserActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="f5582-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="f5582-118">Metadaten für den Gerätekonfigurations-Benutzeraktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="f5582-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="f5582-119">deviceConfigurationDeviceActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="f5582-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="f5582-120">Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="f5582-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="f5582-121">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="f5582-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="f5582-122">ManagedDeviceEnrollmentAbandonmentDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="f5582-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="f5582-123">report</span><span class="sxs-lookup"><span data-stu-id="f5582-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="f5582-124">Metadaten für die Registrierung Aufgabe Detailbericht</span><span class="sxs-lookup"><span data-stu-id="f5582-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="f5582-125">ManagedDeviceEnrollmentAbandonmentSummary-Funktion</span><span class="sxs-lookup"><span data-stu-id="f5582-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="f5582-126">report</span><span class="sxs-lookup"><span data-stu-id="f5582-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="f5582-127">Metadaten für die Registrierung Aufgabe Zusammenfassungsbericht</span><span class="sxs-lookup"><span data-stu-id="f5582-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="f5582-128">ManagedDeviceEnrollmentFailureDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="f5582-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="f5582-129">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f5582-129">Not yet documented</span></span>|
|[<span data-ttu-id="f5582-130">ManagedDeviceEnrollmentFailureTrends-Funktion</span><span class="sxs-lookup"><span data-stu-id="f5582-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="f5582-131">Metadaten für die Registrierung Trends Fehlerbericht</span><span class="sxs-lookup"><span data-stu-id="f5582-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="f5582-132">ManagedDeviceEnrollmentTopFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="f5582-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="f5582-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f5582-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f5582-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f5582-134">Properties</span></span>
|<span data-ttu-id="f5582-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f5582-135">Property</span></span>|<span data-ttu-id="f5582-136">Typ</span><span class="sxs-lookup"><span data-stu-id="f5582-136">Type</span></span>|<span data-ttu-id="f5582-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5582-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5582-138">id</span><span class="sxs-lookup"><span data-stu-id="f5582-138">id</span></span>|<span data-ttu-id="f5582-139">String</span><span class="sxs-lookup"><span data-stu-id="f5582-139">String</span></span>|<span data-ttu-id="f5582-140">Der eindeutige Bezeichner für die Entität.</span><span class="sxs-lookup"><span data-stu-id="f5582-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5582-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f5582-141">Relationships</span></span>
<span data-ttu-id="f5582-142">Keine</span><span class="sxs-lookup"><span data-stu-id="f5582-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5582-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f5582-143">JSON Representation</span></span>
<span data-ttu-id="f5582-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f5582-144">Here is a JSON representation of the resource.</span></span>
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



