---
title: Aktualisieren von „deviceConfigurationUserOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0837767a7855aec4fe60bf9c3d0adfed52b4b368
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156245"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="44cd5-103">Aktualisieren von „deviceConfigurationUserOverview“</span><span class="sxs-lookup"><span data-stu-id="44cd5-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="44cd5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44cd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44cd5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="44cd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44cd5-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="44cd5-106">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44cd5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="44cd5-107">Prerequisites</span></span>
<span data-ttu-id="44cd5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="44cd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44cd5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44cd5-110">Permission type</span></span>|<span data-ttu-id="44cd5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44cd5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44cd5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44cd5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44cd5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44cd5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44cd5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44cd5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44cd5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44cd5-115">Not supported.</span></span>|
|<span data-ttu-id="44cd5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44cd5-116">Application</span></span>|<span data-ttu-id="44cd5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44cd5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44cd5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44cd5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="44cd5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44cd5-119">Request headers</span></span>
|<span data-ttu-id="44cd5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="44cd5-120">Header</span></span>|<span data-ttu-id="44cd5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="44cd5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44cd5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44cd5-122">Authorization</span></span>|<span data-ttu-id="44cd5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="44cd5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44cd5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="44cd5-124">Accept</span></span>|<span data-ttu-id="44cd5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44cd5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44cd5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44cd5-126">Request body</span></span>
<span data-ttu-id="44cd5-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="44cd5-127">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="44cd5-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="44cd5-128">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="44cd5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44cd5-129">Property</span></span>|<span data-ttu-id="44cd5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="44cd5-130">Type</span></span>|<span data-ttu-id="44cd5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44cd5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44cd5-132">id</span><span class="sxs-lookup"><span data-stu-id="44cd5-132">id</span></span>|<span data-ttu-id="44cd5-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="44cd5-133">String</span></span>|<span data-ttu-id="44cd5-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="44cd5-134">Key of the entity.</span></span>|
|<span data-ttu-id="44cd5-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="44cd5-135">pendingCount</span></span>|<span data-ttu-id="44cd5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="44cd5-136">Int32</span></span>|<span data-ttu-id="44cd5-137">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="44cd5-137">Number of pending Users</span></span>|
|<span data-ttu-id="44cd5-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="44cd5-138">notApplicableCount</span></span>|<span data-ttu-id="44cd5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="44cd5-139">Int32</span></span>|<span data-ttu-id="44cd5-140">Anzahl der nicht anwendbaren Benutzer</span><span class="sxs-lookup"><span data-stu-id="44cd5-140">Number of not applicable users</span></span>|
|<span data-ttu-id="44cd5-141">successCount</span><span class="sxs-lookup"><span data-stu-id="44cd5-141">successCount</span></span>|<span data-ttu-id="44cd5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="44cd5-142">Int32</span></span>|<span data-ttu-id="44cd5-143">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="44cd5-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="44cd5-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="44cd5-144">errorCount</span></span>|<span data-ttu-id="44cd5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="44cd5-145">Int32</span></span>|<span data-ttu-id="44cd5-146">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="44cd5-146">Number of error Users</span></span>|
|<span data-ttu-id="44cd5-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="44cd5-147">failedCount</span></span>|<span data-ttu-id="44cd5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="44cd5-148">Int32</span></span>|<span data-ttu-id="44cd5-149">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="44cd5-149">Number of failed Users</span></span>|
|<span data-ttu-id="44cd5-150">Conflictcount zur</span><span class="sxs-lookup"><span data-stu-id="44cd5-150">conflictCount</span></span>|<span data-ttu-id="44cd5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="44cd5-151">Int32</span></span>|<span data-ttu-id="44cd5-152">Anzahl der in Konflikt stehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="44cd5-152">Number of users in conflict</span></span>|
|<span data-ttu-id="44cd5-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="44cd5-153">lastUpdateDateTime</span></span>|<span data-ttu-id="44cd5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44cd5-154">DateTimeOffset</span></span>|<span data-ttu-id="44cd5-155">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="44cd5-155">Last update time</span></span>|
|<span data-ttu-id="44cd5-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="44cd5-156">configurationVersion</span></span>|<span data-ttu-id="44cd5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="44cd5-157">Int32</span></span>|<span data-ttu-id="44cd5-158">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="44cd5-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="44cd5-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="44cd5-159">Response</span></span>
<span data-ttu-id="44cd5-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="44cd5-160">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44cd5-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44cd5-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="44cd5-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44cd5-162">Request</span></span>
<span data-ttu-id="44cd5-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44cd5-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="44cd5-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="44cd5-164">Response</span></span>
<span data-ttu-id="44cd5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44cd5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




