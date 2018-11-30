---
title: IosLobAppProvisioningConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosLobAppProvisioningConfiguration-Objekts.
ms.openlocfilehash: dd1986a3b9a64d77959aeeabb339adf137b92df2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060568"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="8a6af-103">IosLobAppProvisioningConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8a6af-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="8a6af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8a6af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a6af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8a6af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a6af-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8a6af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a6af-107">Aktualisieren Sie die Eigenschaften eines [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8a6af-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a6af-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8a6af-108">Prerequisites</span></span>
<span data-ttu-id="8a6af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a6af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a6af-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a6af-111">Permission type</span></span>|<span data-ttu-id="8a6af-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a6af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a6af-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a6af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a6af-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a6af-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a6af-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a6af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a6af-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a6af-116">Not supported.</span></span>|
|<span data-ttu-id="8a6af-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a6af-117">Application</span></span>|<span data-ttu-id="8a6af-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a6af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a6af-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a6af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8a6af-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a6af-120">Request headers</span></span>
|<span data-ttu-id="8a6af-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8a6af-121">Header</span></span>|<span data-ttu-id="8a6af-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8a6af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a6af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a6af-123">Authorization</span></span>|<span data-ttu-id="8a6af-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8a6af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a6af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a6af-125">Accept</span></span>|<span data-ttu-id="8a6af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a6af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a6af-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a6af-127">Request body</span></span>
<span data-ttu-id="8a6af-128">Geben Sie im Textkörper Anforderung für das Objekt [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8a6af-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="8a6af-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="8a6af-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="8a6af-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8a6af-130">Property</span></span>|<span data-ttu-id="8a6af-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8a6af-131">Type</span></span>|<span data-ttu-id="8a6af-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a6af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a6af-133">id</span><span class="sxs-lookup"><span data-stu-id="8a6af-133">id</span></span>|<span data-ttu-id="8a6af-134">String</span><span class="sxs-lookup"><span data-stu-id="8a6af-134">String</span></span>|<span data-ttu-id="8a6af-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8a6af-135">Key of the entity.</span></span>|
|<span data-ttu-id="8a6af-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8a6af-136">expirationDateTime</span></span>|<span data-ttu-id="8a6af-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a6af-137">DateTimeOffset</span></span>|<span data-ttu-id="8a6af-138">Optionales Profil Ablaufdatum und-Zeit.</span><span class="sxs-lookup"><span data-stu-id="8a6af-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="8a6af-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="8a6af-139">payloadFileName</span></span>|<span data-ttu-id="8a6af-140">String</span><span class="sxs-lookup"><span data-stu-id="8a6af-140">String</span></span>|<span data-ttu-id="8a6af-141">Der Dateiname (\*.mobileprovision Nutzlast</span><span class="sxs-lookup"><span data-stu-id="8a6af-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="8a6af-142">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="8a6af-142">\*.xml).</span></span>|
|<span data-ttu-id="8a6af-143">payload</span><span class="sxs-lookup"><span data-stu-id="8a6af-143">payload</span></span>|<span data-ttu-id="8a6af-144">Binär</span><span class="sxs-lookup"><span data-stu-id="8a6af-144">Binary</span></span>|<span data-ttu-id="8a6af-145">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="8a6af-145">Payload.</span></span> <span data-ttu-id="8a6af-146">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="8a6af-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="8a6af-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a6af-147">createdDateTime</span></span>|<span data-ttu-id="8a6af-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a6af-148">DateTimeOffset</span></span>|<span data-ttu-id="8a6af-149">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="8a6af-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="8a6af-150">description</span><span class="sxs-lookup"><span data-stu-id="8a6af-150">description</span></span>|<span data-ttu-id="8a6af-151">String</span><span class="sxs-lookup"><span data-stu-id="8a6af-151">String</span></span>|<span data-ttu-id="8a6af-152">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="8a6af-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="8a6af-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a6af-153">lastModifiedDateTime</span></span>|<span data-ttu-id="8a6af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a6af-154">DateTimeOffset</span></span>|<span data-ttu-id="8a6af-155">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8a6af-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8a6af-156">displayName</span><span class="sxs-lookup"><span data-stu-id="8a6af-156">displayName</span></span>|<span data-ttu-id="8a6af-157">String</span><span class="sxs-lookup"><span data-stu-id="8a6af-157">String</span></span>|<span data-ttu-id="8a6af-158">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="8a6af-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="8a6af-159">version</span><span class="sxs-lookup"><span data-stu-id="8a6af-159">version</span></span>|<span data-ttu-id="8a6af-160">Int32</span><span class="sxs-lookup"><span data-stu-id="8a6af-160">Int32</span></span>|<span data-ttu-id="8a6af-161">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8a6af-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="8a6af-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a6af-162">Response</span></span>
<span data-ttu-id="8a6af-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8a6af-163">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a6af-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a6af-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a6af-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a6af-165">Request</span></span>
<span data-ttu-id="8a6af-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a6af-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 304

{
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="8a6af-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a6af-167">Response</span></span>
<span data-ttu-id="8a6af-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a6af-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





