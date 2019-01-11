---
title: Aktualisieren von „deviceConfigurationUserOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationUserOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b4ba93e9b945ea4d368250eb481d42662e23f718
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855657"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="88eb7-103">Aktualisieren von „deviceConfigurationUserOverview“</span><span class="sxs-lookup"><span data-stu-id="88eb7-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="88eb7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="88eb7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88eb7-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="88eb7-105">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88eb7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="88eb7-106">Prerequisites</span></span>
<span data-ttu-id="88eb7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88eb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88eb7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="88eb7-109">Permission type</span></span>|<span data-ttu-id="88eb7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88eb7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88eb7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88eb7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88eb7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88eb7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88eb7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88eb7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88eb7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88eb7-114">Not supported.</span></span>|
|<span data-ttu-id="88eb7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88eb7-115">Application</span></span>|<span data-ttu-id="88eb7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88eb7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88eb7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88eb7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="88eb7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88eb7-118">Request headers</span></span>
|<span data-ttu-id="88eb7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="88eb7-119">Header</span></span>|<span data-ttu-id="88eb7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="88eb7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88eb7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88eb7-121">Authorization</span></span>|<span data-ttu-id="88eb7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="88eb7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88eb7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="88eb7-123">Accept</span></span>|<span data-ttu-id="88eb7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88eb7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88eb7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="88eb7-125">Request body</span></span>
<span data-ttu-id="88eb7-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="88eb7-126">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="88eb7-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="88eb7-127">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="88eb7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88eb7-128">Property</span></span>|<span data-ttu-id="88eb7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="88eb7-129">Type</span></span>|<span data-ttu-id="88eb7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88eb7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88eb7-131">id</span><span class="sxs-lookup"><span data-stu-id="88eb7-131">id</span></span>|<span data-ttu-id="88eb7-132">String</span><span class="sxs-lookup"><span data-stu-id="88eb7-132">String</span></span>|<span data-ttu-id="88eb7-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="88eb7-133">Key of the entity.</span></span>|
|<span data-ttu-id="88eb7-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="88eb7-134">pendingCount</span></span>|<span data-ttu-id="88eb7-135">Int32</span><span class="sxs-lookup"><span data-stu-id="88eb7-135">Int32</span></span>|<span data-ttu-id="88eb7-136">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="88eb7-136">Number of pending Users</span></span>|
|<span data-ttu-id="88eb7-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="88eb7-137">notApplicableCount</span></span>|<span data-ttu-id="88eb7-138">Int32</span><span class="sxs-lookup"><span data-stu-id="88eb7-138">Int32</span></span>|<span data-ttu-id="88eb7-139">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="88eb7-139">Number of not applicable users</span></span>|
|<span data-ttu-id="88eb7-140">successCount</span><span class="sxs-lookup"><span data-stu-id="88eb7-140">successCount</span></span>|<span data-ttu-id="88eb7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="88eb7-141">Int32</span></span>|<span data-ttu-id="88eb7-142">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="88eb7-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="88eb7-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="88eb7-143">errorCount</span></span>|<span data-ttu-id="88eb7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="88eb7-144">Int32</span></span>|<span data-ttu-id="88eb7-145">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="88eb7-145">Number of error Users</span></span>|
|<span data-ttu-id="88eb7-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="88eb7-146">failedCount</span></span>|<span data-ttu-id="88eb7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="88eb7-147">Int32</span></span>|<span data-ttu-id="88eb7-148">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="88eb7-148">Number of failed Users</span></span>|
|<span data-ttu-id="88eb7-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="88eb7-149">lastUpdateDateTime</span></span>|<span data-ttu-id="88eb7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88eb7-150">DateTimeOffset</span></span>|<span data-ttu-id="88eb7-151">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="88eb7-151">Last update time</span></span>|
|<span data-ttu-id="88eb7-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="88eb7-152">configurationVersion</span></span>|<span data-ttu-id="88eb7-153">Int32</span><span class="sxs-lookup"><span data-stu-id="88eb7-153">Int32</span></span>|<span data-ttu-id="88eb7-154">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="88eb7-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="88eb7-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="88eb7-155">Response</span></span>
<span data-ttu-id="88eb7-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="88eb7-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88eb7-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88eb7-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="88eb7-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88eb7-158">Request</span></span>
<span data-ttu-id="88eb7-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="88eb7-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 282

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="88eb7-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="88eb7-160">Response</span></span>
<span data-ttu-id="88eb7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="88eb7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



