---
title: ManagedDeviceCertificateState löschen
description: Löscht eine ManagedDeviceCertificateState.
ms.openlocfilehash: eb9d886c9d5479c20ea4c65bb1447036cf3c35f7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065164"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="d5f66-103">ManagedDeviceCertificateState löschen</span><span class="sxs-lookup"><span data-stu-id="d5f66-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="d5f66-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d5f66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5f66-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5f66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5f66-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d5f66-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5f66-107">Löscht eine [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="d5f66-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5f66-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d5f66-108">Prerequisites</span></span>
<span data-ttu-id="d5f66-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5f66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5f66-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5f66-111">Permission type</span></span>|<span data-ttu-id="d5f66-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5f66-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5f66-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5f66-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5f66-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5f66-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5f66-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5f66-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5f66-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5f66-116">Not supported.</span></span>|
|<span data-ttu-id="d5f66-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5f66-117">Application</span></span>|<span data-ttu-id="d5f66-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5f66-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5f66-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5f66-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d5f66-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d5f66-120">Request headers</span></span>
|<span data-ttu-id="d5f66-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d5f66-121">Header</span></span>|<span data-ttu-id="d5f66-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d5f66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5f66-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5f66-123">Authorization</span></span>|<span data-ttu-id="d5f66-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d5f66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5f66-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5f66-125">Accept</span></span>|<span data-ttu-id="d5f66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5f66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5f66-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d5f66-127">Request body</span></span>
<span data-ttu-id="d5f66-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d5f66-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5f66-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5f66-129">Response</span></span>
<span data-ttu-id="d5f66-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5f66-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d5f66-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d5f66-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5f66-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5f66-132">Request</span></span>
<span data-ttu-id="d5f66-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5f66-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="d5f66-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5f66-134">Response</span></span>
<span data-ttu-id="d5f66-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5f66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




