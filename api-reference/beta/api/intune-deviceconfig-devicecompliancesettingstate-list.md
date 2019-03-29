---
title: Auflisten von „deviceComplianceSettingState“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceSettingState auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 160e35b4e1559c7be264071961285c207bc70269
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961896"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="27be3-103">Auflisten von „deviceComplianceSettingState“</span><span class="sxs-lookup"><span data-stu-id="27be3-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="27be3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="27be3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27be3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="27be3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27be3-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) auf.</span><span class="sxs-lookup"><span data-stu-id="27be3-106">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27be3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="27be3-107">Prerequisites</span></span>
<span data-ttu-id="27be3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27be3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27be3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="27be3-110">Permission type</span></span>|<span data-ttu-id="27be3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="27be3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27be3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="27be3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27be3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="27be3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="27be3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="27be3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27be3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27be3-115">Not supported.</span></span>|
|<span data-ttu-id="27be3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="27be3-116">Application</span></span>|<span data-ttu-id="27be3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27be3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27be3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="27be3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="27be3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="27be3-119">Request headers</span></span>
|<span data-ttu-id="27be3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="27be3-120">Header</span></span>|<span data-ttu-id="27be3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="27be3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27be3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27be3-122">Authorization</span></span>|<span data-ttu-id="27be3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="27be3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27be3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="27be3-124">Accept</span></span>|<span data-ttu-id="27be3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27be3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27be3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="27be3-126">Request body</span></span>
<span data-ttu-id="27be3-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="27be3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27be3-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="27be3-128">Response</span></span>
<span data-ttu-id="27be3-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="27be3-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27be3-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="27be3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="27be3-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="27be3-131">Request</span></span>
<span data-ttu-id="27be3-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="27be3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="27be3-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="27be3-133">Response</span></span>
<span data-ttu-id="27be3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="27be3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "platformType": "windowsRT",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```




