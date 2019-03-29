---
title: Auflisten von „windowsPhone81CompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81CompliancePolicy auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e6bd59b81739aa740fcc6bbb178db1773afdb52
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965445"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="df853-103">Auflisten von „windowsPhone81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="df853-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="df853-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df853-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df853-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="df853-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df853-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="df853-106">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df853-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="df853-107">Prerequisites</span></span>
<span data-ttu-id="df853-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df853-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df853-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df853-110">Permission type</span></span>|<span data-ttu-id="df853-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df853-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df853-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df853-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df853-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="df853-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="df853-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df853-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df853-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df853-115">Not supported.</span></span>|
|<span data-ttu-id="df853-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df853-116">Application</span></span>|<span data-ttu-id="df853-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df853-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df853-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df853-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="df853-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df853-119">Request headers</span></span>
|<span data-ttu-id="df853-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="df853-120">Header</span></span>|<span data-ttu-id="df853-121">Wert</span><span class="sxs-lookup"><span data-stu-id="df853-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df853-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df853-122">Authorization</span></span>|<span data-ttu-id="df853-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="df853-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df853-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="df853-124">Accept</span></span>|<span data-ttu-id="df853-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df853-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df853-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df853-126">Request body</span></span>
<span data-ttu-id="df853-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="df853-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df853-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="df853-128">Response</span></span>
<span data-ttu-id="df853-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="df853-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df853-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df853-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="df853-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df853-131">Request</span></span>
<span data-ttu-id="df853-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df853-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="df853-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="df853-133">Response</span></span>
<span data-ttu-id="df853-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df853-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




