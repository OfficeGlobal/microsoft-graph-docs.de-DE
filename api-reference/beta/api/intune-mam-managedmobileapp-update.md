---
title: Aktualisieren von „managedMobileApp“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfbeafd30626aa5de8679e27002eefbfdc49e4ee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167200"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="25ed4-103">Aktualisieren von „managedMobileApp“</span><span class="sxs-lookup"><span data-stu-id="25ed4-103">Update managedMobileApp</span></span>

> <span data-ttu-id="25ed4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25ed4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25ed4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="25ed4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25ed4-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="25ed4-106">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25ed4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="25ed4-107">Prerequisites</span></span>
<span data-ttu-id="25ed4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="25ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="25ed4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25ed4-110">Permission type</span></span>|<span data-ttu-id="25ed4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25ed4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25ed4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25ed4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25ed4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25ed4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="25ed4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25ed4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25ed4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25ed4-115">Not supported.</span></span>|
|<span data-ttu-id="25ed4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25ed4-116">Application</span></span>|<span data-ttu-id="25ed4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25ed4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25ed4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25ed4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="25ed4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="25ed4-119">Request headers</span></span>
|<span data-ttu-id="25ed4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="25ed4-120">Header</span></span>|<span data-ttu-id="25ed4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="25ed4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25ed4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25ed4-122">Authorization</span></span>|<span data-ttu-id="25ed4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="25ed4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25ed4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="25ed4-124">Accept</span></span>|<span data-ttu-id="25ed4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25ed4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25ed4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25ed4-126">Request body</span></span>
<span data-ttu-id="25ed4-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="25ed4-127">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="25ed4-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="25ed4-128">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="25ed4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="25ed4-129">Property</span></span>|<span data-ttu-id="25ed4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="25ed4-130">Type</span></span>|<span data-ttu-id="25ed4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25ed4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25ed4-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="25ed4-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="25ed4-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="25ed4-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="25ed4-134">Bezeichner der App mit dem zugehörigen Betriebssystemtyp</span><span class="sxs-lookup"><span data-stu-id="25ed4-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="25ed4-135">id</span><span class="sxs-lookup"><span data-stu-id="25ed4-135">id</span></span>|<span data-ttu-id="25ed4-136">string</span><span class="sxs-lookup"><span data-stu-id="25ed4-136">String</span></span>|<span data-ttu-id="25ed4-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="25ed4-137">Key of the entity.</span></span>|
|<span data-ttu-id="25ed4-138">Version</span><span class="sxs-lookup"><span data-stu-id="25ed4-138">version</span></span>|<span data-ttu-id="25ed4-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="25ed4-139">String</span></span>|<span data-ttu-id="25ed4-140">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="25ed4-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="25ed4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="25ed4-141">Response</span></span>
<span data-ttu-id="25ed4-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="25ed4-142">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25ed4-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="25ed4-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="25ed4-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25ed4-144">Request</span></span>
<span data-ttu-id="25ed4-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="25ed4-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="25ed4-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="25ed4-146">Response</span></span>
<span data-ttu-id="25ed4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25ed4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




