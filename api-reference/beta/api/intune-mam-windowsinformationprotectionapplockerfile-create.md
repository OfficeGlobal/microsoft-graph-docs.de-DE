---
title: windowsInformationProtectionAppLockerFile erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLockerFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9399f23590bee975506a2972f6ba3bc0fa8c3c07
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975784"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="6a301-103">windowsInformationProtectionAppLockerFile erstellen</span><span class="sxs-lookup"><span data-stu-id="6a301-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="6a301-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a301-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a301-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6a301-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a301-106">Erstellen eines neuen [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a301-106">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a301-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6a301-107">Prerequisites</span></span>
<span data-ttu-id="6a301-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a301-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a301-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a301-110">Permission type</span></span>|<span data-ttu-id="6a301-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a301-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a301-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a301-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a301-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a301-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a301-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a301-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a301-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a301-115">Not supported.</span></span>|
|<span data-ttu-id="6a301-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a301-116">Application</span></span>|<span data-ttu-id="6a301-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a301-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a301-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a301-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="6a301-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a301-119">Request headers</span></span>
|<span data-ttu-id="6a301-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6a301-120">Header</span></span>|<span data-ttu-id="6a301-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6a301-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a301-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a301-122">Authorization</span></span>|<span data-ttu-id="6a301-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6a301-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a301-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6a301-124">Accept</span></span>|<span data-ttu-id="6a301-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a301-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a301-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a301-126">Request body</span></span>
<span data-ttu-id="6a301-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das WindowsInformationProtectionAppLockerFile-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="6a301-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="6a301-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLockerFile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6a301-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="6a301-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a301-129">Property</span></span>|<span data-ttu-id="6a301-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6a301-130">Type</span></span>|<span data-ttu-id="6a301-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a301-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a301-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6a301-132">displayName</span></span>|<span data-ttu-id="6a301-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a301-133">String</span></span>|<span data-ttu-id="6a301-134">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="6a301-134">The friendly name</span></span>|
|<span data-ttu-id="6a301-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="6a301-135">fileHash</span></span>|<span data-ttu-id="6a301-136">String</span><span class="sxs-lookup"><span data-stu-id="6a301-136">String</span></span>|<span data-ttu-id="6a301-137">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="6a301-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="6a301-138">file</span><span class="sxs-lookup"><span data-stu-id="6a301-138">file</span></span>|<span data-ttu-id="6a301-139">Binär</span><span class="sxs-lookup"><span data-stu-id="6a301-139">Binary</span></span>|<span data-ttu-id="6a301-140">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="6a301-140">File as a byte array</span></span>|
|<span data-ttu-id="6a301-141">id</span><span class="sxs-lookup"><span data-stu-id="6a301-141">id</span></span>|<span data-ttu-id="6a301-142">String</span><span class="sxs-lookup"><span data-stu-id="6a301-142">String</span></span>|<span data-ttu-id="6a301-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6a301-143">Key of the entity.</span></span>|
|<span data-ttu-id="6a301-144">Version</span><span class="sxs-lookup"><span data-stu-id="6a301-144">version</span></span>|<span data-ttu-id="6a301-145">String</span><span class="sxs-lookup"><span data-stu-id="6a301-145">String</span></span>|<span data-ttu-id="6a301-146">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="6a301-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6a301-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a301-147">Response</span></span>
<span data-ttu-id="6a301-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a301-148">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a301-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a301-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a301-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a301-150">Request</span></span>
<span data-ttu-id="6a301-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a301-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="6a301-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a301-152">Response</span></span>
<span data-ttu-id="6a301-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a301-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```




