---
title: Abrufen von „windowsInformationProtectionAppLockerFile“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94ff91a6a59035d82d85d9712902581e05f7f69a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980908"
---
# <a name="get-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="21289-103">Abrufen von „windowsInformationProtectionAppLockerFile“</span><span class="sxs-lookup"><span data-stu-id="21289-103">Get windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="21289-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21289-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21289-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="21289-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21289-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="21289-106">Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21289-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21289-107">Prerequisites</span></span>
<span data-ttu-id="21289-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21289-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21289-110">Permission type</span></span>|<span data-ttu-id="21289-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21289-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21289-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21289-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21289-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21289-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="21289-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21289-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21289-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21289-115">Not supported.</span></span>|
|<span data-ttu-id="21289-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21289-116">Application</span></span>|<span data-ttu-id="21289-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21289-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21289-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21289-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21289-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="21289-119">Optional query parameters</span></span>
<span data-ttu-id="21289-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="21289-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21289-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21289-121">Request headers</span></span>
|<span data-ttu-id="21289-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="21289-122">Header</span></span>|<span data-ttu-id="21289-123">Wert</span><span class="sxs-lookup"><span data-stu-id="21289-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21289-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="21289-124">Authorization</span></span>|<span data-ttu-id="21289-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21289-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21289-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="21289-126">Accept</span></span>|<span data-ttu-id="21289-127">application/json</span><span class="sxs-lookup"><span data-stu-id="21289-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21289-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21289-128">Request body</span></span>
<span data-ttu-id="21289-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="21289-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21289-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="21289-130">Response</span></span>
<span data-ttu-id="21289-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="21289-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21289-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21289-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="21289-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21289-133">Request</span></span>
<span data-ttu-id="21289-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21289-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="21289-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="21289-135">Response</span></span>
<span data-ttu-id="21289-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21289-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
    "displayName": "Display Name value",
    "fileHash": "File Hash value",
    "file": "ZmlsZQ==",
    "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
    "version": "Version value"
  }
}
```




