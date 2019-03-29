---
title: AppLogCollectionRequest aktualisieren
description: Aktualisieren der Eigenschaften eines appLogCollectionRequest-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 81ac65687cabba41ee48c0e88e56428ac8735658
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962547"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="2af1d-103">AppLogCollectionRequest aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2af1d-103">Update appLogCollectionRequest</span></span>

> <span data-ttu-id="2af1d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2af1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2af1d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2af1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2af1d-106">Aktualisieren der Eigenschaften eines [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2af1d-106">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2af1d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2af1d-107">Prerequisites</span></span>
<span data-ttu-id="2af1d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2af1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2af1d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2af1d-110">Permission type</span></span>|<span data-ttu-id="2af1d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2af1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2af1d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2af1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2af1d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af1d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2af1d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2af1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2af1d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2af1d-115">Not supported.</span></span>|
|<span data-ttu-id="2af1d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2af1d-116">Application</span></span>|<span data-ttu-id="2af1d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2af1d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2af1d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2af1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="2af1d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2af1d-119">Request headers</span></span>
|<span data-ttu-id="2af1d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2af1d-120">Header</span></span>|<span data-ttu-id="2af1d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2af1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2af1d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2af1d-122">Authorization</span></span>|<span data-ttu-id="2af1d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2af1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2af1d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2af1d-124">Accept</span></span>|<span data-ttu-id="2af1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2af1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2af1d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2af1d-126">Request body</span></span>
<span data-ttu-id="2af1d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="2af1d-127">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="2af1d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2af1d-128">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="2af1d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2af1d-129">Property</span></span>|<span data-ttu-id="2af1d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2af1d-130">Type</span></span>|<span data-ttu-id="2af1d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2af1d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2af1d-132">id</span><span class="sxs-lookup"><span data-stu-id="2af1d-132">id</span></span>|<span data-ttu-id="2af1d-133">String</span><span class="sxs-lookup"><span data-stu-id="2af1d-133">String</span></span>|<span data-ttu-id="2af1d-134">Der eindeutige Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="2af1d-134">The unique Identifier.</span></span> <span data-ttu-id="2af1d-135">Dies ist userId_DeviceId_AppId-ID.</span><span class="sxs-lookup"><span data-stu-id="2af1d-135">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="2af1d-136">status</span><span class="sxs-lookup"><span data-stu-id="2af1d-136">status</span></span>|[<span data-ttu-id="2af1d-137">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="2af1d-137">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="2af1d-138">Protokoll Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="2af1d-138">Log upload status.</span></span> <span data-ttu-id="2af1d-139">Mögliche Werte sind: `pending`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="2af1d-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="2af1d-140">errorMessage</span><span class="sxs-lookup"><span data-stu-id="2af1d-140">errorMessage</span></span>|<span data-ttu-id="2af1d-141">String</span><span class="sxs-lookup"><span data-stu-id="2af1d-141">String</span></span>|<span data-ttu-id="2af1d-142">Fehlermeldung, falls vorhanden, während des Uploads</span><span class="sxs-lookup"><span data-stu-id="2af1d-142">Error message if any during the upload process</span></span>|
|<span data-ttu-id="2af1d-143">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="2af1d-143">customLogFolders</span></span>|<span data-ttu-id="2af1d-144">String collection</span><span class="sxs-lookup"><span data-stu-id="2af1d-144">String collection</span></span>|<span data-ttu-id="2af1d-145">Liste der Protokollordner.</span><span class="sxs-lookup"><span data-stu-id="2af1d-145">List of log folders.</span></span> |
|<span data-ttu-id="2af1d-146">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2af1d-146">completedDateTime</span></span>|<span data-ttu-id="2af1d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2af1d-147">DateTimeOffset</span></span>|<span data-ttu-id="2af1d-148">Zeitpunkt, zu dem die Upload-Protokollanforderung einen Terminalstatus erreicht hat</span><span class="sxs-lookup"><span data-stu-id="2af1d-148">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="2af1d-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="2af1d-149">Response</span></span>
<span data-ttu-id="2af1d-150">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2af1d-150">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2af1d-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2af1d-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="2af1d-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2af1d-152">Request</span></span>
<span data-ttu-id="2af1d-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2af1d-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
Content-type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```

### <a name="response"></a><span data-ttu-id="2af1d-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="2af1d-154">Response</span></span>
<span data-ttu-id="2af1d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2af1d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 306

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```




