---
title: DefaultDeviceCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines defaultDeviceCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83b1c534c8b5e27e91bb6a1153f3b0a8f25496d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157701"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="feb87-103">DefaultDeviceCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="feb87-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="feb87-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="feb87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="feb87-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="feb87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feb87-106">Aktualisieren der Eigenschaften eines [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="feb87-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="feb87-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="feb87-107">Prerequisites</span></span>
<span data-ttu-id="feb87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="feb87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="feb87-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="feb87-110">Permission type</span></span>|<span data-ttu-id="feb87-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="feb87-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="feb87-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="feb87-112">Delegated (work or school account)</span></span>|<span data-ttu-id="feb87-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb87-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="feb87-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="feb87-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feb87-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="feb87-115">Not supported.</span></span>|
|<span data-ttu-id="feb87-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="feb87-116">Application</span></span>|<span data-ttu-id="feb87-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="feb87-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="feb87-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="feb87-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="feb87-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="feb87-119">Request headers</span></span>
|<span data-ttu-id="feb87-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="feb87-120">Header</span></span>|<span data-ttu-id="feb87-121">Wert</span><span class="sxs-lookup"><span data-stu-id="feb87-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="feb87-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="feb87-122">Authorization</span></span>|<span data-ttu-id="feb87-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="feb87-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="feb87-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="feb87-124">Accept</span></span>|<span data-ttu-id="feb87-125">application/json</span><span class="sxs-lookup"><span data-stu-id="feb87-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="feb87-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="feb87-126">Request body</span></span>
<span data-ttu-id="feb87-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="feb87-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="feb87-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="feb87-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="feb87-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="feb87-129">Property</span></span>|<span data-ttu-id="feb87-130">Typ</span><span class="sxs-lookup"><span data-stu-id="feb87-130">Type</span></span>|<span data-ttu-id="feb87-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="feb87-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb87-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="feb87-132">roleScopeTagIds</span></span>|<span data-ttu-id="feb87-133">String collection</span><span class="sxs-lookup"><span data-stu-id="feb87-133">String collection</span></span>|<span data-ttu-id="feb87-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="feb87-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="feb87-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="feb87-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="feb87-136">id</span><span class="sxs-lookup"><span data-stu-id="feb87-136">id</span></span>|<span data-ttu-id="feb87-137">string</span><span class="sxs-lookup"><span data-stu-id="feb87-137">String</span></span>|<span data-ttu-id="feb87-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="feb87-138">Key of the entity.</span></span> <span data-ttu-id="feb87-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="feb87-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="feb87-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="feb87-140">createdDateTime</span></span>|<span data-ttu-id="feb87-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feb87-141">DateTimeOffset</span></span>|<span data-ttu-id="feb87-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="feb87-142">DateTime the object was created.</span></span> <span data-ttu-id="feb87-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="feb87-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="feb87-144">description</span><span class="sxs-lookup"><span data-stu-id="feb87-144">description</span></span>|<span data-ttu-id="feb87-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="feb87-145">String</span></span>|<span data-ttu-id="feb87-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="feb87-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="feb87-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="feb87-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="feb87-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="feb87-148">lastModifiedDateTime</span></span>|<span data-ttu-id="feb87-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feb87-149">DateTimeOffset</span></span>|<span data-ttu-id="feb87-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="feb87-150">DateTime the object was last modified.</span></span> <span data-ttu-id="feb87-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="feb87-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="feb87-152">displayName</span><span class="sxs-lookup"><span data-stu-id="feb87-152">displayName</span></span>|<span data-ttu-id="feb87-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="feb87-153">String</span></span>|<span data-ttu-id="feb87-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="feb87-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="feb87-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="feb87-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="feb87-156">Version</span><span class="sxs-lookup"><span data-stu-id="feb87-156">version</span></span>|<span data-ttu-id="feb87-157">Int32</span><span class="sxs-lookup"><span data-stu-id="feb87-157">Int32</span></span>|<span data-ttu-id="feb87-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="feb87-158">Version of the device configuration.</span></span> <span data-ttu-id="feb87-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="feb87-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="feb87-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="feb87-160">Response</span></span>
<span data-ttu-id="feb87-161">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="feb87-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feb87-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="feb87-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="feb87-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="feb87-163">Request</span></span>
<span data-ttu-id="feb87-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="feb87-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 229

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="feb87-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="feb87-165">Response</span></span>
<span data-ttu-id="feb87-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="feb87-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a285f027-f027-a285-27f0-85a227f085a2",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




