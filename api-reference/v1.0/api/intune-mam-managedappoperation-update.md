---
title: Aktualisieren von „managedAppOperation“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52ff91c1db2d20a484b7bf1f8bde282007ea9485
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978472"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="72e56-103">Aktualisieren von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="72e56-103">Update managedAppOperation</span></span>

> <span data-ttu-id="72e56-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="72e56-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72e56-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="72e56-105">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72e56-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="72e56-106">Prerequisites</span></span>
<span data-ttu-id="72e56-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72e56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72e56-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="72e56-109">Permission type</span></span>|<span data-ttu-id="72e56-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="72e56-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72e56-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="72e56-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72e56-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72e56-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="72e56-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="72e56-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72e56-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72e56-114">Not supported.</span></span>|
|<span data-ttu-id="72e56-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="72e56-115">Application</span></span>|<span data-ttu-id="72e56-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72e56-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72e56-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="72e56-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="72e56-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="72e56-118">Request headers</span></span>
|<span data-ttu-id="72e56-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="72e56-119">Header</span></span>|<span data-ttu-id="72e56-120">Wert</span><span class="sxs-lookup"><span data-stu-id="72e56-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72e56-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="72e56-121">Authorization</span></span>|<span data-ttu-id="72e56-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="72e56-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72e56-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="72e56-123">Accept</span></span>|<span data-ttu-id="72e56-124">application/json</span><span class="sxs-lookup"><span data-stu-id="72e56-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72e56-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="72e56-125">Request body</span></span>
<span data-ttu-id="72e56-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) an.</span><span class="sxs-lookup"><span data-stu-id="72e56-126">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="72e56-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="72e56-127">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="72e56-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72e56-128">Property</span></span>|<span data-ttu-id="72e56-129">Typ</span><span class="sxs-lookup"><span data-stu-id="72e56-129">Type</span></span>|<span data-ttu-id="72e56-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72e56-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72e56-131">displayName</span><span class="sxs-lookup"><span data-stu-id="72e56-131">displayName</span></span>|<span data-ttu-id="72e56-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72e56-132">String</span></span>|<span data-ttu-id="72e56-133">Name des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="72e56-133">The operation name.</span></span>|
|<span data-ttu-id="72e56-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72e56-134">lastModifiedDateTime</span></span>|<span data-ttu-id="72e56-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72e56-135">DateTimeOffset</span></span>|<span data-ttu-id="72e56-136">Datum und Uhrzeit der letzten Änderung des App-Vorgangs</span><span class="sxs-lookup"><span data-stu-id="72e56-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="72e56-137">state</span><span class="sxs-lookup"><span data-stu-id="72e56-137">state</span></span>|<span data-ttu-id="72e56-138">String</span><span class="sxs-lookup"><span data-stu-id="72e56-138">String</span></span>|<span data-ttu-id="72e56-139">Aktueller Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="72e56-139">The current state of the operation</span></span>|
|<span data-ttu-id="72e56-140">id</span><span class="sxs-lookup"><span data-stu-id="72e56-140">id</span></span>|<span data-ttu-id="72e56-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72e56-141">String</span></span>|<span data-ttu-id="72e56-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="72e56-142">Key of the entity.</span></span>|
|<span data-ttu-id="72e56-143">Version</span><span class="sxs-lookup"><span data-stu-id="72e56-143">version</span></span>|<span data-ttu-id="72e56-144">String</span><span class="sxs-lookup"><span data-stu-id="72e56-144">String</span></span>|<span data-ttu-id="72e56-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="72e56-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="72e56-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="72e56-146">Response</span></span>
<span data-ttu-id="72e56-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="72e56-147">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72e56-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="72e56-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="72e56-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="72e56-149">Request</span></span>
<span data-ttu-id="72e56-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="72e56-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="72e56-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="72e56-151">Response</span></span>
<span data-ttu-id="72e56-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="72e56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



