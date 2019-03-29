---
title: DefaultDeviceCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines defaultDeviceCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c895a4f6f3b709d4b9c5a539108609bc5f572162
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967713"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="959b9-103">DefaultDeviceCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="959b9-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="959b9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="959b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="959b9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="959b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="959b9-106">Aktualisieren der Eigenschaften eines [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="959b9-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="959b9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="959b9-107">Prerequisites</span></span>
<span data-ttu-id="959b9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="959b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="959b9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="959b9-110">Permission type</span></span>|<span data-ttu-id="959b9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="959b9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="959b9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="959b9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="959b9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="959b9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="959b9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="959b9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="959b9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="959b9-115">Not supported.</span></span>|
|<span data-ttu-id="959b9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="959b9-116">Application</span></span>|<span data-ttu-id="959b9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="959b9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="959b9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="959b9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="959b9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="959b9-119">Request headers</span></span>
|<span data-ttu-id="959b9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="959b9-120">Header</span></span>|<span data-ttu-id="959b9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="959b9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="959b9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="959b9-122">Authorization</span></span>|<span data-ttu-id="959b9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="959b9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="959b9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="959b9-124">Accept</span></span>|<span data-ttu-id="959b9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="959b9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="959b9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="959b9-126">Request body</span></span>
<span data-ttu-id="959b9-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="959b9-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="959b9-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="959b9-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="959b9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="959b9-129">Property</span></span>|<span data-ttu-id="959b9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="959b9-130">Type</span></span>|<span data-ttu-id="959b9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="959b9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="959b9-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="959b9-132">roleScopeTagIds</span></span>|<span data-ttu-id="959b9-133">String collection</span><span class="sxs-lookup"><span data-stu-id="959b9-133">String collection</span></span>|<span data-ttu-id="959b9-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="959b9-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="959b9-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="959b9-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="959b9-136">id</span><span class="sxs-lookup"><span data-stu-id="959b9-136">id</span></span>|<span data-ttu-id="959b9-137">String</span><span class="sxs-lookup"><span data-stu-id="959b9-137">String</span></span>|<span data-ttu-id="959b9-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="959b9-138">Key of the entity.</span></span> <span data-ttu-id="959b9-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="959b9-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="959b9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="959b9-140">createdDateTime</span></span>|<span data-ttu-id="959b9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="959b9-141">DateTimeOffset</span></span>|<span data-ttu-id="959b9-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="959b9-142">DateTime the object was created.</span></span> <span data-ttu-id="959b9-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="959b9-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="959b9-144">description</span><span class="sxs-lookup"><span data-stu-id="959b9-144">description</span></span>|<span data-ttu-id="959b9-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="959b9-145">String</span></span>|<span data-ttu-id="959b9-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="959b9-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="959b9-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="959b9-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="959b9-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="959b9-148">lastModifiedDateTime</span></span>|<span data-ttu-id="959b9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="959b9-149">DateTimeOffset</span></span>|<span data-ttu-id="959b9-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="959b9-150">DateTime the object was last modified.</span></span> <span data-ttu-id="959b9-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="959b9-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="959b9-152">displayName</span><span class="sxs-lookup"><span data-stu-id="959b9-152">displayName</span></span>|<span data-ttu-id="959b9-153">String</span><span class="sxs-lookup"><span data-stu-id="959b9-153">String</span></span>|<span data-ttu-id="959b9-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="959b9-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="959b9-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="959b9-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="959b9-156">Version</span><span class="sxs-lookup"><span data-stu-id="959b9-156">version</span></span>|<span data-ttu-id="959b9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="959b9-157">Int32</span></span>|<span data-ttu-id="959b9-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="959b9-158">Version of the device configuration.</span></span> <span data-ttu-id="959b9-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="959b9-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="959b9-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="959b9-160">Response</span></span>
<span data-ttu-id="959b9-161">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="959b9-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="959b9-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="959b9-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="959b9-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="959b9-163">Request</span></span>
<span data-ttu-id="959b9-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="959b9-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="959b9-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="959b9-165">Response</span></span>
<span data-ttu-id="959b9-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="959b9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




