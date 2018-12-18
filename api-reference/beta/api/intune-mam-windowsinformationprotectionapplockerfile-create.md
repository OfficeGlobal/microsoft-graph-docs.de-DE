---
title: windowsInformationProtectionAppLockerFile erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLockerFile-Objekts.
author: tfitzmac
ms.openlocfilehash: f2cbed922d6f2ac130169e5d9c85e3a5231184a5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317122"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="0b3aa-103">windowsInformationProtectionAppLockerFile erstellen</span><span class="sxs-lookup"><span data-stu-id="0b3aa-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="0b3aa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0b3aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b3aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0b3aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b3aa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0b3aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b3aa-107">Erstellen eines neuen [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0b3aa-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b3aa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0b3aa-108">Prerequisites</span></span>
<span data-ttu-id="0b3aa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b3aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b3aa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b3aa-111">Permission type</span></span>|<span data-ttu-id="0b3aa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b3aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b3aa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b3aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b3aa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b3aa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b3aa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b3aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b3aa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b3aa-116">Not supported.</span></span>|
|<span data-ttu-id="0b3aa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b3aa-117">Application</span></span>|<span data-ttu-id="0b3aa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b3aa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b3aa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b3aa-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0b3aa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b3aa-120">Request headers</span></span>
|<span data-ttu-id="0b3aa-121">Header</span><span class="sxs-lookup"><span data-stu-id="0b3aa-121">Header</span></span>|<span data-ttu-id="0b3aa-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0b3aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b3aa-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0b3aa-123">Authorization</span></span>|<span data-ttu-id="0b3aa-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0b3aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b3aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b3aa-125">Accept</span></span>|<span data-ttu-id="0b3aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b3aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b3aa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b3aa-127">Request body</span></span>
<span data-ttu-id="0b3aa-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das WindowsInformationProtectionAppLockerFile-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="0b3aa-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="0b3aa-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLockerFile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0b3aa-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="0b3aa-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b3aa-130">Property</span></span>|<span data-ttu-id="0b3aa-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0b3aa-131">Type</span></span>|<span data-ttu-id="0b3aa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b3aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b3aa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0b3aa-133">displayName</span></span>|<span data-ttu-id="0b3aa-134">String</span><span class="sxs-lookup"><span data-stu-id="0b3aa-134">String</span></span>|<span data-ttu-id="0b3aa-135">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="0b3aa-135">The friendly name</span></span>|
|<span data-ttu-id="0b3aa-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="0b3aa-136">fileHash</span></span>|<span data-ttu-id="0b3aa-137">String</span><span class="sxs-lookup"><span data-stu-id="0b3aa-137">String</span></span>|<span data-ttu-id="0b3aa-138">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="0b3aa-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="0b3aa-139">file</span><span class="sxs-lookup"><span data-stu-id="0b3aa-139">file</span></span>|<span data-ttu-id="0b3aa-140">Binär</span><span class="sxs-lookup"><span data-stu-id="0b3aa-140">Binary</span></span>|<span data-ttu-id="0b3aa-141">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="0b3aa-141">File as a byte array</span></span>|
|<span data-ttu-id="0b3aa-142">id</span><span class="sxs-lookup"><span data-stu-id="0b3aa-142">id</span></span>|<span data-ttu-id="0b3aa-143">String</span><span class="sxs-lookup"><span data-stu-id="0b3aa-143">String</span></span>|<span data-ttu-id="0b3aa-144">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0b3aa-144">Key of the entity.</span></span>|
|<span data-ttu-id="0b3aa-145">Version</span><span class="sxs-lookup"><span data-stu-id="0b3aa-145">version</span></span>|<span data-ttu-id="0b3aa-146">String</span><span class="sxs-lookup"><span data-stu-id="0b3aa-146">String</span></span>|<span data-ttu-id="0b3aa-147">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="0b3aa-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0b3aa-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b3aa-148">Response</span></span>
<span data-ttu-id="0b3aa-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b3aa-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b3aa-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b3aa-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b3aa-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b3aa-151">Request</span></span>
<span data-ttu-id="0b3aa-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b3aa-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b3aa-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b3aa-153">Response</span></span>
<span data-ttu-id="0b3aa-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b3aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





