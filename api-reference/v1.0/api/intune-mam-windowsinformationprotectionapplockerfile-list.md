---
title: Auflisten von „windowsInformationProtectionAppLockerFile“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsInformationProtectionAppLockerFile auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 220aef93b6e3b77b5c6665d61ec47512c5f30431
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973817"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="b2653-103">Auflisten von „windowsInformationProtectionAppLockerFile“</span><span class="sxs-lookup"><span data-stu-id="b2653-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="b2653-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b2653-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2653-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b2653-105">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2653-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b2653-106">Prerequisites</span></span>
<span data-ttu-id="b2653-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2653-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b2653-109">Permission type</span></span>|<span data-ttu-id="b2653-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b2653-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2653-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b2653-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2653-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2653-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b2653-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b2653-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2653-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2653-114">Not supported.</span></span>|
|<span data-ttu-id="b2653-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b2653-115">Application</span></span>|<span data-ttu-id="b2653-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2653-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2653-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2653-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b2653-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b2653-118">Request headers</span></span>
|<span data-ttu-id="b2653-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b2653-119">Header</span></span>|<span data-ttu-id="b2653-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b2653-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2653-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2653-121">Authorization</span></span>|<span data-ttu-id="b2653-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b2653-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2653-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b2653-123">Accept</span></span>|<span data-ttu-id="b2653-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b2653-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2653-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b2653-125">Request body</span></span>
<span data-ttu-id="b2653-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b2653-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2653-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2653-127">Response</span></span>
<span data-ttu-id="b2653-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b2653-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2653-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b2653-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2653-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2653-130">Request</span></span>
<span data-ttu-id="b2653-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b2653-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="b2653-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2653-132">Response</span></span>
<span data-ttu-id="b2653-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2653-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



