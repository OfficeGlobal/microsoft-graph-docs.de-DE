---
title: Erstellen von defaultDeviceCompliancePolicy
description: Erstellen eines neuen DefaultDeviceCompliancePolicy-Objekts.
ms.openlocfilehash: 8c05cc7eedc1249175b6738ea241dea37fa5cad4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058894"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="acc38-103">Erstellen von defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="acc38-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="acc38-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="acc38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acc38-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="acc38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acc38-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="acc38-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acc38-107">Erstellen eines neuen [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="acc38-107">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acc38-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="acc38-108">Prerequisites</span></span>
<span data-ttu-id="acc38-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acc38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acc38-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acc38-111">Permission type</span></span>|<span data-ttu-id="acc38-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acc38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acc38-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acc38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acc38-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acc38-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="acc38-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acc38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acc38-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acc38-116">Not supported.</span></span>|
|<span data-ttu-id="acc38-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acc38-117">Application</span></span>|<span data-ttu-id="acc38-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acc38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acc38-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acc38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="acc38-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acc38-120">Request headers</span></span>
|<span data-ttu-id="acc38-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="acc38-121">Header</span></span>|<span data-ttu-id="acc38-122">Wert</span><span class="sxs-lookup"><span data-stu-id="acc38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acc38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acc38-123">Authorization</span></span>|<span data-ttu-id="acc38-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="acc38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acc38-125">Accept</span><span class="sxs-lookup"><span data-stu-id="acc38-125">Accept</span></span>|<span data-ttu-id="acc38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acc38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acc38-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acc38-127">Request body</span></span>
<span data-ttu-id="acc38-128">Geben Sie im Textkörper Anforderung für das Objekt DefaultDeviceCompliancePolicy eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="acc38-128">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="acc38-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DefaultDeviceCompliancePolicy erstellen.</span><span class="sxs-lookup"><span data-stu-id="acc38-129">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="acc38-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acc38-130">Property</span></span>|<span data-ttu-id="acc38-131">Typ</span><span class="sxs-lookup"><span data-stu-id="acc38-131">Type</span></span>|<span data-ttu-id="acc38-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acc38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acc38-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="acc38-133">roleScopeTagIds</span></span>|<span data-ttu-id="acc38-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="acc38-134">String collection</span></span>|<span data-ttu-id="acc38-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="acc38-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="acc38-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="acc38-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="acc38-137">id</span><span class="sxs-lookup"><span data-stu-id="acc38-137">id</span></span>|<span data-ttu-id="acc38-138">String</span><span class="sxs-lookup"><span data-stu-id="acc38-138">String</span></span>|<span data-ttu-id="acc38-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="acc38-139">Key of the entity.</span></span> <span data-ttu-id="acc38-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="acc38-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="acc38-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acc38-141">createdDateTime</span></span>|<span data-ttu-id="acc38-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acc38-142">DateTimeOffset</span></span>|<span data-ttu-id="acc38-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="acc38-143">DateTime the object was created.</span></span> <span data-ttu-id="acc38-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="acc38-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="acc38-145">description</span><span class="sxs-lookup"><span data-stu-id="acc38-145">description</span></span>|<span data-ttu-id="acc38-146">String</span><span class="sxs-lookup"><span data-stu-id="acc38-146">String</span></span>|<span data-ttu-id="acc38-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="acc38-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="acc38-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="acc38-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="acc38-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acc38-149">lastModifiedDateTime</span></span>|<span data-ttu-id="acc38-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acc38-150">DateTimeOffset</span></span>|<span data-ttu-id="acc38-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="acc38-151">DateTime the object was last modified.</span></span> <span data-ttu-id="acc38-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="acc38-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="acc38-153">displayName</span><span class="sxs-lookup"><span data-stu-id="acc38-153">displayName</span></span>|<span data-ttu-id="acc38-154">String</span><span class="sxs-lookup"><span data-stu-id="acc38-154">String</span></span>|<span data-ttu-id="acc38-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="acc38-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="acc38-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="acc38-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="acc38-157">Version</span><span class="sxs-lookup"><span data-stu-id="acc38-157">version</span></span>|<span data-ttu-id="acc38-158">Int32</span><span class="sxs-lookup"><span data-stu-id="acc38-158">Int32</span></span>|<span data-ttu-id="acc38-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="acc38-159">Version of the device configuration.</span></span> <span data-ttu-id="acc38-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="acc38-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="acc38-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="acc38-161">Response</span></span>
<span data-ttu-id="acc38-162">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="acc38-162">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acc38-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acc38-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="acc38-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acc38-164">Request</span></span>
<span data-ttu-id="acc38-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acc38-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="acc38-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="acc38-166">Response</span></span>
<span data-ttu-id="acc38-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acc38-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





