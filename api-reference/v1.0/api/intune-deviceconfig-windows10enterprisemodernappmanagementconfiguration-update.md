---
title: Aktualisieren von „windows10EnterpriseModernAppManagementConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10EnterpriseModernAppManagementConfiguration.
ms.openlocfilehash: 6eb9259be829723b66e7b8b2136bceb8b7449c45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018506"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="bd0fe-103">Aktualisieren von „windows10EnterpriseModernAppManagementConfiguration“</span><span class="sxs-lookup"><span data-stu-id="bd0fe-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="bd0fe-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd0fe-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-105">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd0fe-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bd0fe-106">Prerequisites</span></span>
<span data-ttu-id="bd0fe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd0fe-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd0fe-109">Permission type</span></span>|<span data-ttu-id="bd0fe-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd0fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd0fe-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd0fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd0fe-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd0fe-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd0fe-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd0fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd0fe-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd0fe-114">Not supported.</span></span>|
|<span data-ttu-id="bd0fe-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd0fe-115">Application</span></span>|<span data-ttu-id="bd0fe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd0fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd0fe-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd0fe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bd0fe-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd0fe-118">Request headers</span></span>
|<span data-ttu-id="bd0fe-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bd0fe-119">Header</span></span>|<span data-ttu-id="bd0fe-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bd0fe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd0fe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd0fe-121">Authorization</span></span>|<span data-ttu-id="bd0fe-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bd0fe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd0fe-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bd0fe-123">Accept</span></span>|<span data-ttu-id="bd0fe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bd0fe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd0fe-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd0fe-125">Request body</span></span>
<span data-ttu-id="bd0fe-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-126">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="bd0fe-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-127">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="bd0fe-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd0fe-128">Property</span></span>|<span data-ttu-id="bd0fe-129">Typ</span><span class="sxs-lookup"><span data-stu-id="bd0fe-129">Type</span></span>|<span data-ttu-id="bd0fe-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd0fe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd0fe-131">id</span><span class="sxs-lookup"><span data-stu-id="bd0fe-131">id</span></span>|<span data-ttu-id="bd0fe-132">String</span><span class="sxs-lookup"><span data-stu-id="bd0fe-132">String</span></span>|<span data-ttu-id="bd0fe-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bd0fe-133">Key of the entity.</span></span> <span data-ttu-id="bd0fe-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd0fe-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd0fe-135">lastModifiedDateTime</span></span>|<span data-ttu-id="bd0fe-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd0fe-136">DateTimeOffset</span></span>|<span data-ttu-id="bd0fe-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-137">DateTime the object was last modified.</span></span> <span data-ttu-id="bd0fe-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd0fe-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd0fe-139">createdDateTime</span></span>|<span data-ttu-id="bd0fe-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd0fe-140">DateTimeOffset</span></span>|<span data-ttu-id="bd0fe-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-141">DateTime the object was created.</span></span> <span data-ttu-id="bd0fe-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd0fe-143">description</span><span class="sxs-lookup"><span data-stu-id="bd0fe-143">description</span></span>|<span data-ttu-id="bd0fe-144">String</span><span class="sxs-lookup"><span data-stu-id="bd0fe-144">String</span></span>|<span data-ttu-id="bd0fe-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bd0fe-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd0fe-147">displayName</span><span class="sxs-lookup"><span data-stu-id="bd0fe-147">displayName</span></span>|<span data-ttu-id="bd0fe-148">String</span><span class="sxs-lookup"><span data-stu-id="bd0fe-148">String</span></span>|<span data-ttu-id="bd0fe-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bd0fe-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd0fe-151">Version</span><span class="sxs-lookup"><span data-stu-id="bd0fe-151">version</span></span>|<span data-ttu-id="bd0fe-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bd0fe-152">Int32</span></span>|<span data-ttu-id="bd0fe-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-153">Version of the device configuration.</span></span> <span data-ttu-id="bd0fe-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd0fe-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd0fe-155">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="bd0fe-155">uninstallBuiltInApps</span></span>|<span data-ttu-id="bd0fe-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd0fe-156">Boolean</span></span>|<span data-ttu-id="bd0fe-157">Gibt an, ob eine festgelegte Liste integrierter Windows-Apps deinstalliert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-157">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="bd0fe-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd0fe-158">Response</span></span>
<span data-ttu-id="bd0fe-159">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-159">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd0fe-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd0fe-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd0fe-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd0fe-161">Request</span></span>
<span data-ttu-id="bd0fe-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="bd0fe-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd0fe-163">Response</span></span>
<span data-ttu-id="bd0fe-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd0fe-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```



