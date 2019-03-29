---
title: EmbeddedSIMDeviceState erstellen
description: Erstellen eines neuen embeddedSIMDeviceState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8472694638770964853f7d7e3e00480d472f7767
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965697"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="38af1-103">EmbeddedSIMDeviceState erstellen</span><span class="sxs-lookup"><span data-stu-id="38af1-103">Create embeddedSIMDeviceState</span></span>

> <span data-ttu-id="38af1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="38af1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38af1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="38af1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38af1-106">Erstellen eines neuen [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="38af1-106">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38af1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="38af1-107">Prerequisites</span></span>
<span data-ttu-id="38af1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38af1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38af1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38af1-110">Permission type</span></span>|<span data-ttu-id="38af1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38af1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38af1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38af1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38af1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38af1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38af1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38af1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38af1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38af1-115">Not supported.</span></span>|
|<span data-ttu-id="38af1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38af1-116">Application</span></span>|<span data-ttu-id="38af1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38af1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38af1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38af1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="38af1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38af1-119">Request headers</span></span>
|<span data-ttu-id="38af1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="38af1-120">Header</span></span>|<span data-ttu-id="38af1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="38af1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38af1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38af1-122">Authorization</span></span>|<span data-ttu-id="38af1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="38af1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38af1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="38af1-124">Accept</span></span>|<span data-ttu-id="38af1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38af1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38af1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38af1-126">Request body</span></span>
<span data-ttu-id="38af1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das embeddedSIMDeviceState-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="38af1-127">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="38af1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der embeddedSIMDeviceState erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="38af1-128">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="38af1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38af1-129">Property</span></span>|<span data-ttu-id="38af1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="38af1-130">Type</span></span>|<span data-ttu-id="38af1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38af1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38af1-132">id</span><span class="sxs-lookup"><span data-stu-id="38af1-132">id</span></span>|<span data-ttu-id="38af1-133">String</span><span class="sxs-lookup"><span data-stu-id="38af1-133">String</span></span>|<span data-ttu-id="38af1-134">Eindeutiger Bezeichner für den Status des eingebetteten SIM-Geräts.</span><span class="sxs-lookup"><span data-stu-id="38af1-134">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="38af1-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="38af1-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="38af1-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38af1-136">createdDateTime</span></span>|<span data-ttu-id="38af1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38af1-137">DateTimeOffset</span></span>|<span data-ttu-id="38af1-138">Der Zeitpunkt, zu dem der Status des eingebetteten SIM-Geräts erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="38af1-138">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="38af1-139">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="38af1-139">Generated service side.</span></span>|
|<span data-ttu-id="38af1-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38af1-140">modifiedDateTime</span></span>|<span data-ttu-id="38af1-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38af1-141">DateTimeOffset</span></span>|<span data-ttu-id="38af1-142">Zeitpunkt, zu dem der Status des eingebetteten SIM-Geräts zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="38af1-142">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="38af1-143">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="38af1-143">Updated service side.</span></span>|
|<span data-ttu-id="38af1-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="38af1-144">lastSyncDateTime</span></span>|<span data-ttu-id="38af1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38af1-145">DateTimeOffset</span></span>|<span data-ttu-id="38af1-146">Zeitpunkt, zu dem das eingebettete SIM-Gerät zuletzt eingecheckt hat.</span><span class="sxs-lookup"><span data-stu-id="38af1-146">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="38af1-147">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="38af1-147">Updated service side.</span></span>|
|<span data-ttu-id="38af1-148">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="38af1-148">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="38af1-149">String</span><span class="sxs-lookup"><span data-stu-id="38af1-149">String</span></span>|<span data-ttu-id="38af1-150">Der universelle integrierte Leiterkarten Bezeichner (UICCID), der die Hardware identifiziert, auf der ein Profil bereitgestellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="38af1-150">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="38af1-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="38af1-151">deviceName</span></span>|<span data-ttu-id="38af1-152">String</span><span class="sxs-lookup"><span data-stu-id="38af1-152">String</span></span>|<span data-ttu-id="38af1-153">Gerätename, für den das Abonnement vorgesehen wurde (z. b. DESKTOP-JOE)</span><span class="sxs-lookup"><span data-stu-id="38af1-153">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="38af1-154">userName</span><span class="sxs-lookup"><span data-stu-id="38af1-154">userName</span></span>|<span data-ttu-id="38af1-155">String</span><span class="sxs-lookup"><span data-stu-id="38af1-155">String</span></span>|<span data-ttu-id="38af1-156">Benutzername, für den das Abonnement z. b. joe@contoso.com wurde</span><span class="sxs-lookup"><span data-stu-id="38af1-156">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="38af1-157">state</span><span class="sxs-lookup"><span data-stu-id="38af1-157">state</span></span>|[<span data-ttu-id="38af1-158">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="38af1-158">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="38af1-159">Der Status des auf das Gerät angewendeten Profil Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="38af1-159">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="38af1-160">Mögliche Werte: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="38af1-160">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="38af1-161">stateDetails</span><span class="sxs-lookup"><span data-stu-id="38af1-161">stateDetails</span></span>|<span data-ttu-id="38af1-162">String</span><span class="sxs-lookup"><span data-stu-id="38af1-162">String</span></span>|<span data-ttu-id="38af1-163">Beschreibung des Zustands der Einrichtung.</span><span class="sxs-lookup"><span data-stu-id="38af1-163">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="38af1-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="38af1-164">Response</span></span>
<span data-ttu-id="38af1-165">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="38af1-165">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38af1-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38af1-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="38af1-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38af1-167">Request</span></span>
<span data-ttu-id="38af1-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38af1-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="38af1-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="38af1-169">Response</span></span>
<span data-ttu-id="38af1-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38af1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```




