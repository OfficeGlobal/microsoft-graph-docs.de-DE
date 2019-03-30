---
title: Auflisten von „windowsInformationProtectionAppLockerFile“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsInformationProtectionAppLockerFile auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e85388b8ed9e219bc5f2dbd8231e14f3a23254b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985487"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="a285e-103">Auflisten von „windowsInformationProtectionAppLockerFile“</span><span class="sxs-lookup"><span data-stu-id="a285e-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="a285e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a285e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a285e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a285e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a285e-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) auf.</span><span class="sxs-lookup"><span data-stu-id="a285e-106">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a285e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a285e-107">Prerequisites</span></span>
<span data-ttu-id="a285e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a285e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a285e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a285e-110">Permission type</span></span>|<span data-ttu-id="a285e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a285e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a285e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a285e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a285e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a285e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a285e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a285e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a285e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a285e-115">Not supported.</span></span>|
|<span data-ttu-id="a285e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a285e-116">Application</span></span>|<span data-ttu-id="a285e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a285e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a285e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a285e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="a285e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a285e-119">Request headers</span></span>
|<span data-ttu-id="a285e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a285e-120">Header</span></span>|<span data-ttu-id="a285e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a285e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a285e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a285e-122">Authorization</span></span>|<span data-ttu-id="a285e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a285e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a285e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a285e-124">Accept</span></span>|<span data-ttu-id="a285e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a285e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a285e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a285e-126">Request body</span></span>
<span data-ttu-id="a285e-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a285e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a285e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a285e-128">Response</span></span>
<span data-ttu-id="a285e-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a285e-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a285e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a285e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a285e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a285e-131">Request</span></span>
<span data-ttu-id="a285e-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a285e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="a285e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a285e-133">Response</span></span>
<span data-ttu-id="a285e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a285e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
      "displayName": "Display Name value",
      "fileHash": "File Hash value",
      "file": "ZmlsZQ==",
      "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
      "version": "Version value"
    }
  ]
}
```




