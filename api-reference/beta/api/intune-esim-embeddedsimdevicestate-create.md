---
title: EmbeddedSIMDeviceState erstellen
description: Erstellen eines neuen embeddedSIMDeviceState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d7ad1aa42f0cdeec9390d518491a02af346207b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175255"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="4bdbb-103">EmbeddedSIMDeviceState erstellen</span><span class="sxs-lookup"><span data-stu-id="4bdbb-103">Create embeddedSIMDeviceState</span></span>

> <span data-ttu-id="4bdbb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bdbb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bdbb-106">Erstellen eines neuen [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-106">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bdbb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4bdbb-107">Prerequisites</span></span>
<span data-ttu-id="4bdbb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bdbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4bdbb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4bdbb-110">Permission type</span></span>|<span data-ttu-id="4bdbb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4bdbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bdbb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4bdbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4bdbb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bdbb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4bdbb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4bdbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bdbb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bdbb-115">Not supported.</span></span>|
|<span data-ttu-id="4bdbb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4bdbb-116">Application</span></span>|<span data-ttu-id="4bdbb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bdbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bdbb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bdbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="4bdbb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4bdbb-119">Request headers</span></span>
|<span data-ttu-id="4bdbb-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4bdbb-120">Header</span></span>|<span data-ttu-id="4bdbb-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4bdbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bdbb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bdbb-122">Authorization</span></span>|<span data-ttu-id="4bdbb-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4bdbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bdbb-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4bdbb-124">Accept</span></span>|<span data-ttu-id="4bdbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4bdbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bdbb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4bdbb-126">Request body</span></span>
<span data-ttu-id="4bdbb-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das embeddedSIMDeviceState-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-127">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="4bdbb-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der embeddedSIMDeviceState erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-128">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="4bdbb-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4bdbb-129">Property</span></span>|<span data-ttu-id="4bdbb-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4bdbb-130">Type</span></span>|<span data-ttu-id="4bdbb-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bdbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bdbb-132">id</span><span class="sxs-lookup"><span data-stu-id="4bdbb-132">id</span></span>|<span data-ttu-id="4bdbb-133">String</span><span class="sxs-lookup"><span data-stu-id="4bdbb-133">String</span></span>|<span data-ttu-id="4bdbb-134">Eindeutiger Bezeichner für den Status des eingebetteten SIM-Geräts.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-134">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="4bdbb-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="4bdbb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4bdbb-136">createdDateTime</span></span>|<span data-ttu-id="4bdbb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bdbb-137">DateTimeOffset</span></span>|<span data-ttu-id="4bdbb-138">Der Zeitpunkt, zu dem der Status des eingebetteten SIM-Geräts erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-138">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="4bdbb-139">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-139">Generated service side.</span></span>|
|<span data-ttu-id="4bdbb-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bdbb-140">modifiedDateTime</span></span>|<span data-ttu-id="4bdbb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bdbb-141">DateTimeOffset</span></span>|<span data-ttu-id="4bdbb-142">Zeitpunkt, zu dem der Status des eingebetteten SIM-Geräts zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-142">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="4bdbb-143">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-143">Updated service side.</span></span>|
|<span data-ttu-id="4bdbb-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4bdbb-144">lastSyncDateTime</span></span>|<span data-ttu-id="4bdbb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bdbb-145">DateTimeOffset</span></span>|<span data-ttu-id="4bdbb-146">Zeitpunkt, zu dem das eingebettete SIM-Gerät zuletzt eingecheckt hat.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-146">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="4bdbb-147">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-147">Updated service side.</span></span>|
|<span data-ttu-id="4bdbb-148">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="4bdbb-148">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="4bdbb-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4bdbb-149">String</span></span>|<span data-ttu-id="4bdbb-150">Der universelle integrierte Leiterkarten Bezeichner (UICCID), der die Hardware identifiziert, auf der ein Profil bereitgestellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-150">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="4bdbb-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="4bdbb-151">deviceName</span></span>|<span data-ttu-id="4bdbb-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4bdbb-152">String</span></span>|<span data-ttu-id="4bdbb-153">Gerätename, für den das Abonnement vorgesehen wurde (z. b. DESKTOP-JOE)</span><span class="sxs-lookup"><span data-stu-id="4bdbb-153">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="4bdbb-154">userName</span><span class="sxs-lookup"><span data-stu-id="4bdbb-154">userName</span></span>|<span data-ttu-id="4bdbb-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4bdbb-155">String</span></span>|<span data-ttu-id="4bdbb-156">Benutzername, für den das Abonnement z. b. joe@contoso.com wurde</span><span class="sxs-lookup"><span data-stu-id="4bdbb-156">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="4bdbb-157">state</span><span class="sxs-lookup"><span data-stu-id="4bdbb-157">state</span></span>|[<span data-ttu-id="4bdbb-158">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="4bdbb-158">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="4bdbb-159">Der Status des auf das Gerät angewendeten Profil Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-159">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="4bdbb-160">Mögliche Werte sind: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted` und `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-160">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="4bdbb-161">stateDetails</span><span class="sxs-lookup"><span data-stu-id="4bdbb-161">stateDetails</span></span>|<span data-ttu-id="4bdbb-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4bdbb-162">String</span></span>|<span data-ttu-id="4bdbb-163">Beschreibung des Zustands der Einrichtung.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-163">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="4bdbb-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bdbb-164">Response</span></span>
<span data-ttu-id="4bdbb-165">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-165">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bdbb-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4bdbb-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bdbb-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bdbb-167">Request</span></span>
<span data-ttu-id="4bdbb-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4bdbb-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bdbb-169">Response</span></span>
<span data-ttu-id="4bdbb-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4bdbb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




