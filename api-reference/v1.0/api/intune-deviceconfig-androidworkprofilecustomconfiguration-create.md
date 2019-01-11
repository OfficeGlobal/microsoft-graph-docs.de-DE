---
title: Erstellen von androidWorkProfileCustomConfiguration
description: Erstellen eines neuen AndroidWorkProfileCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0d05aee835dfe98d78b3afc31e0ec2af0e7775be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850813"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="0e041-103">Erstellen von androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e041-103">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="0e041-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0e041-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e041-105">Erstellen eines neuen [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e041-105">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e041-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0e041-106">Prerequisites</span></span>
<span data-ttu-id="0e041-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e041-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e041-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e041-109">Permission type</span></span>|<span data-ttu-id="0e041-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e041-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e041-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e041-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e041-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e041-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e041-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e041-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e041-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e041-114">Not supported.</span></span>|
|<span data-ttu-id="0e041-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e041-115">Application</span></span>|<span data-ttu-id="0e041-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e041-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e041-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e041-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0e041-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e041-118">Request headers</span></span>
|<span data-ttu-id="0e041-119">Header</span><span class="sxs-lookup"><span data-stu-id="0e041-119">Header</span></span>|<span data-ttu-id="0e041-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0e041-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e041-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e041-121">Authorization</span></span>|<span data-ttu-id="0e041-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0e041-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e041-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0e041-123">Accept</span></span>|<span data-ttu-id="0e041-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e041-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e041-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e041-125">Request body</span></span>
<span data-ttu-id="0e041-126">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfileCustomConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0e041-126">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="0e041-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfileCustomConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="0e041-127">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="0e041-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e041-128">Property</span></span>|<span data-ttu-id="0e041-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0e041-129">Type</span></span>|<span data-ttu-id="0e041-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e041-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e041-131">id</span><span class="sxs-lookup"><span data-stu-id="0e041-131">id</span></span>|<span data-ttu-id="0e041-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e041-132">String</span></span>|<span data-ttu-id="0e041-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0e041-133">Key of the entity.</span></span> <span data-ttu-id="0e041-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e041-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e041-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e041-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0e041-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e041-136">DateTimeOffset</span></span>|<span data-ttu-id="0e041-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e041-137">DateTime the object was last modified.</span></span> <span data-ttu-id="0e041-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e041-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e041-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e041-139">createdDateTime</span></span>|<span data-ttu-id="0e041-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e041-140">DateTimeOffset</span></span>|<span data-ttu-id="0e041-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e041-141">DateTime the object was created.</span></span> <span data-ttu-id="0e041-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e041-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e041-143">description</span><span class="sxs-lookup"><span data-stu-id="0e041-143">description</span></span>|<span data-ttu-id="0e041-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e041-144">String</span></span>|<span data-ttu-id="0e041-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0e041-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e041-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e041-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e041-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0e041-147">displayName</span></span>|<span data-ttu-id="0e041-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e041-148">String</span></span>|<span data-ttu-id="0e041-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0e041-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e041-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e041-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e041-151">Version</span><span class="sxs-lookup"><span data-stu-id="0e041-151">version</span></span>|<span data-ttu-id="0e041-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0e041-152">Int32</span></span>|<span data-ttu-id="0e041-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0e041-153">Version of the device configuration.</span></span> <span data-ttu-id="0e041-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e041-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e041-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="0e041-155">omaSettings</span></span>|<span data-ttu-id="0e041-156">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e041-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="0e041-157">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="0e041-157">OMA settings.</span></span> <span data-ttu-id="0e041-158">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="0e041-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0e041-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e041-159">Response</span></span>
<span data-ttu-id="0e041-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0e041-160">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e041-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e041-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e041-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e041-162">Request</span></span>
<span data-ttu-id="0e041-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e041-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0e041-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e041-164">Response</span></span>
<span data-ttu-id="0e041-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e041-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



