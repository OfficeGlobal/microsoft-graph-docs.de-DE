---
title: windowsInformationProtectionAppLockerFile erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLockerFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 13b6d9a0e8fc6e23b2a5b7b85e257ef8d3ac9c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853319"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="64109-103">windowsInformationProtectionAppLockerFile erstellen</span><span class="sxs-lookup"><span data-stu-id="64109-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="64109-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="64109-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64109-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64109-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64109-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="64109-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64109-107">Erstellen eines neuen [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="64109-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64109-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="64109-108">Prerequisites</span></span>
<span data-ttu-id="64109-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64109-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64109-111">Permission type</span></span>|<span data-ttu-id="64109-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64109-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64109-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64109-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64109-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64109-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64109-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64109-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64109-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64109-116">Not supported.</span></span>|
|<span data-ttu-id="64109-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64109-117">Application</span></span>|<span data-ttu-id="64109-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64109-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64109-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64109-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="64109-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64109-120">Request headers</span></span>
|<span data-ttu-id="64109-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="64109-121">Header</span></span>|<span data-ttu-id="64109-122">Wert</span><span class="sxs-lookup"><span data-stu-id="64109-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64109-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64109-123">Authorization</span></span>|<span data-ttu-id="64109-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="64109-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64109-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="64109-125">Accept</span></span>|<span data-ttu-id="64109-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64109-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64109-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64109-127">Request body</span></span>
<span data-ttu-id="64109-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das WindowsInformationProtectionAppLockerFile-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="64109-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="64109-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLockerFile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="64109-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="64109-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="64109-130">Property</span></span>|<span data-ttu-id="64109-131">Typ</span><span class="sxs-lookup"><span data-stu-id="64109-131">Type</span></span>|<span data-ttu-id="64109-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64109-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64109-133">displayName</span><span class="sxs-lookup"><span data-stu-id="64109-133">displayName</span></span>|<span data-ttu-id="64109-134">String</span><span class="sxs-lookup"><span data-stu-id="64109-134">String</span></span>|<span data-ttu-id="64109-135">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="64109-135">The friendly name</span></span>|
|<span data-ttu-id="64109-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="64109-136">fileHash</span></span>|<span data-ttu-id="64109-137">String</span><span class="sxs-lookup"><span data-stu-id="64109-137">String</span></span>|<span data-ttu-id="64109-138">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="64109-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="64109-139">file</span><span class="sxs-lookup"><span data-stu-id="64109-139">file</span></span>|<span data-ttu-id="64109-140">Binär</span><span class="sxs-lookup"><span data-stu-id="64109-140">Binary</span></span>|<span data-ttu-id="64109-141">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="64109-141">File as a byte array</span></span>|
|<span data-ttu-id="64109-142">id</span><span class="sxs-lookup"><span data-stu-id="64109-142">id</span></span>|<span data-ttu-id="64109-143">String</span><span class="sxs-lookup"><span data-stu-id="64109-143">String</span></span>|<span data-ttu-id="64109-144">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="64109-144">Key of the entity.</span></span>|
|<span data-ttu-id="64109-145">Version</span><span class="sxs-lookup"><span data-stu-id="64109-145">version</span></span>|<span data-ttu-id="64109-146">String</span><span class="sxs-lookup"><span data-stu-id="64109-146">String</span></span>|<span data-ttu-id="64109-147">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="64109-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="64109-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="64109-148">Response</span></span>
<span data-ttu-id="64109-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64109-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64109-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64109-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="64109-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64109-151">Request</span></span>
<span data-ttu-id="64109-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64109-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64109-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="64109-153">Response</span></span>
<span data-ttu-id="64109-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64109-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





