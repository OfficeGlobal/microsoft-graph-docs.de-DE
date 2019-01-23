---
title: Erstellen von embeddedSIMDeviceState
description: Erstellen eines neuen EmbeddedSIMDeviceState-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 451f40d7ad23787311e4a0b9ed3c046cbe34b830
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413416"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="c757a-103">Erstellen von embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="c757a-103">Create embeddedSIMDeviceState</span></span>

> <span data-ttu-id="c757a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c757a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c757a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c757a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c757a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c757a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c757a-107">Erstellen eines neuen [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c757a-107">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c757a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c757a-108">Prerequisites</span></span>
<span data-ttu-id="c757a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c757a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c757a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c757a-111">Permission type</span></span>|<span data-ttu-id="c757a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c757a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c757a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c757a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c757a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c757a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c757a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c757a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c757a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c757a-116">Not supported.</span></span>|
|<span data-ttu-id="c757a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c757a-117">Application</span></span>|<span data-ttu-id="c757a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c757a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c757a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c757a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="c757a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c757a-120">Request headers</span></span>
|<span data-ttu-id="c757a-121">Header</span><span class="sxs-lookup"><span data-stu-id="c757a-121">Header</span></span>|<span data-ttu-id="c757a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c757a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c757a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c757a-123">Authorization</span></span>|<span data-ttu-id="c757a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c757a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c757a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c757a-125">Accept</span></span>|<span data-ttu-id="c757a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c757a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c757a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c757a-127">Request body</span></span>
<span data-ttu-id="c757a-128">Geben Sie im Textkörper Anforderung für das Objekt EmbeddedSIMDeviceState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c757a-128">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="c757a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die EmbeddedSIMDeviceState erstellen.</span><span class="sxs-lookup"><span data-stu-id="c757a-129">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="c757a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c757a-130">Property</span></span>|<span data-ttu-id="c757a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c757a-131">Type</span></span>|<span data-ttu-id="c757a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c757a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c757a-133">id</span><span class="sxs-lookup"><span data-stu-id="c757a-133">id</span></span>|<span data-ttu-id="c757a-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c757a-134">String</span></span>|<span data-ttu-id="c757a-135">Eindeutiger Bezeichner für die eingebettete SIM Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="c757a-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="c757a-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="c757a-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="c757a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c757a-137">createdDateTime</span></span>|<span data-ttu-id="c757a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c757a-138">DateTimeOffset</span></span>|<span data-ttu-id="c757a-139">Der Zeitpunkt der eingebetteten SIM Gerätestatus erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c757a-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="c757a-140">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="c757a-140">Generated service side.</span></span>|
|<span data-ttu-id="c757a-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c757a-141">modifiedDateTime</span></span>|<span data-ttu-id="c757a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c757a-142">DateTimeOffset</span></span>|<span data-ttu-id="c757a-143">Der Zeitpunkt der letzten Änderung der eingebetteten SIM Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="c757a-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="c757a-144">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="c757a-144">Updated service side.</span></span>|
|<span data-ttu-id="c757a-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c757a-145">lastSyncDateTime</span></span>|<span data-ttu-id="c757a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c757a-146">DateTimeOffset</span></span>|<span data-ttu-id="c757a-147">Zeitpunkt, zu das eingebettete SIM Gerät zuletzt eingecheckt.</span><span class="sxs-lookup"><span data-stu-id="c757a-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="c757a-148">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="c757a-148">Updated service side.</span></span>|
|<span data-ttu-id="c757a-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="c757a-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="c757a-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c757a-150">String</span></span>|<span data-ttu-id="c757a-151">Der universelle Chip Karte Bezeichner (UICCID), identifiziert der Hardware, auf der ein Profil ist bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="c757a-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="c757a-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="c757a-152">deviceName</span></span>|<span data-ttu-id="c757a-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c757a-153">String</span></span>|<span data-ttu-id="c757a-154">Name des Aufnahmegeräts, dem das Abonnement wurde, bereitgestellt, z. B. DESKTOP JOE</span><span class="sxs-lookup"><span data-stu-id="c757a-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="c757a-155">userName</span><span class="sxs-lookup"><span data-stu-id="c757a-155">userName</span></span>|<span data-ttu-id="c757a-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c757a-156">String</span></span>|<span data-ttu-id="c757a-157">Benutzernamen, der das Abonnement, z. B. joe@contoso.com bereitgestellt wurde</span><span class="sxs-lookup"><span data-stu-id="c757a-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="c757a-158">Zustand</span><span class="sxs-lookup"><span data-stu-id="c757a-158">state</span></span>|[<span data-ttu-id="c757a-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="c757a-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="c757a-160">Der Status des Vorgangs Profil angewendet auf das Gerät.</span><span class="sxs-lookup"><span data-stu-id="c757a-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="c757a-161">Mögliche Werte sind: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted` und `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="c757a-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="c757a-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="c757a-162">stateDetails</span></span>|<span data-ttu-id="c757a-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c757a-163">String</span></span>|<span data-ttu-id="c757a-164">Beschreibung des provisioning Status eine Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="c757a-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="c757a-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="c757a-165">Response</span></span>
<span data-ttu-id="c757a-166">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c757a-166">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c757a-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c757a-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="c757a-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c757a-168">Request</span></span>
<span data-ttu-id="c757a-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c757a-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c757a-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="c757a-170">Response</span></span>
<span data-ttu-id="c757a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c757a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




