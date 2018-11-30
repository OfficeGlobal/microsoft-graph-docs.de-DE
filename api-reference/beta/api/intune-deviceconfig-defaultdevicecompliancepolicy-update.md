---
title: DefaultDeviceCompliancePolicy aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DefaultDeviceCompliancePolicy-Objekts.
ms.openlocfilehash: 65dcf950a1d8f3bbcbbb19b4132713bfb13b5153
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065157"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="c7c63-103">DefaultDeviceCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c7c63-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="c7c63-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7c63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7c63-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7c63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7c63-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c7c63-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7c63-107">Aktualisieren Sie die Eigenschaften eines [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7c63-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7c63-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c7c63-108">Prerequisites</span></span>
<span data-ttu-id="c7c63-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7c63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c63-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7c63-111">Permission type</span></span>|<span data-ttu-id="c7c63-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7c63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7c63-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7c63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7c63-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c63-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7c63-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7c63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7c63-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7c63-116">Not supported.</span></span>|
|<span data-ttu-id="c7c63-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7c63-117">Application</span></span>|<span data-ttu-id="c7c63-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7c63-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7c63-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7c63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c7c63-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7c63-120">Request headers</span></span>
|<span data-ttu-id="c7c63-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c7c63-121">Header</span></span>|<span data-ttu-id="c7c63-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c7c63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7c63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c63-123">Authorization</span></span>|<span data-ttu-id="c7c63-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c7c63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7c63-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7c63-125">Accept</span></span>|<span data-ttu-id="c7c63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7c63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c63-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7c63-127">Request body</span></span>
<span data-ttu-id="c7c63-128">Geben Sie im Textkörper Anforderung für das Objekt [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c7c63-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="c7c63-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="c7c63-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="c7c63-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7c63-130">Property</span></span>|<span data-ttu-id="c7c63-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c7c63-131">Type</span></span>|<span data-ttu-id="c7c63-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7c63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7c63-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7c63-133">roleScopeTagIds</span></span>|<span data-ttu-id="c7c63-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c7c63-134">String collection</span></span>|<span data-ttu-id="c7c63-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="c7c63-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c7c63-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7c63-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7c63-137">id</span><span class="sxs-lookup"><span data-stu-id="c7c63-137">id</span></span>|<span data-ttu-id="c7c63-138">String</span><span class="sxs-lookup"><span data-stu-id="c7c63-138">String</span></span>|<span data-ttu-id="c7c63-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c7c63-139">Key of the entity.</span></span> <span data-ttu-id="c7c63-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7c63-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7c63-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c63-141">createdDateTime</span></span>|<span data-ttu-id="c7c63-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7c63-142">DateTimeOffset</span></span>|<span data-ttu-id="c7c63-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7c63-143">DateTime the object was created.</span></span> <span data-ttu-id="c7c63-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7c63-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7c63-145">description</span><span class="sxs-lookup"><span data-stu-id="c7c63-145">description</span></span>|<span data-ttu-id="c7c63-146">String</span><span class="sxs-lookup"><span data-stu-id="c7c63-146">String</span></span>|<span data-ttu-id="c7c63-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c7c63-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7c63-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7c63-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7c63-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c63-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c7c63-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7c63-150">DateTimeOffset</span></span>|<span data-ttu-id="c7c63-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7c63-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c7c63-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7c63-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7c63-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c7c63-153">displayName</span></span>|<span data-ttu-id="c7c63-154">String</span><span class="sxs-lookup"><span data-stu-id="c7c63-154">String</span></span>|<span data-ttu-id="c7c63-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c7c63-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7c63-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7c63-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7c63-157">Version</span><span class="sxs-lookup"><span data-stu-id="c7c63-157">version</span></span>|<span data-ttu-id="c7c63-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c7c63-158">Int32</span></span>|<span data-ttu-id="c7c63-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c7c63-159">Version of the device configuration.</span></span> <span data-ttu-id="c7c63-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7c63-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c7c63-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7c63-161">Response</span></span>
<span data-ttu-id="c7c63-162">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c7c63-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c63-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7c63-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7c63-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7c63-164">Request</span></span>
<span data-ttu-id="c7c63-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7c63-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7c63-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7c63-166">Response</span></span>
<span data-ttu-id="c7c63-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7c63-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





