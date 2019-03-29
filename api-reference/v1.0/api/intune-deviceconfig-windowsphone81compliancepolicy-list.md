---
title: Auflisten von „windowsPhone81CompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81CompliancePolicy auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b41b67c1ca9b7daf29e1bc3870ea6a4e71c36210
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961287"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="ecb7d-103">Auflisten von „windowsPhone81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="ecb7d-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="ecb7d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ecb7d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecb7d-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ecb7d-105">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecb7d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ecb7d-106">Prerequisites</span></span>
<span data-ttu-id="ecb7d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecb7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb7d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ecb7d-109">Permission type</span></span>|<span data-ttu-id="ecb7d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ecb7d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecb7d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ecb7d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ecb7d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecb7d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ecb7d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ecb7d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecb7d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ecb7d-114">Not supported.</span></span>|
|<span data-ttu-id="ecb7d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ecb7d-115">Application</span></span>|<span data-ttu-id="ecb7d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ecb7d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecb7d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecb7d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ecb7d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ecb7d-118">Request headers</span></span>
|<span data-ttu-id="ecb7d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ecb7d-119">Header</span></span>|<span data-ttu-id="ecb7d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ecb7d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecb7d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecb7d-121">Authorization</span></span>|<span data-ttu-id="ecb7d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ecb7d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecb7d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ecb7d-123">Accept</span></span>|<span data-ttu-id="ecb7d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ecb7d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecb7d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ecb7d-125">Request body</span></span>
<span data-ttu-id="ecb7d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ecb7d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecb7d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecb7d-127">Response</span></span>
<span data-ttu-id="ecb7d-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ecb7d-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecb7d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ecb7d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecb7d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecb7d-130">Request</span></span>
<span data-ttu-id="ecb7d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ecb7d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="ecb7d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecb7d-132">Response</span></span>
<span data-ttu-id="ecb7d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ecb7d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
      "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```



