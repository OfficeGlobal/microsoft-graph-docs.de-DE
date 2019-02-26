---
title: windowsInformationProtectionAppLockerFile erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLockerFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f3b411e680a3df86b86517f63c8055cec8e4f17
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261838"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="a407e-103">windowsInformationProtectionAppLockerFile erstellen</span><span class="sxs-lookup"><span data-stu-id="a407e-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="a407e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a407e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a407e-105">Erstellen eines neuen [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a407e-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a407e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a407e-106">Prerequisites</span></span>
<span data-ttu-id="a407e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a407e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a407e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a407e-109">Permission type</span></span>|<span data-ttu-id="a407e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a407e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a407e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a407e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a407e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a407e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a407e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a407e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a407e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a407e-114">Not supported.</span></span>|
|<span data-ttu-id="a407e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a407e-115">Application</span></span>|<span data-ttu-id="a407e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a407e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a407e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a407e-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a407e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a407e-118">Request headers</span></span>
|<span data-ttu-id="a407e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a407e-119">Header</span></span>|<span data-ttu-id="a407e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a407e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a407e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a407e-121">Authorization</span></span>|<span data-ttu-id="a407e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a407e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a407e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a407e-123">Accept</span></span>|<span data-ttu-id="a407e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a407e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a407e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a407e-125">Request body</span></span>
<span data-ttu-id="a407e-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das WindowsInformationProtectionAppLockerFile-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="a407e-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="a407e-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLockerFile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a407e-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="a407e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a407e-128">Property</span></span>|<span data-ttu-id="a407e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a407e-129">Type</span></span>|<span data-ttu-id="a407e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a407e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a407e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a407e-131">displayName</span></span>|<span data-ttu-id="a407e-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a407e-132">String</span></span>|<span data-ttu-id="a407e-133">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="a407e-133">The friendly name</span></span>|
|<span data-ttu-id="a407e-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="a407e-134">fileHash</span></span>|<span data-ttu-id="a407e-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a407e-135">String</span></span>|<span data-ttu-id="a407e-136">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="a407e-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="a407e-137">file</span><span class="sxs-lookup"><span data-stu-id="a407e-137">file</span></span>|<span data-ttu-id="a407e-138">Binär</span><span class="sxs-lookup"><span data-stu-id="a407e-138">Binary</span></span>|<span data-ttu-id="a407e-139">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="a407e-139">File as a byte array</span></span>|
|<span data-ttu-id="a407e-140">id</span><span class="sxs-lookup"><span data-stu-id="a407e-140">id</span></span>|<span data-ttu-id="a407e-141">string</span><span class="sxs-lookup"><span data-stu-id="a407e-141">String</span></span>|<span data-ttu-id="a407e-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a407e-142">Key of the entity.</span></span>|
|<span data-ttu-id="a407e-143">Version</span><span class="sxs-lookup"><span data-stu-id="a407e-143">version</span></span>|<span data-ttu-id="a407e-144">String</span><span class="sxs-lookup"><span data-stu-id="a407e-144">String</span></span>|<span data-ttu-id="a407e-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="a407e-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="a407e-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="a407e-146">Response</span></span>
<span data-ttu-id="a407e-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a407e-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a407e-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a407e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="a407e-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a407e-149">Request</span></span>
<span data-ttu-id="a407e-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a407e-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
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

### <a name="response"></a><span data-ttu-id="a407e-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="a407e-151">Response</span></span>
<span data-ttu-id="a407e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a407e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



