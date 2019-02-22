---
title: Abrufen von „macOSCompliancePolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d93c5b8a13a2d879169994d55ac9821673231247
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159619"
---
# <a name="get-macoscompliancepolicy"></a><span data-ttu-id="542c8-103">Abrufen von „macOSCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="542c8-103">Get macOSCompliancePolicy</span></span>

> <span data-ttu-id="542c8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="542c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="542c8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="542c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="542c8-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="542c8-106">Read properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="542c8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="542c8-107">Prerequisites</span></span>
<span data-ttu-id="542c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="542c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="542c8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="542c8-110">Permission type</span></span>|<span data-ttu-id="542c8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="542c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="542c8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="542c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="542c8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="542c8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="542c8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="542c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="542c8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="542c8-115">Not supported.</span></span>|
|<span data-ttu-id="542c8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="542c8-116">Application</span></span>|<span data-ttu-id="542c8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="542c8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="542c8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="542c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="542c8-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="542c8-119">Optional query parameters</span></span>
<span data-ttu-id="542c8-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="542c8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="542c8-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="542c8-121">Request headers</span></span>
|<span data-ttu-id="542c8-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="542c8-122">Header</span></span>|<span data-ttu-id="542c8-123">Wert</span><span class="sxs-lookup"><span data-stu-id="542c8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="542c8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="542c8-124">Authorization</span></span>|<span data-ttu-id="542c8-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="542c8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="542c8-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="542c8-126">Accept</span></span>|<span data-ttu-id="542c8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="542c8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="542c8-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="542c8-128">Request body</span></span>
<span data-ttu-id="542c8-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="542c8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="542c8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="542c8-130">Response</span></span>
<span data-ttu-id="542c8-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="542c8-131">If successful, this method returns a `200 OK` response code and [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="542c8-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="542c8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="542c8-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="542c8-133">Request</span></span>
<span data-ttu-id="542c8-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="542c8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="542c8-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="542c8-135">Response</span></span>
<span data-ttu-id="542c8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="542c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1334

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
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
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "osMinimumBuildVersion": "Os Minimum Build Version value",
    "osMaximumBuildVersion": "Os Maximum Build Version value",
    "systemIntegrityProtectionEnabled": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "storageRequireEncryption": true,
    "gatekeeperAllowedAppSource": "macAppStore",
    "firewallEnabled": true,
    "firewallBlockAllIncoming": true,
    "firewallEnableStealthMode": true
  }
}
```




