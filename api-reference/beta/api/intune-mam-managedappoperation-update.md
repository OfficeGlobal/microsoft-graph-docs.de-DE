---
title: Aktualisieren von „managedAppOperation“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedAppOperation.
ms.openlocfilehash: 793b4eb48a0f70c0b1877aebd40969fba334e65e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062526"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="94aec-103">Aktualisieren von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="94aec-103">Update managedAppOperation</span></span>

> <span data-ttu-id="94aec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="94aec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94aec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94aec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94aec-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="94aec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94aec-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="94aec-107">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94aec-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="94aec-108">Prerequisites</span></span>
<span data-ttu-id="94aec-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94aec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94aec-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94aec-111">Permission type</span></span>|<span data-ttu-id="94aec-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94aec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94aec-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94aec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94aec-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94aec-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="94aec-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94aec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94aec-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94aec-116">Not supported.</span></span>|
|<span data-ttu-id="94aec-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94aec-117">Application</span></span>|<span data-ttu-id="94aec-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94aec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94aec-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94aec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="94aec-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94aec-120">Request headers</span></span>
|<span data-ttu-id="94aec-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="94aec-121">Header</span></span>|<span data-ttu-id="94aec-122">Wert</span><span class="sxs-lookup"><span data-stu-id="94aec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94aec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94aec-123">Authorization</span></span>|<span data-ttu-id="94aec-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="94aec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94aec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="94aec-125">Accept</span></span>|<span data-ttu-id="94aec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94aec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94aec-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94aec-127">Request body</span></span>
<span data-ttu-id="94aec-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) an.</span><span class="sxs-lookup"><span data-stu-id="94aec-128">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="94aec-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="94aec-129">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="94aec-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94aec-130">Property</span></span>|<span data-ttu-id="94aec-131">Typ</span><span class="sxs-lookup"><span data-stu-id="94aec-131">Type</span></span>|<span data-ttu-id="94aec-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94aec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94aec-133">displayName</span><span class="sxs-lookup"><span data-stu-id="94aec-133">displayName</span></span>|<span data-ttu-id="94aec-134">String</span><span class="sxs-lookup"><span data-stu-id="94aec-134">String</span></span>|<span data-ttu-id="94aec-135">Name des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="94aec-135">The operation name.</span></span>|
|<span data-ttu-id="94aec-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94aec-136">lastModifiedDateTime</span></span>|<span data-ttu-id="94aec-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94aec-137">DateTimeOffset</span></span>|<span data-ttu-id="94aec-138">Datum und Uhrzeit der letzten Änderung des App-Vorgangs</span><span class="sxs-lookup"><span data-stu-id="94aec-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="94aec-139">state</span><span class="sxs-lookup"><span data-stu-id="94aec-139">state</span></span>|<span data-ttu-id="94aec-140">String</span><span class="sxs-lookup"><span data-stu-id="94aec-140">String</span></span>|<span data-ttu-id="94aec-141">Aktueller Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="94aec-141">The current state of the operation</span></span>|
|<span data-ttu-id="94aec-142">id</span><span class="sxs-lookup"><span data-stu-id="94aec-142">id</span></span>|<span data-ttu-id="94aec-143">String</span><span class="sxs-lookup"><span data-stu-id="94aec-143">String</span></span>|<span data-ttu-id="94aec-144">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="94aec-144">Key of the entity.</span></span>|
|<span data-ttu-id="94aec-145">Version</span><span class="sxs-lookup"><span data-stu-id="94aec-145">version</span></span>|<span data-ttu-id="94aec-146">String</span><span class="sxs-lookup"><span data-stu-id="94aec-146">String</span></span>|<span data-ttu-id="94aec-147">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="94aec-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="94aec-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="94aec-148">Response</span></span>
<span data-ttu-id="94aec-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="94aec-149">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94aec-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94aec-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="94aec-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94aec-151">Request</span></span>
<span data-ttu-id="94aec-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94aec-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 165

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="94aec-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="94aec-153">Response</span></span>
<span data-ttu-id="94aec-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94aec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```





