---
title: mobileAppContentFile aktualisieren
description: Aktualisieren der Eigenschaften eines MobileAppContentFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e2cafce913352a0b5298149689e4a404daa020c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171400"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="77dd3-103">mobileAppContentFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="77dd3-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="77dd3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77dd3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77dd3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="77dd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77dd3-106">Aktualisieren der Eigenschaften eines [MobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="77dd3-106">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77dd3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77dd3-107">Prerequisites</span></span>
<span data-ttu-id="77dd3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="77dd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77dd3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77dd3-110">Permission type</span></span>|<span data-ttu-id="77dd3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77dd3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77dd3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77dd3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77dd3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77dd3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77dd3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77dd3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77dd3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77dd3-115">Not supported.</span></span>|
|<span data-ttu-id="77dd3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77dd3-116">Application</span></span>|<span data-ttu-id="77dd3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77dd3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77dd3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77dd3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="77dd3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77dd3-119">Request headers</span></span>
|<span data-ttu-id="77dd3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77dd3-120">Header</span></span>|<span data-ttu-id="77dd3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="77dd3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77dd3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77dd3-122">Authorization</span></span>|<span data-ttu-id="77dd3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77dd3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77dd3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="77dd3-124">Accept</span></span>|<span data-ttu-id="77dd3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77dd3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77dd3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77dd3-126">Request body</span></span>
<span data-ttu-id="77dd3-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) an.</span><span class="sxs-lookup"><span data-stu-id="77dd3-127">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="77dd3-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="77dd3-128">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="77dd3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77dd3-129">Property</span></span>|<span data-ttu-id="77dd3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="77dd3-130">Type</span></span>|<span data-ttu-id="77dd3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77dd3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77dd3-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="77dd3-132">azureStorageUri</span></span>|<span data-ttu-id="77dd3-133">String</span><span class="sxs-lookup"><span data-stu-id="77dd3-133">String</span></span>|<span data-ttu-id="77dd3-134">Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="77dd3-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="77dd3-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="77dd3-135">isCommitted</span></span>|<span data-ttu-id="77dd3-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="77dd3-136">Boolean</span></span>|<span data-ttu-id="77dd3-137">Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde</span><span class="sxs-lookup"><span data-stu-id="77dd3-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="77dd3-138">id</span><span class="sxs-lookup"><span data-stu-id="77dd3-138">id</span></span>|<span data-ttu-id="77dd3-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77dd3-139">String</span></span>|<span data-ttu-id="77dd3-140">ID der Datei</span><span class="sxs-lookup"><span data-stu-id="77dd3-140">The File Id.</span></span>|
|<span data-ttu-id="77dd3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77dd3-141">createdDateTime</span></span>|<span data-ttu-id="77dd3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77dd3-142">DateTimeOffset</span></span>|<span data-ttu-id="77dd3-143">Datum und Uhrzeit der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="77dd3-143">The time the file was created.</span></span>|
|<span data-ttu-id="77dd3-144">name</span><span class="sxs-lookup"><span data-stu-id="77dd3-144">name</span></span>|<span data-ttu-id="77dd3-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77dd3-145">String</span></span>|<span data-ttu-id="77dd3-146">Name der Datei</span><span class="sxs-lookup"><span data-stu-id="77dd3-146">the file name.</span></span>|
|<span data-ttu-id="77dd3-147">size</span><span class="sxs-lookup"><span data-stu-id="77dd3-147">size</span></span>|<span data-ttu-id="77dd3-148">Int64</span><span class="sxs-lookup"><span data-stu-id="77dd3-148">Int64</span></span>|<span data-ttu-id="77dd3-149">Größe der Datei vor der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="77dd3-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="77dd3-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="77dd3-150">sizeEncrypted</span></span>|<span data-ttu-id="77dd3-151">Int64</span><span class="sxs-lookup"><span data-stu-id="77dd3-151">Int64</span></span>|<span data-ttu-id="77dd3-152">Größe der Datei nach der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="77dd3-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="77dd3-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="77dd3-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="77dd3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77dd3-154">DateTimeOffset</span></span>|<span data-ttu-id="77dd3-155">Datum und Uhrzeit des Ablaufs des Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="77dd3-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="77dd3-156">manifest</span><span class="sxs-lookup"><span data-stu-id="77dd3-156">manifest</span></span>|<span data-ttu-id="77dd3-157">Binär</span><span class="sxs-lookup"><span data-stu-id="77dd3-157">Binary</span></span>|<span data-ttu-id="77dd3-158">Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="77dd3-158">The manifest information.</span></span>|
|<span data-ttu-id="77dd3-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="77dd3-159">uploadState</span></span>|[<span data-ttu-id="77dd3-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="77dd3-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="77dd3-161">Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="77dd3-161">The state of the current upload request.</span></span> <span data-ttu-id="77dd3-162">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="77dd3-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="77dd3-163">isFrameworkdatei</span><span class="sxs-lookup"><span data-stu-id="77dd3-163">isFrameworkFile</span></span>|<span data-ttu-id="77dd3-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="77dd3-164">Boolean</span></span>|<span data-ttu-id="77dd3-165">Ein Wert, der angibt, ob es sich bei der Datei um eine frameworkdatei handelt.</span><span class="sxs-lookup"><span data-stu-id="77dd3-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="77dd3-166">isDependency</span><span class="sxs-lookup"><span data-stu-id="77dd3-166">isDependency</span></span>|<span data-ttu-id="77dd3-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="77dd3-167">Boolean</span></span>|<span data-ttu-id="77dd3-168">Gibt an, ob die Inhaltsdatei eine Abhängigkeit für die Hauptinhaltsdatei ist.</span><span class="sxs-lookup"><span data-stu-id="77dd3-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="77dd3-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="77dd3-169">Response</span></span>
<span data-ttu-id="77dd3-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77dd3-170">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77dd3-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77dd3-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="77dd3-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77dd3-172">Request</span></span>
<span data-ttu-id="77dd3-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77dd3-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
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

### <a name="response"></a><span data-ttu-id="77dd3-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="77dd3-174">Response</span></span>
<span data-ttu-id="77dd3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77dd3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




