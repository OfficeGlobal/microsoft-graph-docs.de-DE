---
title: Auflisten von „windowsPhone81CompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81CompliancePolicy auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: afff1ee89af34f04a83fa0fd0f950a8f480244b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401187"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="50e20-103">Auflisten von „windowsPhone81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="50e20-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="50e20-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="50e20-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50e20-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50e20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50e20-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50e20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50e20-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="50e20-107">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50e20-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50e20-108">Prerequisites</span></span>
<span data-ttu-id="50e20-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="50e20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="50e20-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50e20-111">Permission type</span></span>|<span data-ttu-id="50e20-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50e20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50e20-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50e20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50e20-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50e20-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50e20-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50e20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50e20-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50e20-116">Not supported.</span></span>|
|<span data-ttu-id="50e20-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50e20-117">Application</span></span>|<span data-ttu-id="50e20-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50e20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50e20-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50e20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="50e20-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50e20-120">Request headers</span></span>
|<span data-ttu-id="50e20-121">Header</span><span class="sxs-lookup"><span data-stu-id="50e20-121">Header</span></span>|<span data-ttu-id="50e20-122">Wert</span><span class="sxs-lookup"><span data-stu-id="50e20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50e20-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="50e20-123">Authorization</span></span>|<span data-ttu-id="50e20-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50e20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50e20-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="50e20-125">Accept</span></span>|<span data-ttu-id="50e20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50e20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50e20-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50e20-127">Request body</span></span>
<span data-ttu-id="50e20-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="50e20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50e20-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="50e20-129">Response</span></span>
<span data-ttu-id="50e20-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="50e20-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50e20-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50e20-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="50e20-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50e20-132">Request</span></span>
<span data-ttu-id="50e20-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50e20-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="50e20-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="50e20-134">Response</span></span>
<span data-ttu-id="50e20-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50e20-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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




