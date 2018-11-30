---
title: settingStateDeviceSummary löschen
description: Löscht ein settingStateDeviceSummary-Objekt.
ms.openlocfilehash: 3f00c115b6956335a412ddd11adfb61156294f6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061731"
---
# <a name="delete-settingstatedevicesummary"></a><span data-ttu-id="b8a82-103">settingStateDeviceSummary löschen</span><span class="sxs-lookup"><span data-stu-id="b8a82-103">Delete settingStateDeviceSummary</span></span>

> <span data-ttu-id="b8a82-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b8a82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8a82-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8a82-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8a82-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8a82-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8a82-107">Löscht ein [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b8a82-107">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8a82-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8a82-108">Prerequisites</span></span>
<span data-ttu-id="b8a82-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8a82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8a82-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8a82-111">Permission type</span></span>|<span data-ttu-id="b8a82-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8a82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8a82-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8a82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8a82-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8a82-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8a82-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8a82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8a82-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8a82-116">Not supported.</span></span>|
|<span data-ttu-id="b8a82-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8a82-117">Application</span></span>|<span data-ttu-id="b8a82-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8a82-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8a82-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8a82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b8a82-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8a82-120">Request headers</span></span>
|<span data-ttu-id="b8a82-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8a82-121">Header</span></span>|<span data-ttu-id="b8a82-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b8a82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8a82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8a82-123">Authorization</span></span>|<span data-ttu-id="b8a82-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8a82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8a82-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8a82-125">Accept</span></span>|<span data-ttu-id="b8a82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8a82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8a82-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8a82-127">Request body</span></span>
<span data-ttu-id="b8a82-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b8a82-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8a82-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8a82-129">Response</span></span>
<span data-ttu-id="b8a82-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8a82-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8a82-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8a82-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8a82-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8a82-132">Request</span></span>
<span data-ttu-id="b8a82-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8a82-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="b8a82-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8a82-134">Response</span></span>
<span data-ttu-id="b8a82-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8a82-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





