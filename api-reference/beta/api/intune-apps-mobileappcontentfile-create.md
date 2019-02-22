---
title: Erstellen von „mobileAppContentFile“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43e56cbf1fd3419cae2d0b88ac64225985e07b5f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167004"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="86910-103">Erstellen von „mobileAppContentFile“</span><span class="sxs-lookup"><span data-stu-id="86910-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="86910-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="86910-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86910-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="86910-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86910-106">Diese Methode erstellt ein neues Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="86910-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86910-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="86910-107">Prerequisites</span></span>
<span data-ttu-id="86910-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="86910-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86910-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86910-110">Permission type</span></span>|<span data-ttu-id="86910-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86910-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86910-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86910-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86910-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86910-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="86910-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86910-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86910-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86910-115">Not supported.</span></span>|
|<span data-ttu-id="86910-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86910-116">Application</span></span>|<span data-ttu-id="86910-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86910-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86910-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86910-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="86910-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86910-119">Request headers</span></span>
|<span data-ttu-id="86910-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="86910-120">Header</span></span>|<span data-ttu-id="86910-121">Wert</span><span class="sxs-lookup"><span data-stu-id="86910-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86910-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86910-122">Authorization</span></span>|<span data-ttu-id="86910-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="86910-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86910-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="86910-124">Accept</span></span>|<span data-ttu-id="86910-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86910-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86910-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86910-126">Request body</span></span>
<span data-ttu-id="86910-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppContentFile“ an.</span><span class="sxs-lookup"><span data-stu-id="86910-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="86910-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppContentFile“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="86910-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="86910-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86910-129">Property</span></span>|<span data-ttu-id="86910-130">Typ</span><span class="sxs-lookup"><span data-stu-id="86910-130">Type</span></span>|<span data-ttu-id="86910-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86910-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86910-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="86910-132">azureStorageUri</span></span>|<span data-ttu-id="86910-133">String</span><span class="sxs-lookup"><span data-stu-id="86910-133">String</span></span>|<span data-ttu-id="86910-134">Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="86910-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="86910-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="86910-135">isCommitted</span></span>|<span data-ttu-id="86910-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="86910-136">Boolean</span></span>|<span data-ttu-id="86910-137">Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde</span><span class="sxs-lookup"><span data-stu-id="86910-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="86910-138">id</span><span class="sxs-lookup"><span data-stu-id="86910-138">id</span></span>|<span data-ttu-id="86910-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86910-139">String</span></span>|<span data-ttu-id="86910-140">ID der Datei</span><span class="sxs-lookup"><span data-stu-id="86910-140">The File Id.</span></span>|
|<span data-ttu-id="86910-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86910-141">createdDateTime</span></span>|<span data-ttu-id="86910-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86910-142">DateTimeOffset</span></span>|<span data-ttu-id="86910-143">Datum und Uhrzeit der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="86910-143">The time the file was created.</span></span>|
|<span data-ttu-id="86910-144">name</span><span class="sxs-lookup"><span data-stu-id="86910-144">name</span></span>|<span data-ttu-id="86910-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86910-145">String</span></span>|<span data-ttu-id="86910-146">Name der Datei</span><span class="sxs-lookup"><span data-stu-id="86910-146">the file name.</span></span>|
|<span data-ttu-id="86910-147">size</span><span class="sxs-lookup"><span data-stu-id="86910-147">size</span></span>|<span data-ttu-id="86910-148">Int64</span><span class="sxs-lookup"><span data-stu-id="86910-148">Int64</span></span>|<span data-ttu-id="86910-149">Größe der Datei vor der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="86910-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="86910-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="86910-150">sizeEncrypted</span></span>|<span data-ttu-id="86910-151">Int64</span><span class="sxs-lookup"><span data-stu-id="86910-151">Int64</span></span>|<span data-ttu-id="86910-152">Größe der Datei nach der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="86910-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="86910-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="86910-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="86910-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86910-154">DateTimeOffset</span></span>|<span data-ttu-id="86910-155">Datum und Uhrzeit des Ablaufs des Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="86910-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="86910-156">manifest</span><span class="sxs-lookup"><span data-stu-id="86910-156">manifest</span></span>|<span data-ttu-id="86910-157">Binär</span><span class="sxs-lookup"><span data-stu-id="86910-157">Binary</span></span>|<span data-ttu-id="86910-158">Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="86910-158">The manifest information.</span></span>|
|<span data-ttu-id="86910-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="86910-159">uploadState</span></span>|[<span data-ttu-id="86910-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="86910-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="86910-161">Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="86910-161">The state of the current upload request.</span></span> <span data-ttu-id="86910-162">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="86910-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="86910-163">isFrameworkdatei</span><span class="sxs-lookup"><span data-stu-id="86910-163">isFrameworkFile</span></span>|<span data-ttu-id="86910-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86910-164">Boolean</span></span>|<span data-ttu-id="86910-165">Ein Wert, der angibt, ob es sich bei der Datei um eine frameworkdatei handelt.</span><span class="sxs-lookup"><span data-stu-id="86910-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="86910-166">isDependency</span><span class="sxs-lookup"><span data-stu-id="86910-166">isDependency</span></span>|<span data-ttu-id="86910-167">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86910-167">Boolean</span></span>|<span data-ttu-id="86910-168">Gibt an, ob die Inhaltsdatei eine Abhängigkeit für die Hauptinhaltsdatei ist.</span><span class="sxs-lookup"><span data-stu-id="86910-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="86910-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="86910-169">Response</span></span>
<span data-ttu-id="86910-170">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="86910-170">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86910-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86910-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="86910-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86910-172">Request</span></span>
<span data-ttu-id="86910-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86910-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-type: application/json
Content-length: 395

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```

### <a name="response"></a><span data-ttu-id="86910-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="86910-174">Response</span></span>
<span data-ttu-id="86910-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86910-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 503

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```




