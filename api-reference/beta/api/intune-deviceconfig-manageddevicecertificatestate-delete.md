---
title: ManagedDeviceCertificateState löschen
description: Löscht eine managedDeviceCertificateState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf22947ba12497f772282442d42bdd855d837f2b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150918"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="7ce00-103">ManagedDeviceCertificateState löschen</span><span class="sxs-lookup"><span data-stu-id="7ce00-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="7ce00-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ce00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ce00-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7ce00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ce00-106">Löscht eine [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="7ce00-106">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ce00-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7ce00-107">Prerequisites</span></span>
<span data-ttu-id="7ce00-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7ce00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7ce00-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ce00-110">Permission type</span></span>|<span data-ttu-id="7ce00-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ce00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ce00-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ce00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ce00-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ce00-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ce00-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ce00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ce00-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ce00-115">Not supported.</span></span>|
|<span data-ttu-id="7ce00-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ce00-116">Application</span></span>|<span data-ttu-id="7ce00-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ce00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ce00-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ce00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7ce00-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ce00-119">Request headers</span></span>
|<span data-ttu-id="7ce00-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7ce00-120">Header</span></span>|<span data-ttu-id="7ce00-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7ce00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ce00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ce00-122">Authorization</span></span>|<span data-ttu-id="7ce00-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7ce00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ce00-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7ce00-124">Accept</span></span>|<span data-ttu-id="7ce00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ce00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ce00-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ce00-126">Request body</span></span>
<span data-ttu-id="7ce00-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7ce00-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ce00-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ce00-128">Response</span></span>
<span data-ttu-id="7ce00-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ce00-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7ce00-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ce00-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ce00-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ce00-131">Request</span></span>
<span data-ttu-id="7ce00-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ce00-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="7ce00-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ce00-133">Response</span></span>
<span data-ttu-id="7ce00-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ce00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




