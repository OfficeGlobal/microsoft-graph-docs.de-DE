---
title: Aktualisieren von „deviceConfigurationUserOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationUserOverview.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cedb9b1116024821d22dec7d159cadc602fba08e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412989"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="f781c-103">Aktualisieren von „deviceConfigurationUserOverview“</span><span class="sxs-lookup"><span data-stu-id="f781c-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="f781c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f781c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f781c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f781c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f781c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f781c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f781c-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="f781c-107">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f781c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f781c-108">Prerequisites</span></span>
<span data-ttu-id="f781c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f781c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f781c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f781c-111">Permission type</span></span>|<span data-ttu-id="f781c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f781c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f781c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f781c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f781c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f781c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f781c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f781c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f781c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f781c-116">Not supported.</span></span>|
|<span data-ttu-id="f781c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f781c-117">Application</span></span>|<span data-ttu-id="f781c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f781c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f781c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f781c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f781c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f781c-120">Request headers</span></span>
|<span data-ttu-id="f781c-121">Header</span><span class="sxs-lookup"><span data-stu-id="f781c-121">Header</span></span>|<span data-ttu-id="f781c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f781c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f781c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f781c-123">Authorization</span></span>|<span data-ttu-id="f781c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f781c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f781c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f781c-125">Accept</span></span>|<span data-ttu-id="f781c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f781c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f781c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f781c-127">Request body</span></span>
<span data-ttu-id="f781c-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="f781c-128">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="f781c-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f781c-129">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="f781c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f781c-130">Property</span></span>|<span data-ttu-id="f781c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f781c-131">Type</span></span>|<span data-ttu-id="f781c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f781c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f781c-133">id</span><span class="sxs-lookup"><span data-stu-id="f781c-133">id</span></span>|<span data-ttu-id="f781c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f781c-134">String</span></span>|<span data-ttu-id="f781c-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f781c-135">Key of the entity.</span></span>|
|<span data-ttu-id="f781c-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f781c-136">pendingCount</span></span>|<span data-ttu-id="f781c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f781c-137">Int32</span></span>|<span data-ttu-id="f781c-138">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="f781c-138">Number of pending Users</span></span>|
|<span data-ttu-id="f781c-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f781c-139">notApplicableCount</span></span>|<span data-ttu-id="f781c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f781c-140">Int32</span></span>|<span data-ttu-id="f781c-141">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="f781c-141">Number of not applicable users</span></span>|
|<span data-ttu-id="f781c-142">successCount</span><span class="sxs-lookup"><span data-stu-id="f781c-142">successCount</span></span>|<span data-ttu-id="f781c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f781c-143">Int32</span></span>|<span data-ttu-id="f781c-144">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="f781c-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="f781c-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="f781c-145">errorCount</span></span>|<span data-ttu-id="f781c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f781c-146">Int32</span></span>|<span data-ttu-id="f781c-147">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="f781c-147">Number of error Users</span></span>|
|<span data-ttu-id="f781c-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="f781c-148">failedCount</span></span>|<span data-ttu-id="f781c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f781c-149">Int32</span></span>|<span data-ttu-id="f781c-150">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="f781c-150">Number of failed Users</span></span>|
|<span data-ttu-id="f781c-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="f781c-151">conflictCount</span></span>|<span data-ttu-id="f781c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f781c-152">Int32</span></span>|<span data-ttu-id="f781c-153">Anzahl von Benutzern in Konflikt</span><span class="sxs-lookup"><span data-stu-id="f781c-153">Number of users in conflict</span></span>|
|<span data-ttu-id="f781c-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f781c-154">lastUpdateDateTime</span></span>|<span data-ttu-id="f781c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f781c-155">DateTimeOffset</span></span>|<span data-ttu-id="f781c-156">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="f781c-156">Last update time</span></span>|
|<span data-ttu-id="f781c-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f781c-157">configurationVersion</span></span>|<span data-ttu-id="f781c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f781c-158">Int32</span></span>|<span data-ttu-id="f781c-159">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="f781c-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f781c-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="f781c-160">Response</span></span>
<span data-ttu-id="f781c-161">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f781c-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f781c-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f781c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f781c-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f781c-163">Request</span></span>
<span data-ttu-id="f781c-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f781c-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f781c-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="f781c-165">Response</span></span>
<span data-ttu-id="f781c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f781c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




