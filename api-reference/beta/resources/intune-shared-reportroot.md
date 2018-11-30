---
title: reportRoot-Ressourcentyp
description: Die Ressource, die eine Instanz eines Geräts oder zur Problembehandlung Bericht, je nach Kontext darstellt.
ms.openlocfilehash: 581f13bd7383be31ccdce7e536626eb6375ba777
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058457"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="6654b-103">reportRoot-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6654b-103">reportRoot resource type</span></span>

> <span data-ttu-id="6654b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6654b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6654b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6654b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6654b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6654b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6654b-107">Die Ressource, die eine Instanz eines Geräts oder zur Problembehandlung Bericht, je nach Kontext darstellt.</span><span class="sxs-lookup"><span data-stu-id="6654b-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="6654b-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="6654b-108">Methods</span></span>
|<span data-ttu-id="6654b-109">Methode</span><span class="sxs-lookup"><span data-stu-id="6654b-109">Method</span></span>|<span data-ttu-id="6654b-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6654b-110">Return Type</span></span>|<span data-ttu-id="6654b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6654b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6654b-112">reportRoot abrufen</span><span class="sxs-lookup"><span data-stu-id="6654b-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="6654b-113">Lesen von Eigenschaften und Beziehungen des [reportRoot](../resources/intune-shared-reportroot.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6654b-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="6654b-114">reportRoot aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6654b-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="6654b-115">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="6654b-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="6654b-116">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="6654b-116">**Device configuration**</span></span>|
|[<span data-ttu-id="6654b-117">deviceConfigurationUserActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="6654b-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="6654b-118">Metadaten für den Gerätekonfigurations-Benutzeraktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="6654b-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="6654b-119">deviceConfigurationDeviceActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="6654b-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="6654b-120">Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="6654b-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="6654b-121">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="6654b-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="6654b-122">ManagedDeviceEnrollmentAbandonmentDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="6654b-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="6654b-123">report</span><span class="sxs-lookup"><span data-stu-id="6654b-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="6654b-124">Metadaten für die Registrierung Aufgabe Detailbericht</span><span class="sxs-lookup"><span data-stu-id="6654b-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="6654b-125">ManagedDeviceEnrollmentAbandonmentSummary-Funktion</span><span class="sxs-lookup"><span data-stu-id="6654b-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="6654b-126">report</span><span class="sxs-lookup"><span data-stu-id="6654b-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="6654b-127">Metadaten für die Registrierung Aufgabe Zusammenfassungsbericht</span><span class="sxs-lookup"><span data-stu-id="6654b-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="6654b-128">ManagedDeviceEnrollmentFailureDetails-Funktion</span><span class="sxs-lookup"><span data-stu-id="6654b-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="6654b-129">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6654b-129">Not yet documented</span></span>|
|[<span data-ttu-id="6654b-130">ManagedDeviceEnrollmentFailureTrends-Funktion</span><span class="sxs-lookup"><span data-stu-id="6654b-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="6654b-131">Metadaten für die Registrierung Trends Fehlerbericht</span><span class="sxs-lookup"><span data-stu-id="6654b-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="6654b-132">ManagedDeviceEnrollmentTopFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="6654b-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="6654b-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6654b-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6654b-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6654b-134">Properties</span></span>
|<span data-ttu-id="6654b-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6654b-135">Property</span></span>|<span data-ttu-id="6654b-136">Typ</span><span class="sxs-lookup"><span data-stu-id="6654b-136">Type</span></span>|<span data-ttu-id="6654b-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6654b-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6654b-138">id</span><span class="sxs-lookup"><span data-stu-id="6654b-138">id</span></span>|<span data-ttu-id="6654b-139">String</span><span class="sxs-lookup"><span data-stu-id="6654b-139">String</span></span>|<span data-ttu-id="6654b-140">Der eindeutige Bezeichner für die Entität.</span><span class="sxs-lookup"><span data-stu-id="6654b-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6654b-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6654b-141">Relationships</span></span>
<span data-ttu-id="6654b-142">Keine</span><span class="sxs-lookup"><span data-stu-id="6654b-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6654b-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6654b-143">JSON Representation</span></span>
<span data-ttu-id="6654b-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6654b-144">Here is a JSON representation of the resource.</span></span>
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



