---
title: windowsInformationProtectionAppLockerFile aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionAppLockerFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6e6d81b953288e1c8c9435a9502616f3f9fbc1d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923824"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="0c512-103">windowsInformationProtectionAppLockerFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0c512-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="0c512-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0c512-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c512-105">Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c512-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c512-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0c512-106">Prerequisites</span></span>
<span data-ttu-id="0c512-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c512-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c512-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c512-109">Permission type</span></span>|<span data-ttu-id="0c512-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c512-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c512-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c512-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c512-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c512-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c512-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c512-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c512-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c512-114">Not supported.</span></span>|
|<span data-ttu-id="0c512-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c512-115">Application</span></span>|<span data-ttu-id="0c512-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c512-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c512-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c512-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0c512-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c512-118">Request headers</span></span>
|<span data-ttu-id="0c512-119">Header</span><span class="sxs-lookup"><span data-stu-id="0c512-119">Header</span></span>|<span data-ttu-id="0c512-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0c512-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c512-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c512-121">Authorization</span></span>|<span data-ttu-id="0c512-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0c512-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c512-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0c512-123">Accept</span></span>|<span data-ttu-id="0c512-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0c512-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c512-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c512-125">Request body</span></span>
<span data-ttu-id="0c512-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="0c512-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="0c512-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0c512-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="0c512-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c512-128">Property</span></span>|<span data-ttu-id="0c512-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0c512-129">Type</span></span>|<span data-ttu-id="0c512-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c512-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c512-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0c512-131">displayName</span></span>|<span data-ttu-id="0c512-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c512-132">String</span></span>|<span data-ttu-id="0c512-133">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="0c512-133">The friendly name</span></span>|
|<span data-ttu-id="0c512-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="0c512-134">fileHash</span></span>|<span data-ttu-id="0c512-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c512-135">String</span></span>|<span data-ttu-id="0c512-136">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="0c512-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="0c512-137">file</span><span class="sxs-lookup"><span data-stu-id="0c512-137">file</span></span>|<span data-ttu-id="0c512-138">Binär</span><span class="sxs-lookup"><span data-stu-id="0c512-138">Binary</span></span>|<span data-ttu-id="0c512-139">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="0c512-139">File as a byte array</span></span>|
|<span data-ttu-id="0c512-140">id</span><span class="sxs-lookup"><span data-stu-id="0c512-140">id</span></span>|<span data-ttu-id="0c512-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c512-141">String</span></span>|<span data-ttu-id="0c512-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0c512-142">Key of the entity.</span></span>|
|<span data-ttu-id="0c512-143">Version</span><span class="sxs-lookup"><span data-stu-id="0c512-143">version</span></span>|<span data-ttu-id="0c512-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c512-144">String</span></span>|<span data-ttu-id="0c512-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="0c512-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0c512-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c512-146">Response</span></span>
<span data-ttu-id="0c512-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c512-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c512-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c512-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c512-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c512-149">Request</span></span>
<span data-ttu-id="0c512-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c512-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c512-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c512-151">Response</span></span>
<span data-ttu-id="0c512-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c512-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



