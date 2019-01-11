---
title: androidCustomConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 78b01b09266aaef7d627f5cf1d4ba4899c2dc41b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831241"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="17e00-103">androidCustomConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="17e00-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="17e00-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="17e00-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17e00-105">Aktualisieren der Eigenschaften eines [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="17e00-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17e00-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="17e00-106">Prerequisites</span></span>
<span data-ttu-id="17e00-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17e00-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17e00-109">Permission type</span></span>|<span data-ttu-id="17e00-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17e00-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17e00-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17e00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="17e00-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17e00-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17e00-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17e00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17e00-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17e00-114">Not supported.</span></span>|
|<span data-ttu-id="17e00-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17e00-115">Application</span></span>|<span data-ttu-id="17e00-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17e00-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17e00-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17e00-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="17e00-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17e00-118">Request headers</span></span>
|<span data-ttu-id="17e00-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="17e00-119">Header</span></span>|<span data-ttu-id="17e00-120">Wert</span><span class="sxs-lookup"><span data-stu-id="17e00-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17e00-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="17e00-121">Authorization</span></span>|<span data-ttu-id="17e00-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="17e00-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17e00-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="17e00-123">Accept</span></span>|<span data-ttu-id="17e00-124">application/json</span><span class="sxs-lookup"><span data-stu-id="17e00-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17e00-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17e00-125">Request body</span></span>
<span data-ttu-id="17e00-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="17e00-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="17e00-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="17e00-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="17e00-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17e00-128">Property</span></span>|<span data-ttu-id="17e00-129">Typ</span><span class="sxs-lookup"><span data-stu-id="17e00-129">Type</span></span>|<span data-ttu-id="17e00-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17e00-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17e00-131">id</span><span class="sxs-lookup"><span data-stu-id="17e00-131">id</span></span>|<span data-ttu-id="17e00-132">String</span><span class="sxs-lookup"><span data-stu-id="17e00-132">String</span></span>|<span data-ttu-id="17e00-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="17e00-133">Key of the entity.</span></span> <span data-ttu-id="17e00-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17e00-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17e00-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17e00-135">lastModifiedDateTime</span></span>|<span data-ttu-id="17e00-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17e00-136">DateTimeOffset</span></span>|<span data-ttu-id="17e00-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="17e00-137">DateTime the object was last modified.</span></span> <span data-ttu-id="17e00-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17e00-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17e00-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17e00-139">createdDateTime</span></span>|<span data-ttu-id="17e00-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17e00-140">DateTimeOffset</span></span>|<span data-ttu-id="17e00-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="17e00-141">DateTime the object was created.</span></span> <span data-ttu-id="17e00-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17e00-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17e00-143">description</span><span class="sxs-lookup"><span data-stu-id="17e00-143">description</span></span>|<span data-ttu-id="17e00-144">String</span><span class="sxs-lookup"><span data-stu-id="17e00-144">String</span></span>|<span data-ttu-id="17e00-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="17e00-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="17e00-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17e00-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17e00-147">displayName</span><span class="sxs-lookup"><span data-stu-id="17e00-147">displayName</span></span>|<span data-ttu-id="17e00-148">String</span><span class="sxs-lookup"><span data-stu-id="17e00-148">String</span></span>|<span data-ttu-id="17e00-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="17e00-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="17e00-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17e00-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17e00-151">Version</span><span class="sxs-lookup"><span data-stu-id="17e00-151">version</span></span>|<span data-ttu-id="17e00-152">Int32</span><span class="sxs-lookup"><span data-stu-id="17e00-152">Int32</span></span>|<span data-ttu-id="17e00-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="17e00-153">Version of the device configuration.</span></span> <span data-ttu-id="17e00-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17e00-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17e00-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="17e00-155">omaSettings</span></span>|<span data-ttu-id="17e00-156">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="17e00-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="17e00-157">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="17e00-157">OMA settings.</span></span> <span data-ttu-id="17e00-158">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="17e00-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="17e00-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="17e00-159">Response</span></span>
<span data-ttu-id="17e00-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="17e00-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17e00-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17e00-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="17e00-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17e00-162">Request</span></span>
<span data-ttu-id="17e00-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17e00-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="17e00-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="17e00-164">Response</span></span>
<span data-ttu-id="17e00-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17e00-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



