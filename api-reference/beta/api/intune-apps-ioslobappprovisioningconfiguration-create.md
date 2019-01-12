---
title: Erstellen von iosLobAppProvisioningConfiguration
description: Erstellen eines neuen IosLobAppProvisioningConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d5a39a91156ebba649a3463568517d9b55a7fdfa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944761"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="dbd2d-103">Erstellen von iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="dbd2d-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="dbd2d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbd2d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbd2d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbd2d-107">Erstellen eines neuen [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dbd2d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dbd2d-108">Prerequisites</span></span>
<span data-ttu-id="dbd2d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbd2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbd2d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dbd2d-111">Permission type</span></span>|<span data-ttu-id="dbd2d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dbd2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbd2d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dbd2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbd2d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbd2d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dbd2d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dbd2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbd2d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dbd2d-116">Not supported.</span></span>|
|<span data-ttu-id="dbd2d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dbd2d-117">Application</span></span>|<span data-ttu-id="dbd2d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dbd2d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbd2d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dbd2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dbd2d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dbd2d-120">Request headers</span></span>
|<span data-ttu-id="dbd2d-121">Header</span><span class="sxs-lookup"><span data-stu-id="dbd2d-121">Header</span></span>|<span data-ttu-id="dbd2d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dbd2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbd2d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbd2d-123">Authorization</span></span>|<span data-ttu-id="dbd2d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dbd2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbd2d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dbd2d-125">Accept</span></span>|<span data-ttu-id="dbd2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbd2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbd2d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dbd2d-127">Request body</span></span>
<span data-ttu-id="dbd2d-128">Geben Sie im Textkörper Anforderung für das Objekt IosLobAppProvisioningConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="dbd2d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosLobAppProvisioningConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="dbd2d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dbd2d-130">Property</span></span>|<span data-ttu-id="dbd2d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="dbd2d-131">Type</span></span>|<span data-ttu-id="dbd2d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbd2d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbd2d-133">id</span><span class="sxs-lookup"><span data-stu-id="dbd2d-133">id</span></span>|<span data-ttu-id="dbd2d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbd2d-134">String</span></span>|<span data-ttu-id="dbd2d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dbd2d-135">Key of the entity.</span></span>|
|<span data-ttu-id="dbd2d-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dbd2d-136">expirationDateTime</span></span>|<span data-ttu-id="dbd2d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbd2d-137">DateTimeOffset</span></span>|<span data-ttu-id="dbd2d-138">Optionales Profil Ablaufdatum und-Zeit.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="dbd2d-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="dbd2d-139">payloadFileName</span></span>|<span data-ttu-id="dbd2d-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbd2d-140">String</span></span>|<span data-ttu-id="dbd2d-141">Der Dateiname (\*.mobileprovision Nutzlast</span><span class="sxs-lookup"><span data-stu-id="dbd2d-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="dbd2d-142">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="dbd2d-142">\*.xml).</span></span>|
|<span data-ttu-id="dbd2d-143">payload</span><span class="sxs-lookup"><span data-stu-id="dbd2d-143">payload</span></span>|<span data-ttu-id="dbd2d-144">Binär</span><span class="sxs-lookup"><span data-stu-id="dbd2d-144">Binary</span></span>|<span data-ttu-id="dbd2d-145">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="dbd2d-145">Payload.</span></span> <span data-ttu-id="dbd2d-146">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="dbd2d-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="dbd2d-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dbd2d-147">createdDateTime</span></span>|<span data-ttu-id="dbd2d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbd2d-148">DateTimeOffset</span></span>|<span data-ttu-id="dbd2d-149">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="dbd2d-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="dbd2d-150">description</span><span class="sxs-lookup"><span data-stu-id="dbd2d-150">description</span></span>|<span data-ttu-id="dbd2d-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbd2d-151">String</span></span>|<span data-ttu-id="dbd2d-152">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="dbd2d-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="dbd2d-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbd2d-153">lastModifiedDateTime</span></span>|<span data-ttu-id="dbd2d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbd2d-154">DateTimeOffset</span></span>|<span data-ttu-id="dbd2d-155">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="dbd2d-156">displayName</span><span class="sxs-lookup"><span data-stu-id="dbd2d-156">displayName</span></span>|<span data-ttu-id="dbd2d-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbd2d-157">String</span></span>|<span data-ttu-id="dbd2d-158">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="dbd2d-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="dbd2d-159">version</span><span class="sxs-lookup"><span data-stu-id="dbd2d-159">version</span></span>|<span data-ttu-id="dbd2d-160">Int32</span><span class="sxs-lookup"><span data-stu-id="dbd2d-160">Int32</span></span>|<span data-ttu-id="dbd2d-161">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="dbd2d-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="dbd2d-162">Response</span></span>
<span data-ttu-id="dbd2d-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-163">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbd2d-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dbd2d-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="dbd2d-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dbd2d-165">Request</span></span>
<span data-ttu-id="dbd2d-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
Content-type: application/json
Content-length: 377

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="dbd2d-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="dbd2d-167">Response</span></span>
<span data-ttu-id="dbd2d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dbd2d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





