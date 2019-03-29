---
title: Aktualisieren von „managedMobileApp“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 378c28bfee54090fd0802ff4c5ae61b262adf41f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972326"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="2f826-103">Aktualisieren von „managedMobileApp“</span><span class="sxs-lookup"><span data-stu-id="2f826-103">Update managedMobileApp</span></span>

> <span data-ttu-id="2f826-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f826-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f826-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2f826-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f826-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f826-106">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f826-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f826-107">Prerequisites</span></span>
<span data-ttu-id="2f826-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f826-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f826-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f826-110">Permission type</span></span>|<span data-ttu-id="2f826-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f826-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f826-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f826-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f826-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f826-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f826-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f826-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f826-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f826-115">Not supported.</span></span>|
|<span data-ttu-id="2f826-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f826-116">Application</span></span>|<span data-ttu-id="2f826-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f826-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f826-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f826-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2f826-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f826-119">Request headers</span></span>
|<span data-ttu-id="2f826-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f826-120">Header</span></span>|<span data-ttu-id="2f826-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2f826-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f826-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f826-122">Authorization</span></span>|<span data-ttu-id="2f826-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f826-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f826-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2f826-124">Accept</span></span>|<span data-ttu-id="2f826-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f826-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f826-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f826-126">Request body</span></span>
<span data-ttu-id="2f826-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="2f826-127">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="2f826-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2f826-128">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="2f826-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f826-129">Property</span></span>|<span data-ttu-id="2f826-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2f826-130">Type</span></span>|<span data-ttu-id="2f826-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f826-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f826-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f826-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="2f826-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f826-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="2f826-134">Bezeichner für eine App mit dem zugehörigen Betriebssystemtyp</span><span class="sxs-lookup"><span data-stu-id="2f826-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="2f826-135">id</span><span class="sxs-lookup"><span data-stu-id="2f826-135">id</span></span>|<span data-ttu-id="2f826-136">String</span><span class="sxs-lookup"><span data-stu-id="2f826-136">String</span></span>|<span data-ttu-id="2f826-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2f826-137">Key of the entity.</span></span>|
|<span data-ttu-id="2f826-138">Version</span><span class="sxs-lookup"><span data-stu-id="2f826-138">version</span></span>|<span data-ttu-id="2f826-139">String</span><span class="sxs-lookup"><span data-stu-id="2f826-139">String</span></span>|<span data-ttu-id="2f826-140">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="2f826-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="2f826-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f826-141">Response</span></span>
<span data-ttu-id="2f826-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2f826-142">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f826-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f826-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f826-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f826-144">Request</span></span>
<span data-ttu-id="2f826-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f826-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f826-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f826-146">Response</span></span>
<span data-ttu-id="2f826-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f826-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




