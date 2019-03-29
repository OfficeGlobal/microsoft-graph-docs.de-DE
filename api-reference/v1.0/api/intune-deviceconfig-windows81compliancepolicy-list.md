---
title: Auflisten von „windows81CompliancePolicy“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs windows81CompliancePolicy auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40ed80b53f7e94942a7c2aa9eca09b66f6d9a576
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959250"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="4cef9-103">Auflisten von „windows81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="4cef9-103">List windows81CompliancePolicies</span></span>

> <span data-ttu-id="4cef9-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4cef9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cef9-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="4cef9-105">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cef9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4cef9-106">Prerequisites</span></span>
<span data-ttu-id="4cef9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cef9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4cef9-109">Permission type</span></span>|<span data-ttu-id="4cef9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4cef9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cef9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4cef9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4cef9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cef9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4cef9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4cef9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cef9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cef9-114">Not supported.</span></span>|
|<span data-ttu-id="4cef9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4cef9-115">Application</span></span>|<span data-ttu-id="4cef9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cef9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cef9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cef9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4cef9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4cef9-118">Request headers</span></span>
|<span data-ttu-id="4cef9-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4cef9-119">Header</span></span>|<span data-ttu-id="4cef9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4cef9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cef9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cef9-121">Authorization</span></span>|<span data-ttu-id="4cef9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4cef9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cef9-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4cef9-123">Accept</span></span>|<span data-ttu-id="4cef9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4cef9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cef9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4cef9-125">Request body</span></span>
<span data-ttu-id="4cef9-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4cef9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cef9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cef9-127">Response</span></span>
<span data-ttu-id="4cef9-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4cef9-128">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cef9-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4cef9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cef9-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cef9-130">Request</span></span>
<span data-ttu-id="4cef9-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4cef9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="4cef9-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cef9-132">Response</span></span>
<span data-ttu-id="4cef9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cef9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 879

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
      "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```



