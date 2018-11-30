---
title: AndroidWorkProfileCustomConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidWorkProfileCustomConfiguration-Objekts.
ms.openlocfilehash: 85d8d361f89358079b1ca945b80be3b9e239af0b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018682"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="157a2-103">AndroidWorkProfileCustomConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="157a2-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="157a2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="157a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="157a2-105">Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="157a2-105">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="157a2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="157a2-106">Prerequisites</span></span>
<span data-ttu-id="157a2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="157a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="157a2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="157a2-109">Permission type</span></span>|<span data-ttu-id="157a2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="157a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="157a2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="157a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="157a2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="157a2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="157a2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="157a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="157a2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="157a2-114">Not supported.</span></span>|
|<span data-ttu-id="157a2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="157a2-115">Application</span></span>|<span data-ttu-id="157a2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="157a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="157a2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="157a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="157a2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="157a2-118">Request headers</span></span>
|<span data-ttu-id="157a2-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="157a2-119">Header</span></span>|<span data-ttu-id="157a2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="157a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="157a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="157a2-121">Authorization</span></span>|<span data-ttu-id="157a2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="157a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="157a2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="157a2-123">Accept</span></span>|<span data-ttu-id="157a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="157a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="157a2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="157a2-125">Request body</span></span>
<span data-ttu-id="157a2-126">Geben Sie im Textkörper Anforderung für das Objekt [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="157a2-126">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="157a2-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="157a2-127">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="157a2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="157a2-128">Property</span></span>|<span data-ttu-id="157a2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="157a2-129">Type</span></span>|<span data-ttu-id="157a2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="157a2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="157a2-131">id</span><span class="sxs-lookup"><span data-stu-id="157a2-131">id</span></span>|<span data-ttu-id="157a2-132">String</span><span class="sxs-lookup"><span data-stu-id="157a2-132">String</span></span>|<span data-ttu-id="157a2-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="157a2-133">Key of the entity.</span></span> <span data-ttu-id="157a2-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="157a2-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="157a2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="157a2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="157a2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="157a2-136">DateTimeOffset</span></span>|<span data-ttu-id="157a2-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="157a2-137">DateTime the object was last modified.</span></span> <span data-ttu-id="157a2-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="157a2-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="157a2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="157a2-139">createdDateTime</span></span>|<span data-ttu-id="157a2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="157a2-140">DateTimeOffset</span></span>|<span data-ttu-id="157a2-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="157a2-141">DateTime the object was created.</span></span> <span data-ttu-id="157a2-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="157a2-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="157a2-143">description</span><span class="sxs-lookup"><span data-stu-id="157a2-143">description</span></span>|<span data-ttu-id="157a2-144">String</span><span class="sxs-lookup"><span data-stu-id="157a2-144">String</span></span>|<span data-ttu-id="157a2-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="157a2-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="157a2-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="157a2-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="157a2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="157a2-147">displayName</span></span>|<span data-ttu-id="157a2-148">String</span><span class="sxs-lookup"><span data-stu-id="157a2-148">String</span></span>|<span data-ttu-id="157a2-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="157a2-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="157a2-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="157a2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="157a2-151">Version</span><span class="sxs-lookup"><span data-stu-id="157a2-151">version</span></span>|<span data-ttu-id="157a2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="157a2-152">Int32</span></span>|<span data-ttu-id="157a2-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="157a2-153">Version of the device configuration.</span></span> <span data-ttu-id="157a2-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="157a2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="157a2-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="157a2-155">omaSettings</span></span>|<span data-ttu-id="157a2-156">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="157a2-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="157a2-157">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="157a2-157">OMA settings.</span></span> <span data-ttu-id="157a2-158">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="157a2-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="157a2-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="157a2-159">Response</span></span>
<span data-ttu-id="157a2-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="157a2-160">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="157a2-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="157a2-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="157a2-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="157a2-162">Request</span></span>
<span data-ttu-id="157a2-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="157a2-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="157a2-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="157a2-164">Response</span></span>
<span data-ttu-id="157a2-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="157a2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```



