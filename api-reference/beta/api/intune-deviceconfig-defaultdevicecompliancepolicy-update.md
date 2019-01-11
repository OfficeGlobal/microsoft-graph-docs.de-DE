---
title: DefaultDeviceCompliancePolicy aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DefaultDeviceCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a6bad561bc82777c594191a34eb6dec8b3a3e3ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817402"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="abbdd-103">DefaultDeviceCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="abbdd-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="abbdd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="abbdd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abbdd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="abbdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abbdd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="abbdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abbdd-107">Aktualisieren Sie die Eigenschaften eines [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="abbdd-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abbdd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="abbdd-108">Prerequisites</span></span>
<span data-ttu-id="abbdd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abbdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abbdd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="abbdd-111">Permission type</span></span>|<span data-ttu-id="abbdd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="abbdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abbdd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="abbdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abbdd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abbdd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abbdd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="abbdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abbdd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abbdd-116">Not supported.</span></span>|
|<span data-ttu-id="abbdd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="abbdd-117">Application</span></span>|<span data-ttu-id="abbdd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abbdd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abbdd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="abbdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="abbdd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="abbdd-120">Request headers</span></span>
|<span data-ttu-id="abbdd-121">Header</span><span class="sxs-lookup"><span data-stu-id="abbdd-121">Header</span></span>|<span data-ttu-id="abbdd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="abbdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abbdd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="abbdd-123">Authorization</span></span>|<span data-ttu-id="abbdd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="abbdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abbdd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="abbdd-125">Accept</span></span>|<span data-ttu-id="abbdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abbdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abbdd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="abbdd-127">Request body</span></span>
<span data-ttu-id="abbdd-128">Geben Sie im Textkörper Anforderung für das Objekt [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="abbdd-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="abbdd-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="abbdd-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="abbdd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="abbdd-130">Property</span></span>|<span data-ttu-id="abbdd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="abbdd-131">Type</span></span>|<span data-ttu-id="abbdd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abbdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abbdd-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="abbdd-133">roleScopeTagIds</span></span>|<span data-ttu-id="abbdd-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="abbdd-134">String collection</span></span>|<span data-ttu-id="abbdd-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="abbdd-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="abbdd-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbdd-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="abbdd-137">id</span><span class="sxs-lookup"><span data-stu-id="abbdd-137">id</span></span>|<span data-ttu-id="abbdd-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abbdd-138">String</span></span>|<span data-ttu-id="abbdd-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="abbdd-139">Key of the entity.</span></span> <span data-ttu-id="abbdd-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbdd-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="abbdd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abbdd-141">createdDateTime</span></span>|<span data-ttu-id="abbdd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbdd-142">DateTimeOffset</span></span>|<span data-ttu-id="abbdd-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="abbdd-143">DateTime the object was created.</span></span> <span data-ttu-id="abbdd-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbdd-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="abbdd-145">description</span><span class="sxs-lookup"><span data-stu-id="abbdd-145">description</span></span>|<span data-ttu-id="abbdd-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abbdd-146">String</span></span>|<span data-ttu-id="abbdd-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="abbdd-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="abbdd-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbdd-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="abbdd-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abbdd-149">lastModifiedDateTime</span></span>|<span data-ttu-id="abbdd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbdd-150">DateTimeOffset</span></span>|<span data-ttu-id="abbdd-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="abbdd-151">DateTime the object was last modified.</span></span> <span data-ttu-id="abbdd-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbdd-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="abbdd-153">displayName</span><span class="sxs-lookup"><span data-stu-id="abbdd-153">displayName</span></span>|<span data-ttu-id="abbdd-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abbdd-154">String</span></span>|<span data-ttu-id="abbdd-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="abbdd-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="abbdd-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbdd-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="abbdd-157">Version</span><span class="sxs-lookup"><span data-stu-id="abbdd-157">version</span></span>|<span data-ttu-id="abbdd-158">Int32</span><span class="sxs-lookup"><span data-stu-id="abbdd-158">Int32</span></span>|<span data-ttu-id="abbdd-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="abbdd-159">Version of the device configuration.</span></span> <span data-ttu-id="abbdd-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbdd-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="abbdd-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="abbdd-161">Response</span></span>
<span data-ttu-id="abbdd-162">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="abbdd-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abbdd-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="abbdd-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="abbdd-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="abbdd-164">Request</span></span>
<span data-ttu-id="abbdd-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="abbdd-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 225

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="abbdd-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="abbdd-166">Response</span></span>
<span data-ttu-id="abbdd-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abbdd-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





