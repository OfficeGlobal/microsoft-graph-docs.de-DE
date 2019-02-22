---
title: Aktualisieren von „managedAppOperation“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2af0440e8778860e6c70b2ad965ea96c9808ba9b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164659"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="5bd69-103">Aktualisieren von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="5bd69-103">Update managedAppOperation</span></span>

> <span data-ttu-id="5bd69-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5bd69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bd69-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5bd69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bd69-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="5bd69-106">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bd69-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5bd69-107">Prerequisites</span></span>
<span data-ttu-id="5bd69-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5bd69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5bd69-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5bd69-110">Permission type</span></span>|<span data-ttu-id="5bd69-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5bd69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bd69-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5bd69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5bd69-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bd69-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5bd69-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5bd69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bd69-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bd69-115">Not supported.</span></span>|
|<span data-ttu-id="5bd69-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5bd69-116">Application</span></span>|<span data-ttu-id="5bd69-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bd69-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bd69-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bd69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="5bd69-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5bd69-119">Request headers</span></span>
|<span data-ttu-id="5bd69-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5bd69-120">Header</span></span>|<span data-ttu-id="5bd69-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5bd69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bd69-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd69-122">Authorization</span></span>|<span data-ttu-id="5bd69-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5bd69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bd69-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5bd69-124">Accept</span></span>|<span data-ttu-id="5bd69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5bd69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bd69-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5bd69-126">Request body</span></span>
<span data-ttu-id="5bd69-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) an.</span><span class="sxs-lookup"><span data-stu-id="5bd69-127">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="5bd69-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5bd69-128">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="5bd69-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5bd69-129">Property</span></span>|<span data-ttu-id="5bd69-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5bd69-130">Type</span></span>|<span data-ttu-id="5bd69-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5bd69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bd69-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5bd69-132">displayName</span></span>|<span data-ttu-id="5bd69-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5bd69-133">String</span></span>|<span data-ttu-id="5bd69-134">Name des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="5bd69-134">The operation name.</span></span>|
|<span data-ttu-id="5bd69-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd69-135">lastModifiedDateTime</span></span>|<span data-ttu-id="5bd69-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd69-136">DateTimeOffset</span></span>|<span data-ttu-id="5bd69-137">Datum und Uhrzeit der letzten Änderung des App-Vorgangs</span><span class="sxs-lookup"><span data-stu-id="5bd69-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="5bd69-138">state</span><span class="sxs-lookup"><span data-stu-id="5bd69-138">state</span></span>|<span data-ttu-id="5bd69-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5bd69-139">String</span></span>|<span data-ttu-id="5bd69-140">Aktueller Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="5bd69-140">The current state of the operation</span></span>|
|<span data-ttu-id="5bd69-141">id</span><span class="sxs-lookup"><span data-stu-id="5bd69-141">id</span></span>|<span data-ttu-id="5bd69-142">string</span><span class="sxs-lookup"><span data-stu-id="5bd69-142">String</span></span>|<span data-ttu-id="5bd69-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5bd69-143">Key of the entity.</span></span>|
|<span data-ttu-id="5bd69-144">Version</span><span class="sxs-lookup"><span data-stu-id="5bd69-144">version</span></span>|<span data-ttu-id="5bd69-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5bd69-145">String</span></span>|<span data-ttu-id="5bd69-146">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="5bd69-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5bd69-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bd69-147">Response</span></span>
<span data-ttu-id="5bd69-148">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5bd69-148">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bd69-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5bd69-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bd69-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bd69-150">Request</span></span>
<span data-ttu-id="5bd69-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5bd69-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="5bd69-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bd69-152">Response</span></span>
<span data-ttu-id="5bd69-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bd69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




