---
title: Aktualisieren von „managedAppOperation“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedAppOperation.
author: tfitzmac
ms.openlocfilehash: 2bd0d326a4300bdae29484b547bbd5aa429728ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311977"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="79b9f-103">Aktualisieren von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="79b9f-103">Update managedAppOperation</span></span>

> <span data-ttu-id="79b9f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="79b9f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79b9f-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="79b9f-105">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79b9f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="79b9f-106">Prerequisites</span></span>
<span data-ttu-id="79b9f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79b9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79b9f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79b9f-109">Permission type</span></span>|<span data-ttu-id="79b9f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79b9f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79b9f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79b9f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79b9f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b9f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79b9f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79b9f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79b9f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79b9f-114">Not supported.</span></span>|
|<span data-ttu-id="79b9f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79b9f-115">Application</span></span>|<span data-ttu-id="79b9f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79b9f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79b9f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79b9f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="79b9f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79b9f-118">Request headers</span></span>
|<span data-ttu-id="79b9f-119">Header</span><span class="sxs-lookup"><span data-stu-id="79b9f-119">Header</span></span>|<span data-ttu-id="79b9f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="79b9f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79b9f-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="79b9f-121">Authorization</span></span>|<span data-ttu-id="79b9f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="79b9f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79b9f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="79b9f-123">Accept</span></span>|<span data-ttu-id="79b9f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79b9f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79b9f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79b9f-125">Request body</span></span>
<span data-ttu-id="79b9f-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) an.</span><span class="sxs-lookup"><span data-stu-id="79b9f-126">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="79b9f-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="79b9f-127">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="79b9f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79b9f-128">Property</span></span>|<span data-ttu-id="79b9f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="79b9f-129">Type</span></span>|<span data-ttu-id="79b9f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79b9f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79b9f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="79b9f-131">displayName</span></span>|<span data-ttu-id="79b9f-132">String</span><span class="sxs-lookup"><span data-stu-id="79b9f-132">String</span></span>|<span data-ttu-id="79b9f-133">Name des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="79b9f-133">The operation name.</span></span>|
|<span data-ttu-id="79b9f-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79b9f-134">lastModifiedDateTime</span></span>|<span data-ttu-id="79b9f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79b9f-135">DateTimeOffset</span></span>|<span data-ttu-id="79b9f-136">Datum und Uhrzeit der letzten Änderung des App-Vorgangs</span><span class="sxs-lookup"><span data-stu-id="79b9f-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="79b9f-137">state</span><span class="sxs-lookup"><span data-stu-id="79b9f-137">state</span></span>|<span data-ttu-id="79b9f-138">String</span><span class="sxs-lookup"><span data-stu-id="79b9f-138">String</span></span>|<span data-ttu-id="79b9f-139">Aktueller Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="79b9f-139">The current state of the operation</span></span>|
|<span data-ttu-id="79b9f-140">id</span><span class="sxs-lookup"><span data-stu-id="79b9f-140">id</span></span>|<span data-ttu-id="79b9f-141">String</span><span class="sxs-lookup"><span data-stu-id="79b9f-141">String</span></span>|<span data-ttu-id="79b9f-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="79b9f-142">Key of the entity.</span></span>|
|<span data-ttu-id="79b9f-143">Version</span><span class="sxs-lookup"><span data-stu-id="79b9f-143">version</span></span>|<span data-ttu-id="79b9f-144">String</span><span class="sxs-lookup"><span data-stu-id="79b9f-144">String</span></span>|<span data-ttu-id="79b9f-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="79b9f-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="79b9f-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="79b9f-146">Response</span></span>
<span data-ttu-id="79b9f-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="79b9f-147">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79b9f-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79b9f-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="79b9f-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79b9f-149">Request</span></span>
<span data-ttu-id="79b9f-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79b9f-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="79b9f-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="79b9f-151">Response</span></span>
<span data-ttu-id="79b9f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79b9f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



