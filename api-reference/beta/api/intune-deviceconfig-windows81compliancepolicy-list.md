---
title: Auflisten von „windows81CompliancePolicy“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs windows81CompliancePolicy auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3362e09cecf1fef715bdd09066d78a12e4416a39
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962659"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="b107b-103">Auflisten von „windows81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="b107b-103">List windows81CompliancePolicies</span></span>

> <span data-ttu-id="b107b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b107b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b107b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b107b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b107b-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b107b-106">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b107b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b107b-107">Prerequisites</span></span>
<span data-ttu-id="b107b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b107b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b107b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b107b-110">Permission type</span></span>|<span data-ttu-id="b107b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b107b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b107b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b107b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b107b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b107b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b107b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b107b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b107b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b107b-115">Not supported.</span></span>|
|<span data-ttu-id="b107b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b107b-116">Application</span></span>|<span data-ttu-id="b107b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b107b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b107b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b107b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b107b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b107b-119">Request headers</span></span>
|<span data-ttu-id="b107b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b107b-120">Header</span></span>|<span data-ttu-id="b107b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b107b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b107b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b107b-122">Authorization</span></span>|<span data-ttu-id="b107b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b107b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b107b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b107b-124">Accept</span></span>|<span data-ttu-id="b107b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b107b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b107b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b107b-126">Request body</span></span>
<span data-ttu-id="b107b-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b107b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b107b-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b107b-128">Response</span></span>
<span data-ttu-id="b107b-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b107b-129">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b107b-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b107b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b107b-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b107b-131">Request</span></span>
<span data-ttu-id="b107b-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b107b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="b107b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b107b-133">Response</span></span>
<span data-ttu-id="b107b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b107b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 953

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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




