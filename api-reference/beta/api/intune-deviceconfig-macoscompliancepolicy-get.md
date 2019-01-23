---
title: Abrufen von „macOSCompliancePolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf31a9fefbb1e98f331f2fe87ac69ffbefdf15cc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419709"
---
# <a name="get-macoscompliancepolicy"></a><span data-ttu-id="201f4-103">Abrufen von „macOSCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="201f4-103">Get macOSCompliancePolicy</span></span>

> <span data-ttu-id="201f4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="201f4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="201f4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="201f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="201f4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="201f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="201f4-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="201f4-107">Read properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="201f4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="201f4-108">Prerequisites</span></span>
<span data-ttu-id="201f4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="201f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="201f4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="201f4-111">Permission type</span></span>|<span data-ttu-id="201f4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="201f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="201f4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="201f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="201f4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="201f4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="201f4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="201f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="201f4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="201f4-116">Not supported.</span></span>|
|<span data-ttu-id="201f4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="201f4-117">Application</span></span>|<span data-ttu-id="201f4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="201f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="201f4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="201f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="201f4-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="201f4-120">Optional query parameters</span></span>
<span data-ttu-id="201f4-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="201f4-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="201f4-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="201f4-122">Request headers</span></span>
|<span data-ttu-id="201f4-123">Header</span><span class="sxs-lookup"><span data-stu-id="201f4-123">Header</span></span>|<span data-ttu-id="201f4-124">Wert</span><span class="sxs-lookup"><span data-stu-id="201f4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="201f4-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="201f4-125">Authorization</span></span>|<span data-ttu-id="201f4-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="201f4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="201f4-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="201f4-127">Accept</span></span>|<span data-ttu-id="201f4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="201f4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="201f4-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="201f4-129">Request body</span></span>
<span data-ttu-id="201f4-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="201f4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="201f4-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="201f4-131">Response</span></span>
<span data-ttu-id="201f4-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="201f4-132">If successful, this method returns a `200 OK` response code and [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="201f4-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="201f4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="201f4-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="201f4-134">Request</span></span>
<span data-ttu-id="201f4-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="201f4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="201f4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="201f4-136">Response</span></span>
<span data-ttu-id="201f4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="201f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




