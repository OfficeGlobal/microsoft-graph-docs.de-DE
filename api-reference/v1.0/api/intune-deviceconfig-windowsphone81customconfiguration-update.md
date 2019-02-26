---
title: Aktualisieren von „windowsPhone81CustomConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9c14408373f735e1b9624895cb4392078f51842
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257750"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="a111b-103">Aktualisieren von „windowsPhone81CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="a111b-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="a111b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a111b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a111b-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a111b-105">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a111b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a111b-106">Prerequisites</span></span>
<span data-ttu-id="a111b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a111b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a111b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a111b-109">Permission type</span></span>|<span data-ttu-id="a111b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a111b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a111b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a111b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a111b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a111b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a111b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a111b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a111b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a111b-114">Not supported.</span></span>|
|<span data-ttu-id="a111b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a111b-115">Application</span></span>|<span data-ttu-id="a111b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a111b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a111b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a111b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a111b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a111b-118">Request headers</span></span>
|<span data-ttu-id="a111b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a111b-119">Header</span></span>|<span data-ttu-id="a111b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a111b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a111b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a111b-121">Authorization</span></span>|<span data-ttu-id="a111b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a111b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a111b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a111b-123">Accept</span></span>|<span data-ttu-id="a111b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a111b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a111b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a111b-125">Request body</span></span>
<span data-ttu-id="a111b-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="a111b-126">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="a111b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a111b-127">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="a111b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a111b-128">Property</span></span>|<span data-ttu-id="a111b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a111b-129">Type</span></span>|<span data-ttu-id="a111b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a111b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a111b-131">id</span><span class="sxs-lookup"><span data-stu-id="a111b-131">id</span></span>|<span data-ttu-id="a111b-132">string</span><span class="sxs-lookup"><span data-stu-id="a111b-132">String</span></span>|<span data-ttu-id="a111b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a111b-133">Key of the entity.</span></span> <span data-ttu-id="a111b-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a111b-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a111b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a111b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a111b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a111b-136">DateTimeOffset</span></span>|<span data-ttu-id="a111b-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a111b-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a111b-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a111b-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a111b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a111b-139">createdDateTime</span></span>|<span data-ttu-id="a111b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a111b-140">DateTimeOffset</span></span>|<span data-ttu-id="a111b-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a111b-141">DateTime the object was created.</span></span> <span data-ttu-id="a111b-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a111b-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a111b-143">description</span><span class="sxs-lookup"><span data-stu-id="a111b-143">description</span></span>|<span data-ttu-id="a111b-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a111b-144">String</span></span>|<span data-ttu-id="a111b-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a111b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a111b-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a111b-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a111b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a111b-147">displayName</span></span>|<span data-ttu-id="a111b-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a111b-148">String</span></span>|<span data-ttu-id="a111b-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a111b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a111b-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a111b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a111b-151">Version</span><span class="sxs-lookup"><span data-stu-id="a111b-151">version</span></span>|<span data-ttu-id="a111b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a111b-152">Int32</span></span>|<span data-ttu-id="a111b-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a111b-153">Version of the device configuration.</span></span> <span data-ttu-id="a111b-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a111b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a111b-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="a111b-155">omaSettings</span></span>|<span data-ttu-id="a111b-156">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a111b-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="a111b-157">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="a111b-157">OMA settings.</span></span> <span data-ttu-id="a111b-158">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a111b-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a111b-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="a111b-159">Response</span></span>
<span data-ttu-id="a111b-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a111b-160">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a111b-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a111b-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="a111b-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a111b-162">Request</span></span>
<span data-ttu-id="a111b-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a111b-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="a111b-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="a111b-164">Response</span></span>
<span data-ttu-id="a111b-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a111b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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



