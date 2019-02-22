---
title: windowsInformationProtectionAppLockerFile aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionAppLockerFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe11c8cba9d2cb1eaba6a4225fa48d2b71adf23b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144037"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="062c5-103">windowsInformationProtectionAppLockerFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="062c5-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="062c5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="062c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="062c5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="062c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="062c5-106">Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="062c5-106">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="062c5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="062c5-107">Prerequisites</span></span>
<span data-ttu-id="062c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="062c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="062c5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="062c5-110">Permission type</span></span>|<span data-ttu-id="062c5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="062c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="062c5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="062c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="062c5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="062c5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="062c5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="062c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="062c5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="062c5-115">Not supported.</span></span>|
|<span data-ttu-id="062c5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="062c5-116">Application</span></span>|<span data-ttu-id="062c5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="062c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="062c5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="062c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="062c5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="062c5-119">Request headers</span></span>
|<span data-ttu-id="062c5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="062c5-120">Header</span></span>|<span data-ttu-id="062c5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="062c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="062c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="062c5-122">Authorization</span></span>|<span data-ttu-id="062c5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="062c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="062c5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="062c5-124">Accept</span></span>|<span data-ttu-id="062c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="062c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="062c5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="062c5-126">Request body</span></span>
<span data-ttu-id="062c5-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="062c5-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="062c5-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="062c5-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="062c5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="062c5-129">Property</span></span>|<span data-ttu-id="062c5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="062c5-130">Type</span></span>|<span data-ttu-id="062c5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="062c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="062c5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="062c5-132">displayName</span></span>|<span data-ttu-id="062c5-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="062c5-133">String</span></span>|<span data-ttu-id="062c5-134">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="062c5-134">The friendly name</span></span>|
|<span data-ttu-id="062c5-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="062c5-135">fileHash</span></span>|<span data-ttu-id="062c5-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="062c5-136">String</span></span>|<span data-ttu-id="062c5-137">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="062c5-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="062c5-138">file</span><span class="sxs-lookup"><span data-stu-id="062c5-138">file</span></span>|<span data-ttu-id="062c5-139">Binär</span><span class="sxs-lookup"><span data-stu-id="062c5-139">Binary</span></span>|<span data-ttu-id="062c5-140">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="062c5-140">File as a byte array</span></span>|
|<span data-ttu-id="062c5-141">id</span><span class="sxs-lookup"><span data-stu-id="062c5-141">id</span></span>|<span data-ttu-id="062c5-142">string</span><span class="sxs-lookup"><span data-stu-id="062c5-142">String</span></span>|<span data-ttu-id="062c5-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="062c5-143">Key of the entity.</span></span>|
|<span data-ttu-id="062c5-144">Version</span><span class="sxs-lookup"><span data-stu-id="062c5-144">version</span></span>|<span data-ttu-id="062c5-145">String</span><span class="sxs-lookup"><span data-stu-id="062c5-145">String</span></span>|<span data-ttu-id="062c5-146">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="062c5-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="062c5-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="062c5-147">Response</span></span>
<span data-ttu-id="062c5-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="062c5-148">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="062c5-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="062c5-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="062c5-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="062c5-150">Request</span></span>
<span data-ttu-id="062c5-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="062c5-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
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

### <a name="response"></a><span data-ttu-id="062c5-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="062c5-152">Response</span></span>
<span data-ttu-id="062c5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="062c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




