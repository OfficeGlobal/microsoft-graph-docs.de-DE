---
title: IosLobAppProvisioningConfiguration erstellen
description: Erstellen eines neuen iosLobAppProvisioningConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08a3cb70d7fc10274e44550d83da252710d9ec9d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171526"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="66d18-103">IosLobAppProvisioningConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="66d18-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="66d18-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66d18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d18-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="66d18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d18-106">Erstellen eines neuen [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="66d18-106">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66d18-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="66d18-107">Prerequisites</span></span>
<span data-ttu-id="66d18-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="66d18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66d18-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66d18-110">Permission type</span></span>|<span data-ttu-id="66d18-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66d18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66d18-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66d18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66d18-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d18-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66d18-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66d18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66d18-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66d18-115">Not supported.</span></span>|
|<span data-ttu-id="66d18-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66d18-116">Application</span></span>|<span data-ttu-id="66d18-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66d18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66d18-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66d18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="66d18-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66d18-119">Request headers</span></span>
|<span data-ttu-id="66d18-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="66d18-120">Header</span></span>|<span data-ttu-id="66d18-121">Wert</span><span class="sxs-lookup"><span data-stu-id="66d18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66d18-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66d18-122">Authorization</span></span>|<span data-ttu-id="66d18-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="66d18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66d18-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="66d18-124">Accept</span></span>|<span data-ttu-id="66d18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66d18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66d18-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66d18-126">Request body</span></span>
<span data-ttu-id="66d18-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das iosLobAppProvisioningConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="66d18-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="66d18-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosLobAppProvisioningConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="66d18-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="66d18-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66d18-129">Property</span></span>|<span data-ttu-id="66d18-130">Typ</span><span class="sxs-lookup"><span data-stu-id="66d18-130">Type</span></span>|<span data-ttu-id="66d18-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66d18-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d18-132">id</span><span class="sxs-lookup"><span data-stu-id="66d18-132">id</span></span>|<span data-ttu-id="66d18-133">string</span><span class="sxs-lookup"><span data-stu-id="66d18-133">String</span></span>|<span data-ttu-id="66d18-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="66d18-134">Key of the entity.</span></span>|
|<span data-ttu-id="66d18-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="66d18-135">expirationDateTime</span></span>|<span data-ttu-id="66d18-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66d18-136">DateTimeOffset</span></span>|<span data-ttu-id="66d18-137">Optionales Profil Ablaufdatum und-Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="66d18-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="66d18-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="66d18-138">payloadFileName</span></span>|<span data-ttu-id="66d18-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66d18-139">String</span></span>|<span data-ttu-id="66d18-140">Name der Nutzlastdatei (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="66d18-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="66d18-141">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="66d18-141">\*.xml).</span></span>|
|<span data-ttu-id="66d18-142">payload</span><span class="sxs-lookup"><span data-stu-id="66d18-142">payload</span></span>|<span data-ttu-id="66d18-143">Binär</span><span class="sxs-lookup"><span data-stu-id="66d18-143">Binary</span></span>|<span data-ttu-id="66d18-144">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="66d18-144">Payload.</span></span> <span data-ttu-id="66d18-145">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="66d18-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="66d18-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66d18-146">createdDateTime</span></span>|<span data-ttu-id="66d18-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66d18-147">DateTimeOffset</span></span>|<span data-ttu-id="66d18-148">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="66d18-148">DateTime the object was created.</span></span>|
|<span data-ttu-id="66d18-149">description</span><span class="sxs-lookup"><span data-stu-id="66d18-149">description</span></span>|<span data-ttu-id="66d18-150">String</span><span class="sxs-lookup"><span data-stu-id="66d18-150">String</span></span>|<span data-ttu-id="66d18-151">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="66d18-151">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="66d18-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66d18-152">lastModifiedDateTime</span></span>|<span data-ttu-id="66d18-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66d18-153">DateTimeOffset</span></span>|<span data-ttu-id="66d18-154">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="66d18-154">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="66d18-155">displayName</span><span class="sxs-lookup"><span data-stu-id="66d18-155">displayName</span></span>|<span data-ttu-id="66d18-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66d18-156">String</span></span>|<span data-ttu-id="66d18-157">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="66d18-157">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="66d18-158">version</span><span class="sxs-lookup"><span data-stu-id="66d18-158">version</span></span>|<span data-ttu-id="66d18-159">Int32</span><span class="sxs-lookup"><span data-stu-id="66d18-159">Int32</span></span>|<span data-ttu-id="66d18-160">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="66d18-160">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="66d18-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="66d18-161">Response</span></span>
<span data-ttu-id="66d18-162">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="66d18-162">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66d18-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66d18-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="66d18-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66d18-164">Request</span></span>
<span data-ttu-id="66d18-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66d18-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="66d18-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="66d18-166">Response</span></span>
<span data-ttu-id="66d18-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66d18-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 485

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




