---
title: Auflisten von „windows10MobileCompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows10MobileCompliancePolicy auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 324f915a5129521f5dcaf33c60e619313bcfdda3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418309"
---
# <a name="list-windows10mobilecompliancepolicies"></a><span data-ttu-id="192ac-103">Auflisten von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="192ac-103">List windows10MobileCompliancePolicies</span></span>

> <span data-ttu-id="192ac-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="192ac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="192ac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="192ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="192ac-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="192ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="192ac-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="192ac-107">List properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="192ac-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="192ac-108">Prerequisites</span></span>
<span data-ttu-id="192ac-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="192ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="192ac-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="192ac-111">Permission type</span></span>|<span data-ttu-id="192ac-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="192ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="192ac-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="192ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="192ac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="192ac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="192ac-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="192ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="192ac-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="192ac-116">Not supported.</span></span>|
|<span data-ttu-id="192ac-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="192ac-117">Application</span></span>|<span data-ttu-id="192ac-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="192ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="192ac-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="192ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="192ac-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="192ac-120">Request headers</span></span>
|<span data-ttu-id="192ac-121">Header</span><span class="sxs-lookup"><span data-stu-id="192ac-121">Header</span></span>|<span data-ttu-id="192ac-122">Wert</span><span class="sxs-lookup"><span data-stu-id="192ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="192ac-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="192ac-123">Authorization</span></span>|<span data-ttu-id="192ac-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="192ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="192ac-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="192ac-125">Accept</span></span>|<span data-ttu-id="192ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="192ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="192ac-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="192ac-127">Request body</span></span>
<span data-ttu-id="192ac-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="192ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="192ac-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="192ac-129">Response</span></span>
<span data-ttu-id="192ac-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="192ac-130">If successful, this method returns a `200 OK` response code and a collection of [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="192ac-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="192ac-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="192ac-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="192ac-132">Request</span></span>
<span data-ttu-id="192ac-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="192ac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="192ac-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="192ac-134">Response</span></span>
<span data-ttu-id="192ac-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="192ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1503

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "3d4237b0-37b0-3d42-b037-423db037423d",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordExpirationDays": 6,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordRequireToUnlockFromIdle": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true,
      "activeFirewallRequired": true,
      "validOperatingSystemBuildRanges": [
        {
          "@odata.type": "microsoft.graph.operatingSystemVersionRange",
          "description": "Description value",
          "lowestVersion": "Lowest Version value",
          "highestVersion": "Highest Version value"
        }
      ]
    }
  ]
}
```




