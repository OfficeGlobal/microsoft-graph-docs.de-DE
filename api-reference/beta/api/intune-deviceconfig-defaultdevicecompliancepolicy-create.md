---
title: Erstellen von defaultDeviceCompliancePolicy
description: Erstellen eines neuen DefaultDeviceCompliancePolicy-Objekts.
author: tfitzmac
ms.openlocfilehash: 7e58ac41c1839429d2a15a4590a6ce765a5341a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327097"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="f70a3-103">Erstellen von defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f70a3-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="f70a3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f70a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f70a3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f70a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f70a3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f70a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f70a3-107">Erstellen eines neuen [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f70a3-107">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f70a3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f70a3-108">Prerequisites</span></span>
<span data-ttu-id="f70a3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f70a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f70a3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f70a3-111">Permission type</span></span>|<span data-ttu-id="f70a3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f70a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f70a3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f70a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f70a3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f70a3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f70a3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f70a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f70a3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f70a3-116">Not supported.</span></span>|
|<span data-ttu-id="f70a3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f70a3-117">Application</span></span>|<span data-ttu-id="f70a3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f70a3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f70a3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f70a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f70a3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f70a3-120">Request headers</span></span>
|<span data-ttu-id="f70a3-121">Header</span><span class="sxs-lookup"><span data-stu-id="f70a3-121">Header</span></span>|<span data-ttu-id="f70a3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f70a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f70a3-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f70a3-123">Authorization</span></span>|<span data-ttu-id="f70a3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f70a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f70a3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f70a3-125">Accept</span></span>|<span data-ttu-id="f70a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f70a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f70a3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f70a3-127">Request body</span></span>
<span data-ttu-id="f70a3-128">Geben Sie im Textkörper Anforderung für das Objekt DefaultDeviceCompliancePolicy eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f70a3-128">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="f70a3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DefaultDeviceCompliancePolicy erstellen.</span><span class="sxs-lookup"><span data-stu-id="f70a3-129">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="f70a3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f70a3-130">Property</span></span>|<span data-ttu-id="f70a3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f70a3-131">Type</span></span>|<span data-ttu-id="f70a3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f70a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f70a3-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f70a3-133">roleScopeTagIds</span></span>|<span data-ttu-id="f70a3-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f70a3-134">String collection</span></span>|<span data-ttu-id="f70a3-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f70a3-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f70a3-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f70a3-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f70a3-137">id</span><span class="sxs-lookup"><span data-stu-id="f70a3-137">id</span></span>|<span data-ttu-id="f70a3-138">String</span><span class="sxs-lookup"><span data-stu-id="f70a3-138">String</span></span>|<span data-ttu-id="f70a3-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f70a3-139">Key of the entity.</span></span> <span data-ttu-id="f70a3-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f70a3-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f70a3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f70a3-141">createdDateTime</span></span>|<span data-ttu-id="f70a3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f70a3-142">DateTimeOffset</span></span>|<span data-ttu-id="f70a3-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f70a3-143">DateTime the object was created.</span></span> <span data-ttu-id="f70a3-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f70a3-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f70a3-145">description</span><span class="sxs-lookup"><span data-stu-id="f70a3-145">description</span></span>|<span data-ttu-id="f70a3-146">String</span><span class="sxs-lookup"><span data-stu-id="f70a3-146">String</span></span>|<span data-ttu-id="f70a3-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f70a3-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f70a3-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f70a3-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f70a3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f70a3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="f70a3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f70a3-150">DateTimeOffset</span></span>|<span data-ttu-id="f70a3-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f70a3-151">DateTime the object was last modified.</span></span> <span data-ttu-id="f70a3-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f70a3-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f70a3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="f70a3-153">displayName</span></span>|<span data-ttu-id="f70a3-154">String</span><span class="sxs-lookup"><span data-stu-id="f70a3-154">String</span></span>|<span data-ttu-id="f70a3-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f70a3-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f70a3-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f70a3-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f70a3-157">Version</span><span class="sxs-lookup"><span data-stu-id="f70a3-157">version</span></span>|<span data-ttu-id="f70a3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f70a3-158">Int32</span></span>|<span data-ttu-id="f70a3-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f70a3-159">Version of the device configuration.</span></span> <span data-ttu-id="f70a3-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f70a3-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f70a3-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="f70a3-161">Response</span></span>
<span data-ttu-id="f70a3-162">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f70a3-162">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f70a3-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f70a3-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="f70a3-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f70a3-164">Request</span></span>
<span data-ttu-id="f70a3-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f70a3-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f70a3-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="f70a3-166">Response</span></span>
<span data-ttu-id="f70a3-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f70a3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





