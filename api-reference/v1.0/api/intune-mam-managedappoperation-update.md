---
title: Aktualisieren von „managedAppOperation“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75752874f78d1f1044e50219dede240e00f0a441
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250194"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="1f04c-103">Aktualisieren von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="1f04c-103">Update managedAppOperation</span></span>

> <span data-ttu-id="1f04c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1f04c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f04c-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="1f04c-105">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f04c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1f04c-106">Prerequisites</span></span>
<span data-ttu-id="1f04c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f04c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1f04c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f04c-109">Permission type</span></span>|<span data-ttu-id="1f04c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f04c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f04c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f04c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f04c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f04c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1f04c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f04c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f04c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f04c-114">Not supported.</span></span>|
|<span data-ttu-id="1f04c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f04c-115">Application</span></span>|<span data-ttu-id="1f04c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f04c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f04c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f04c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="1f04c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f04c-118">Request headers</span></span>
|<span data-ttu-id="1f04c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1f04c-119">Header</span></span>|<span data-ttu-id="1f04c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1f04c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f04c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f04c-121">Authorization</span></span>|<span data-ttu-id="1f04c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1f04c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f04c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1f04c-123">Accept</span></span>|<span data-ttu-id="1f04c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1f04c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f04c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f04c-125">Request body</span></span>
<span data-ttu-id="1f04c-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) an.</span><span class="sxs-lookup"><span data-stu-id="1f04c-126">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="1f04c-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1f04c-127">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="1f04c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f04c-128">Property</span></span>|<span data-ttu-id="1f04c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1f04c-129">Type</span></span>|<span data-ttu-id="1f04c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f04c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f04c-131">displayName</span><span class="sxs-lookup"><span data-stu-id="1f04c-131">displayName</span></span>|<span data-ttu-id="1f04c-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f04c-132">String</span></span>|<span data-ttu-id="1f04c-133">Name des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="1f04c-133">The operation name.</span></span>|
|<span data-ttu-id="1f04c-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f04c-134">lastModifiedDateTime</span></span>|<span data-ttu-id="1f04c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f04c-135">DateTimeOffset</span></span>|<span data-ttu-id="1f04c-136">Datum und Uhrzeit der letzten Änderung des App-Vorgangs</span><span class="sxs-lookup"><span data-stu-id="1f04c-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="1f04c-137">state</span><span class="sxs-lookup"><span data-stu-id="1f04c-137">state</span></span>|<span data-ttu-id="1f04c-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f04c-138">String</span></span>|<span data-ttu-id="1f04c-139">Aktueller Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="1f04c-139">The current state of the operation</span></span>|
|<span data-ttu-id="1f04c-140">id</span><span class="sxs-lookup"><span data-stu-id="1f04c-140">id</span></span>|<span data-ttu-id="1f04c-141">string</span><span class="sxs-lookup"><span data-stu-id="1f04c-141">String</span></span>|<span data-ttu-id="1f04c-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1f04c-142">Key of the entity.</span></span>|
|<span data-ttu-id="1f04c-143">Version</span><span class="sxs-lookup"><span data-stu-id="1f04c-143">version</span></span>|<span data-ttu-id="1f04c-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f04c-144">String</span></span>|<span data-ttu-id="1f04c-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="1f04c-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1f04c-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f04c-146">Response</span></span>
<span data-ttu-id="1f04c-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1f04c-147">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f04c-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f04c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f04c-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f04c-149">Request</span></span>
<span data-ttu-id="1f04c-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f04c-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f04c-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f04c-151">Response</span></span>
<span data-ttu-id="1f04c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f04c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



