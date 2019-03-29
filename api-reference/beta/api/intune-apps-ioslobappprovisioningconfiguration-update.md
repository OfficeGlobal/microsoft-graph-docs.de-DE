---
title: IosLobAppProvisioningConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines iosLobAppProvisioningConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19c5117b6982bbc4d1e12676ddbe2a4878ef0f8e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983183"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="61178-103">IosLobAppProvisioningConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="61178-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="61178-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61178-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61178-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="61178-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61178-106">Aktualisieren der Eigenschaften eines [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="61178-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61178-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="61178-107">Prerequisites</span></span>
<span data-ttu-id="61178-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61178-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61178-110">Permission type</span></span>|<span data-ttu-id="61178-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61178-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61178-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61178-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61178-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61178-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61178-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61178-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61178-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61178-115">Not supported.</span></span>|
|<span data-ttu-id="61178-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61178-116">Application</span></span>|<span data-ttu-id="61178-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61178-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61178-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61178-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="61178-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61178-119">Request headers</span></span>
|<span data-ttu-id="61178-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="61178-120">Header</span></span>|<span data-ttu-id="61178-121">Wert</span><span class="sxs-lookup"><span data-stu-id="61178-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61178-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61178-122">Authorization</span></span>|<span data-ttu-id="61178-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="61178-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61178-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="61178-124">Accept</span></span>|<span data-ttu-id="61178-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61178-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61178-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61178-126">Request body</span></span>
<span data-ttu-id="61178-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="61178-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="61178-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="61178-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="61178-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61178-129">Property</span></span>|<span data-ttu-id="61178-130">Typ</span><span class="sxs-lookup"><span data-stu-id="61178-130">Type</span></span>|<span data-ttu-id="61178-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61178-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61178-132">id</span><span class="sxs-lookup"><span data-stu-id="61178-132">id</span></span>|<span data-ttu-id="61178-133">String</span><span class="sxs-lookup"><span data-stu-id="61178-133">String</span></span>|<span data-ttu-id="61178-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="61178-134">Key of the entity.</span></span>|
|<span data-ttu-id="61178-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="61178-135">expirationDateTime</span></span>|<span data-ttu-id="61178-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61178-136">DateTimeOffset</span></span>|<span data-ttu-id="61178-137">Optionales Profil Ablaufdatum und-Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="61178-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="61178-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="61178-138">payloadFileName</span></span>|<span data-ttu-id="61178-139">String</span><span class="sxs-lookup"><span data-stu-id="61178-139">String</span></span>|<span data-ttu-id="61178-140">Name der Nutzlastdatei (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="61178-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="61178-141">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="61178-141">\*.xml).</span></span>|
|<span data-ttu-id="61178-142">payload</span><span class="sxs-lookup"><span data-stu-id="61178-142">payload</span></span>|<span data-ttu-id="61178-143">Binär</span><span class="sxs-lookup"><span data-stu-id="61178-143">Binary</span></span>|<span data-ttu-id="61178-144">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="61178-144">Payload.</span></span> <span data-ttu-id="61178-145">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="61178-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="61178-146">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="61178-146">roleScopeTagIds</span></span>|<span data-ttu-id="61178-147">String collection</span><span class="sxs-lookup"><span data-stu-id="61178-147">String collection</span></span>|<span data-ttu-id="61178-148">Liste der Bereichs Tags für diese iOS-Konfigurationsentität für Branchen-App-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="61178-148">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="61178-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61178-149">createdDateTime</span></span>|<span data-ttu-id="61178-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61178-150">DateTimeOffset</span></span>|<span data-ttu-id="61178-151">DateTime der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="61178-151">DateTime the object was created.</span></span>|
|<span data-ttu-id="61178-152">description</span><span class="sxs-lookup"><span data-stu-id="61178-152">description</span></span>|<span data-ttu-id="61178-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61178-153">String</span></span>|<span data-ttu-id="61178-154">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="61178-154">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="61178-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61178-155">lastModifiedDateTime</span></span>|<span data-ttu-id="61178-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61178-156">DateTimeOffset</span></span>|<span data-ttu-id="61178-157">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="61178-157">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="61178-158">displayName</span><span class="sxs-lookup"><span data-stu-id="61178-158">displayName</span></span>|<span data-ttu-id="61178-159">String</span><span class="sxs-lookup"><span data-stu-id="61178-159">String</span></span>|<span data-ttu-id="61178-160">Vom Administrator bereitgestellter Name der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="61178-160">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="61178-161">version</span><span class="sxs-lookup"><span data-stu-id="61178-161">version</span></span>|<span data-ttu-id="61178-162">Int32</span><span class="sxs-lookup"><span data-stu-id="61178-162">Int32</span></span>|<span data-ttu-id="61178-163">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="61178-163">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="61178-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="61178-164">Response</span></span>
<span data-ttu-id="61178-165">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="61178-165">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61178-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61178-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="61178-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61178-167">Request</span></span>
<span data-ttu-id="61178-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61178-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="61178-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="61178-169">Response</span></span>
<span data-ttu-id="61178-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61178-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




