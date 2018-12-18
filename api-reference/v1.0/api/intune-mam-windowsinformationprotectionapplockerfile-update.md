---
title: windowsInformationProtectionAppLockerFile aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionAppLockerFile-Objekts.
author: tfitzmac
ms.openlocfilehash: fdf14722d82da5afa2d51cb87b8e8c6ea69b9bf5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309835"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="c7292-103">windowsInformationProtectionAppLockerFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c7292-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="c7292-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c7292-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7292-105">Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7292-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7292-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c7292-106">Prerequisites</span></span>
<span data-ttu-id="c7292-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7292-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7292-109">Permission type</span></span>|<span data-ttu-id="c7292-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7292-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7292-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7292-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7292-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7292-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7292-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7292-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7292-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7292-114">Not supported.</span></span>|
|<span data-ttu-id="c7292-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7292-115">Application</span></span>|<span data-ttu-id="c7292-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7292-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7292-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7292-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c7292-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7292-118">Request headers</span></span>
|<span data-ttu-id="c7292-119">Header</span><span class="sxs-lookup"><span data-stu-id="c7292-119">Header</span></span>|<span data-ttu-id="c7292-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c7292-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7292-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c7292-121">Authorization</span></span>|<span data-ttu-id="c7292-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c7292-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7292-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c7292-123">Accept</span></span>|<span data-ttu-id="c7292-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c7292-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7292-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7292-125">Request body</span></span>
<span data-ttu-id="c7292-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="c7292-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="c7292-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c7292-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="c7292-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7292-128">Property</span></span>|<span data-ttu-id="c7292-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c7292-129">Type</span></span>|<span data-ttu-id="c7292-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7292-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7292-131">displayName</span><span class="sxs-lookup"><span data-stu-id="c7292-131">displayName</span></span>|<span data-ttu-id="c7292-132">String</span><span class="sxs-lookup"><span data-stu-id="c7292-132">String</span></span>|<span data-ttu-id="c7292-133">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="c7292-133">The friendly name</span></span>|
|<span data-ttu-id="c7292-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="c7292-134">fileHash</span></span>|<span data-ttu-id="c7292-135">String</span><span class="sxs-lookup"><span data-stu-id="c7292-135">String</span></span>|<span data-ttu-id="c7292-136">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="c7292-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="c7292-137">file</span><span class="sxs-lookup"><span data-stu-id="c7292-137">file</span></span>|<span data-ttu-id="c7292-138">Binär</span><span class="sxs-lookup"><span data-stu-id="c7292-138">Binary</span></span>|<span data-ttu-id="c7292-139">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="c7292-139">File as a byte array</span></span>|
|<span data-ttu-id="c7292-140">id</span><span class="sxs-lookup"><span data-stu-id="c7292-140">id</span></span>|<span data-ttu-id="c7292-141">String</span><span class="sxs-lookup"><span data-stu-id="c7292-141">String</span></span>|<span data-ttu-id="c7292-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c7292-142">Key of the entity.</span></span>|
|<span data-ttu-id="c7292-143">Version</span><span class="sxs-lookup"><span data-stu-id="c7292-143">version</span></span>|<span data-ttu-id="c7292-144">String</span><span class="sxs-lookup"><span data-stu-id="c7292-144">String</span></span>|<span data-ttu-id="c7292-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="c7292-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c7292-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7292-146">Response</span></span>
<span data-ttu-id="c7292-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7292-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7292-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7292-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7292-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7292-149">Request</span></span>
<span data-ttu-id="c7292-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7292-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
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

### <a name="response"></a><span data-ttu-id="c7292-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7292-151">Response</span></span>
<span data-ttu-id="c7292-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7292-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



