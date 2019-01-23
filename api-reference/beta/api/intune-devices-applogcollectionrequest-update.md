---
title: AppLogCollectionRequest aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AppLogCollectionRequest-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55974ed3c5158d4b005402fe4d6350854a197656
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430136"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="92536-103">AppLogCollectionRequest aktualisieren</span><span class="sxs-lookup"><span data-stu-id="92536-103">Update appLogCollectionRequest</span></span>

> <span data-ttu-id="92536-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="92536-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="92536-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92536-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92536-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92536-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92536-107">Aktualisieren Sie die Eigenschaften eines [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="92536-107">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92536-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="92536-108">Prerequisites</span></span>
<span data-ttu-id="92536-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="92536-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="92536-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92536-111">Permission type</span></span>|<span data-ttu-id="92536-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92536-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92536-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92536-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92536-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92536-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="92536-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92536-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92536-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92536-116">Not supported.</span></span>|
|<span data-ttu-id="92536-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92536-117">Application</span></span>|<span data-ttu-id="92536-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92536-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92536-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92536-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="92536-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92536-120">Request headers</span></span>
|<span data-ttu-id="92536-121">Header</span><span class="sxs-lookup"><span data-stu-id="92536-121">Header</span></span>|<span data-ttu-id="92536-122">Wert</span><span class="sxs-lookup"><span data-stu-id="92536-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92536-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="92536-123">Authorization</span></span>|<span data-ttu-id="92536-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="92536-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92536-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="92536-125">Accept</span></span>|<span data-ttu-id="92536-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92536-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92536-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92536-127">Request body</span></span>
<span data-ttu-id="92536-128">Geben Sie im Textkörper Anforderung für das Objekt [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="92536-128">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="92536-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="92536-129">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="92536-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92536-130">Property</span></span>|<span data-ttu-id="92536-131">Typ</span><span class="sxs-lookup"><span data-stu-id="92536-131">Type</span></span>|<span data-ttu-id="92536-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92536-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92536-133">id</span><span class="sxs-lookup"><span data-stu-id="92536-133">id</span></span>|<span data-ttu-id="92536-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92536-134">String</span></span>|<span data-ttu-id="92536-135">Der eindeutige Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="92536-135">The unique Identifier.</span></span> <span data-ttu-id="92536-136">Dies ist die Id der UserId_DeviceId_AppId.</span><span class="sxs-lookup"><span data-stu-id="92536-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="92536-137">status</span><span class="sxs-lookup"><span data-stu-id="92536-137">status</span></span>|[<span data-ttu-id="92536-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="92536-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="92536-139">Melden Sie sich Upload-Status.</span><span class="sxs-lookup"><span data-stu-id="92536-139">Log upload status.</span></span> <span data-ttu-id="92536-140">Mögliche Werte sind: `pending`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="92536-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="92536-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="92536-141">errorMessage</span></span>|<span data-ttu-id="92536-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92536-142">String</span></span>|<span data-ttu-id="92536-143">Fehlermeldung gegebenenfalls beim Hochladen</span><span class="sxs-lookup"><span data-stu-id="92536-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="92536-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="92536-144">customLogFolders</span></span>|<span data-ttu-id="92536-145">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="92536-145">String collection</span></span>|<span data-ttu-id="92536-146">Liste der Protokollordner.</span><span class="sxs-lookup"><span data-stu-id="92536-146">List of log folders.</span></span> |
|<span data-ttu-id="92536-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="92536-147">completedDateTime</span></span>|<span data-ttu-id="92536-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92536-148">DateTimeOffset</span></span>|<span data-ttu-id="92536-149">Zeit an, die die Upload Protokoll Anforderung einen Endzustand erreicht</span><span class="sxs-lookup"><span data-stu-id="92536-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="92536-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="92536-150">Response</span></span>
<span data-ttu-id="92536-151">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="92536-151">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92536-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92536-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="92536-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92536-153">Request</span></span>
<span data-ttu-id="92536-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="92536-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92536-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="92536-155">Response</span></span>
<span data-ttu-id="92536-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92536-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




