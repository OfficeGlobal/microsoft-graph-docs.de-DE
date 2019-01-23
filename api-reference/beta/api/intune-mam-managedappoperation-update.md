---
title: Aktualisieren von „managedAppOperation“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedAppOperation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 376d54159b2b2eba7ca84d29fecf947cc4561bcb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401278"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="86368-103">Aktualisieren von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="86368-103">Update managedAppOperation</span></span>

> <span data-ttu-id="86368-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="86368-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86368-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="86368-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86368-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86368-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86368-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="86368-107">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86368-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="86368-108">Prerequisites</span></span>
<span data-ttu-id="86368-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="86368-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86368-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86368-111">Permission type</span></span>|<span data-ttu-id="86368-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86368-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86368-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86368-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86368-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86368-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="86368-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86368-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86368-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86368-116">Not supported.</span></span>|
|<span data-ttu-id="86368-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86368-117">Application</span></span>|<span data-ttu-id="86368-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86368-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86368-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86368-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="86368-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86368-120">Request headers</span></span>
|<span data-ttu-id="86368-121">Header</span><span class="sxs-lookup"><span data-stu-id="86368-121">Header</span></span>|<span data-ttu-id="86368-122">Wert</span><span class="sxs-lookup"><span data-stu-id="86368-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86368-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="86368-123">Authorization</span></span>|<span data-ttu-id="86368-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="86368-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86368-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="86368-125">Accept</span></span>|<span data-ttu-id="86368-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86368-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86368-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86368-127">Request body</span></span>
<span data-ttu-id="86368-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) an.</span><span class="sxs-lookup"><span data-stu-id="86368-128">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="86368-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="86368-129">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="86368-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86368-130">Property</span></span>|<span data-ttu-id="86368-131">Typ</span><span class="sxs-lookup"><span data-stu-id="86368-131">Type</span></span>|<span data-ttu-id="86368-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86368-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86368-133">displayName</span><span class="sxs-lookup"><span data-stu-id="86368-133">displayName</span></span>|<span data-ttu-id="86368-134">String</span><span class="sxs-lookup"><span data-stu-id="86368-134">String</span></span>|<span data-ttu-id="86368-135">Name des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="86368-135">The operation name.</span></span>|
|<span data-ttu-id="86368-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86368-136">lastModifiedDateTime</span></span>|<span data-ttu-id="86368-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86368-137">DateTimeOffset</span></span>|<span data-ttu-id="86368-138">Datum und Uhrzeit der letzten Änderung des App-Vorgangs</span><span class="sxs-lookup"><span data-stu-id="86368-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="86368-139">state</span><span class="sxs-lookup"><span data-stu-id="86368-139">state</span></span>|<span data-ttu-id="86368-140">String</span><span class="sxs-lookup"><span data-stu-id="86368-140">String</span></span>|<span data-ttu-id="86368-141">Aktueller Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="86368-141">The current state of the operation</span></span>|
|<span data-ttu-id="86368-142">id</span><span class="sxs-lookup"><span data-stu-id="86368-142">id</span></span>|<span data-ttu-id="86368-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86368-143">String</span></span>|<span data-ttu-id="86368-144">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="86368-144">Key of the entity.</span></span>|
|<span data-ttu-id="86368-145">Version</span><span class="sxs-lookup"><span data-stu-id="86368-145">version</span></span>|<span data-ttu-id="86368-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86368-146">String</span></span>|<span data-ttu-id="86368-147">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="86368-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="86368-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="86368-148">Response</span></span>
<span data-ttu-id="86368-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="86368-149">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86368-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86368-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="86368-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86368-151">Request</span></span>
<span data-ttu-id="86368-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86368-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86368-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="86368-153">Response</span></span>
<span data-ttu-id="86368-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86368-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




