---
title: windowsInformationProtectionAppLockerFile erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLockerFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7e5076b30d577c74551ccd5718ce6d41c3f345e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834356"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="1045e-103">windowsInformationProtectionAppLockerFile erstellen</span><span class="sxs-lookup"><span data-stu-id="1045e-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="1045e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1045e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1045e-105">Erstellen eines neuen [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1045e-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1045e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1045e-106">Prerequisites</span></span>
<span data-ttu-id="1045e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1045e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1045e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1045e-109">Permission type</span></span>|<span data-ttu-id="1045e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1045e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1045e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1045e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1045e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1045e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1045e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1045e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1045e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1045e-114">Not supported.</span></span>|
|<span data-ttu-id="1045e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1045e-115">Application</span></span>|<span data-ttu-id="1045e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1045e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1045e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1045e-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1045e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1045e-118">Request headers</span></span>
|<span data-ttu-id="1045e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1045e-119">Header</span></span>|<span data-ttu-id="1045e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1045e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1045e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1045e-121">Authorization</span></span>|<span data-ttu-id="1045e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1045e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1045e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1045e-123">Accept</span></span>|<span data-ttu-id="1045e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1045e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1045e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1045e-125">Request body</span></span>
<span data-ttu-id="1045e-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das WindowsInformationProtectionAppLockerFile-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="1045e-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="1045e-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLockerFile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1045e-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="1045e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1045e-128">Property</span></span>|<span data-ttu-id="1045e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1045e-129">Type</span></span>|<span data-ttu-id="1045e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1045e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1045e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="1045e-131">displayName</span></span>|<span data-ttu-id="1045e-132">String</span><span class="sxs-lookup"><span data-stu-id="1045e-132">String</span></span>|<span data-ttu-id="1045e-133">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="1045e-133">The friendly name</span></span>|
|<span data-ttu-id="1045e-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="1045e-134">fileHash</span></span>|<span data-ttu-id="1045e-135">String</span><span class="sxs-lookup"><span data-stu-id="1045e-135">String</span></span>|<span data-ttu-id="1045e-136">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="1045e-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="1045e-137">file</span><span class="sxs-lookup"><span data-stu-id="1045e-137">file</span></span>|<span data-ttu-id="1045e-138">Binär</span><span class="sxs-lookup"><span data-stu-id="1045e-138">Binary</span></span>|<span data-ttu-id="1045e-139">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="1045e-139">File as a byte array</span></span>|
|<span data-ttu-id="1045e-140">id</span><span class="sxs-lookup"><span data-stu-id="1045e-140">id</span></span>|<span data-ttu-id="1045e-141">String</span><span class="sxs-lookup"><span data-stu-id="1045e-141">String</span></span>|<span data-ttu-id="1045e-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1045e-142">Key of the entity.</span></span>|
|<span data-ttu-id="1045e-143">Version</span><span class="sxs-lookup"><span data-stu-id="1045e-143">version</span></span>|<span data-ttu-id="1045e-144">String</span><span class="sxs-lookup"><span data-stu-id="1045e-144">String</span></span>|<span data-ttu-id="1045e-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="1045e-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1045e-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1045e-146">Response</span></span>
<span data-ttu-id="1045e-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1045e-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1045e-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1045e-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="1045e-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1045e-149">Request</span></span>
<span data-ttu-id="1045e-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1045e-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1045e-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="1045e-151">Response</span></span>
<span data-ttu-id="1045e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1045e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



