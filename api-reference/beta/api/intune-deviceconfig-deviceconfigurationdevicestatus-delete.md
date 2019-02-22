---
title: deviceConfigurationDeviceStatus löschen
description: Löscht ein deviceConfigurationDeviceStatus-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9590d9e6aab09fa1b74291bdc1856f20ba30d0c2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155279"
---
# <a name="delete-deviceconfigurationdevicestatus"></a><span data-ttu-id="ed546-103">deviceConfigurationDeviceStatus löschen</span><span class="sxs-lookup"><span data-stu-id="ed546-103">Delete deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="ed546-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed546-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed546-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ed546-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed546-106">Löscht ein [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ed546-106">Deletes a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed546-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ed546-107">Prerequisites</span></span>
<span data-ttu-id="ed546-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed546-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ed546-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed546-110">Permission type</span></span>|<span data-ttu-id="ed546-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed546-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed546-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed546-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed546-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed546-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed546-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed546-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed546-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed546-115">Not supported.</span></span>|
|<span data-ttu-id="ed546-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed546-116">Application</span></span>|<span data-ttu-id="ed546-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed546-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed546-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed546-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ed546-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed546-119">Request headers</span></span>
|<span data-ttu-id="ed546-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ed546-120">Header</span></span>|<span data-ttu-id="ed546-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ed546-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed546-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed546-122">Authorization</span></span>|<span data-ttu-id="ed546-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ed546-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed546-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ed546-124">Accept</span></span>|<span data-ttu-id="ed546-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed546-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed546-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed546-126">Request body</span></span>
<span data-ttu-id="ed546-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ed546-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed546-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed546-128">Response</span></span>
<span data-ttu-id="ed546-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed546-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ed546-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed546-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed546-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed546-131">Request</span></span>
<span data-ttu-id="ed546-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed546-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="ed546-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed546-133">Response</span></span>
<span data-ttu-id="ed546-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed546-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




