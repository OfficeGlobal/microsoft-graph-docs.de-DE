---
title: ManagedDeviceCertificateState löschen
description: Löscht eine ManagedDeviceCertificateState.
author: tfitzmac
ms.openlocfilehash: e97757843bc8c4ef7444bd81cee6ffb0666ab94f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341615"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="3b1ba-103">ManagedDeviceCertificateState löschen</span><span class="sxs-lookup"><span data-stu-id="3b1ba-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="3b1ba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b1ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b1ba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b1ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b1ba-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3b1ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b1ba-107">Löscht eine [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="3b1ba-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b1ba-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3b1ba-108">Prerequisites</span></span>
<span data-ttu-id="3b1ba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b1ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b1ba-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b1ba-111">Permission type</span></span>|<span data-ttu-id="3b1ba-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b1ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b1ba-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b1ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b1ba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b1ba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b1ba-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b1ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b1ba-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b1ba-116">Not supported.</span></span>|
|<span data-ttu-id="3b1ba-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b1ba-117">Application</span></span>|<span data-ttu-id="3b1ba-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b1ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b1ba-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b1ba-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3b1ba-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b1ba-120">Request headers</span></span>
|<span data-ttu-id="3b1ba-121">Header</span><span class="sxs-lookup"><span data-stu-id="3b1ba-121">Header</span></span>|<span data-ttu-id="3b1ba-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3b1ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b1ba-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3b1ba-123">Authorization</span></span>|<span data-ttu-id="3b1ba-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3b1ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b1ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b1ba-125">Accept</span></span>|<span data-ttu-id="3b1ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b1ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b1ba-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b1ba-127">Request body</span></span>
<span data-ttu-id="3b1ba-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3b1ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b1ba-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b1ba-129">Response</span></span>
<span data-ttu-id="3b1ba-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b1ba-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3b1ba-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b1ba-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b1ba-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b1ba-132">Request</span></span>
<span data-ttu-id="3b1ba-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b1ba-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="3b1ba-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b1ba-134">Response</span></span>
<span data-ttu-id="3b1ba-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b1ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





