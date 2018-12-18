---
title: androidCustomConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidCustomConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 4ed0f4eb37ebee3c6915dafe271a2827e7b39c3e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356021"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="7c9cb-103">androidCustomConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7c9cb-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="7c9cb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c9cb-105">Aktualisieren der Eigenschaften eines [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c9cb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c9cb-106">Prerequisites</span></span>
<span data-ttu-id="7c9cb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c9cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c9cb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c9cb-109">Permission type</span></span>|<span data-ttu-id="7c9cb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c9cb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c9cb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c9cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c9cb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c9cb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c9cb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c9cb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c9cb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c9cb-114">Not supported.</span></span>|
|<span data-ttu-id="7c9cb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c9cb-115">Application</span></span>|<span data-ttu-id="7c9cb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c9cb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c9cb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c9cb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7c9cb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c9cb-118">Request headers</span></span>
|<span data-ttu-id="7c9cb-119">Header</span><span class="sxs-lookup"><span data-stu-id="7c9cb-119">Header</span></span>|<span data-ttu-id="7c9cb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7c9cb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c9cb-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7c9cb-121">Authorization</span></span>|<span data-ttu-id="7c9cb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c9cb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c9cb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7c9cb-123">Accept</span></span>|<span data-ttu-id="7c9cb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7c9cb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c9cb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c9cb-125">Request body</span></span>
<span data-ttu-id="7c9cb-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="7c9cb-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="7c9cb-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c9cb-128">Property</span></span>|<span data-ttu-id="7c9cb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7c9cb-129">Type</span></span>|<span data-ttu-id="7c9cb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c9cb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c9cb-131">id</span><span class="sxs-lookup"><span data-stu-id="7c9cb-131">id</span></span>|<span data-ttu-id="7c9cb-132">String</span><span class="sxs-lookup"><span data-stu-id="7c9cb-132">String</span></span>|<span data-ttu-id="7c9cb-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7c9cb-133">Key of the entity.</span></span> <span data-ttu-id="7c9cb-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c9cb-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c9cb-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c9cb-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7c9cb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c9cb-136">DateTimeOffset</span></span>|<span data-ttu-id="7c9cb-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7c9cb-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c9cb-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c9cb-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c9cb-139">createdDateTime</span></span>|<span data-ttu-id="7c9cb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c9cb-140">DateTimeOffset</span></span>|<span data-ttu-id="7c9cb-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-141">DateTime the object was created.</span></span> <span data-ttu-id="7c9cb-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c9cb-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c9cb-143">description</span><span class="sxs-lookup"><span data-stu-id="7c9cb-143">description</span></span>|<span data-ttu-id="7c9cb-144">String</span><span class="sxs-lookup"><span data-stu-id="7c9cb-144">String</span></span>|<span data-ttu-id="7c9cb-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7c9cb-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7c9cb-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c9cb-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c9cb-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7c9cb-147">displayName</span></span>|<span data-ttu-id="7c9cb-148">String</span><span class="sxs-lookup"><span data-stu-id="7c9cb-148">String</span></span>|<span data-ttu-id="7c9cb-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7c9cb-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7c9cb-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c9cb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c9cb-151">Version</span><span class="sxs-lookup"><span data-stu-id="7c9cb-151">version</span></span>|<span data-ttu-id="7c9cb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9cb-152">Int32</span></span>|<span data-ttu-id="7c9cb-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-153">Version of the device configuration.</span></span> <span data-ttu-id="7c9cb-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c9cb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c9cb-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="7c9cb-155">omaSettings</span></span>|<span data-ttu-id="7c9cb-156">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7c9cb-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="7c9cb-157">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-157">OMA settings.</span></span> <span data-ttu-id="7c9cb-158">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7c9cb-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c9cb-159">Response</span></span>
<span data-ttu-id="7c9cb-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c9cb-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c9cb-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c9cb-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c9cb-162">Request</span></span>
<span data-ttu-id="7c9cb-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c9cb-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c9cb-164">Response</span></span>
<span data-ttu-id="7c9cb-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c9cb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



