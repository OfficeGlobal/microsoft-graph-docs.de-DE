---
title: EmbeddedSIMDeviceState aktualisieren
description: Aktualisieren Sie die Eigenschaften eines EmbeddedSIMDeviceState-Objekts.
ms.openlocfilehash: 5a102bd686a65cf14bb078e1ae66df31bbe4dae5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059832"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="7a4d2-103">EmbeddedSIMDeviceState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7a4d2-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="7a4d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a4d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a4d2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a4d2-107">Aktualisieren Sie die Eigenschaften eines [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a4d2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a4d2-108">Prerequisites</span></span>
<span data-ttu-id="7a4d2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a4d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a4d2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a4d2-111">Permission type</span></span>|<span data-ttu-id="7a4d2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a4d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a4d2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a4d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a4d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a4d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a4d2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a4d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a4d2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a4d2-116">Not supported.</span></span>|
|<span data-ttu-id="7a4d2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a4d2-117">Application</span></span>|<span data-ttu-id="7a4d2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a4d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a4d2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a4d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7a4d2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a4d2-120">Request headers</span></span>
|<span data-ttu-id="7a4d2-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7a4d2-121">Header</span></span>|<span data-ttu-id="7a4d2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7a4d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a4d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a4d2-123">Authorization</span></span>|<span data-ttu-id="7a4d2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a4d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a4d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a4d2-125">Accept</span></span>|<span data-ttu-id="7a4d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a4d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a4d2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a4d2-127">Request body</span></span>
<span data-ttu-id="7a4d2-128">Geben Sie im Textkörper Anforderung für das Objekt [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="7a4d2-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="7a4d2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7a4d2-130">Property</span></span>|<span data-ttu-id="7a4d2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7a4d2-131">Type</span></span>|<span data-ttu-id="7a4d2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a4d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a4d2-133">id</span><span class="sxs-lookup"><span data-stu-id="7a4d2-133">id</span></span>|<span data-ttu-id="7a4d2-134">String</span><span class="sxs-lookup"><span data-stu-id="7a4d2-134">String</span></span>|<span data-ttu-id="7a4d2-135">Eindeutiger Bezeichner für die eingebettete SIM Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="7a4d2-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="7a4d2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a4d2-137">createdDateTime</span></span>|<span data-ttu-id="7a4d2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a4d2-138">DateTimeOffset</span></span>|<span data-ttu-id="7a4d2-139">Der Zeitpunkt der eingebetteten SIM Gerätestatus erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="7a4d2-140">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-140">Generated service side.</span></span>|
|<span data-ttu-id="7a4d2-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a4d2-141">modifiedDateTime</span></span>|<span data-ttu-id="7a4d2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a4d2-142">DateTimeOffset</span></span>|<span data-ttu-id="7a4d2-143">Der Zeitpunkt der letzten Änderung der eingebetteten SIM Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="7a4d2-144">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-144">Updated service side.</span></span>|
|<span data-ttu-id="7a4d2-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7a4d2-145">lastSyncDateTime</span></span>|<span data-ttu-id="7a4d2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a4d2-146">DateTimeOffset</span></span>|<span data-ttu-id="7a4d2-147">Zeitpunkt, zu das eingebettete SIM Gerät zuletzt eingecheckt.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="7a4d2-148">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-148">Updated service side.</span></span>|
|<span data-ttu-id="7a4d2-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="7a4d2-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="7a4d2-150">String</span><span class="sxs-lookup"><span data-stu-id="7a4d2-150">String</span></span>|<span data-ttu-id="7a4d2-151">Der universelle Chip Karte Bezeichner (UICCID), identifiziert der Hardware, auf der ein Profil ist bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="7a4d2-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="7a4d2-152">deviceName</span></span>|<span data-ttu-id="7a4d2-153">String</span><span class="sxs-lookup"><span data-stu-id="7a4d2-153">String</span></span>|<span data-ttu-id="7a4d2-154">Name des Aufnahmegeräts, dem das Abonnement wurde, bereitgestellt, z. B. DESKTOP JOE</span><span class="sxs-lookup"><span data-stu-id="7a4d2-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="7a4d2-155">userName</span><span class="sxs-lookup"><span data-stu-id="7a4d2-155">userName</span></span>|<span data-ttu-id="7a4d2-156">String</span><span class="sxs-lookup"><span data-stu-id="7a4d2-156">String</span></span>|<span data-ttu-id="7a4d2-157">Benutzernamen, der das Abonnement, z. B. joe@contoso.com bereitgestellt wurde</span><span class="sxs-lookup"><span data-stu-id="7a4d2-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="7a4d2-158">state</span><span class="sxs-lookup"><span data-stu-id="7a4d2-158">state</span></span>|[<span data-ttu-id="7a4d2-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="7a4d2-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="7a4d2-160">Der Status des Vorgangs Profil angewendet auf das Gerät.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="7a4d2-161">Mögliche Werte sind: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted` und `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="7a4d2-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="7a4d2-162">stateDetails</span></span>|<span data-ttu-id="7a4d2-163">String</span><span class="sxs-lookup"><span data-stu-id="7a4d2-163">String</span></span>|<span data-ttu-id="7a4d2-164">Beschreibung des provisioning Status eine Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="7a4d2-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a4d2-165">Response</span></span>
<span data-ttu-id="7a4d2-166">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a4d2-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a4d2-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a4d2-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a4d2-168">Request</span></span>
<span data-ttu-id="7a4d2-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 300

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="7a4d2-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a4d2-170">Response</span></span>
<span data-ttu-id="7a4d2-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a4d2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





