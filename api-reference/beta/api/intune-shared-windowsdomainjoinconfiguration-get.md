---
title: Abrufen von windowsDomainJoinConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des WindowsDomainJoinConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64a295ae105a69865e304c45d08e339eadbf7936
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950242"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="a5e3b-103">Abrufen von windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="a5e3b-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="a5e3b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5e3b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5e3b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5e3b-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5e3b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a5e3b-108">Prerequisites</span></span>

<span data-ttu-id="a5e3b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5e3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5e3b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5e3b-111">Permission type</span></span>|<span data-ttu-id="a5e3b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5e3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5e3b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5e3b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a5e3b-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="a5e3b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a5e3b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5e3b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="a5e3b-116">&nbsp; &nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="a5e3b-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="a5e3b-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5e3b-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="a5e3b-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5e3b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5e3b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5e3b-119">Not supported.</span></span>|
|<span data-ttu-id="a5e3b-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5e3b-120">Application</span></span>|<span data-ttu-id="a5e3b-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5e3b-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5e3b-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5e3b-122">HTTP Request</span></span>
<span data-ttu-id="a5e3b-123">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a5e3b-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="a5e3b-124">**Registrierung**</span><span class="sxs-lookup"><span data-stu-id="a5e3b-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5e3b-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a5e3b-125">Optional query parameters</span></span>

<span data-ttu-id="a5e3b-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5e3b-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5e3b-127">Request headers</span></span>

|<span data-ttu-id="a5e3b-128">Header</span><span class="sxs-lookup"><span data-stu-id="a5e3b-128">Header</span></span>|<span data-ttu-id="a5e3b-129">Wert</span><span class="sxs-lookup"><span data-stu-id="a5e3b-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5e3b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5e3b-130">Authorization</span></span>|<span data-ttu-id="a5e3b-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a5e3b-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5e3b-132">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a5e3b-132">Accept</span></span>|<span data-ttu-id="a5e3b-133">application/json</span><span class="sxs-lookup"><span data-stu-id="a5e3b-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5e3b-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5e3b-134">Request body</span></span>

<span data-ttu-id="a5e3b-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5e3b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5e3b-136">Response</span></span>

<span data-ttu-id="a5e3b-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5e3b-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5e3b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5e3b-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5e3b-139">Request</span></span>

<span data-ttu-id="a5e3b-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a5e3b-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5e3b-141">Response</span></span>

<span data-ttu-id="a5e3b-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-142">Here is an example of the response.</span></span> <span data-ttu-id="a5e3b-143">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a5e3b-144">Eigenschaften von einer tatsächlichen Aufruf zurückgegeben richten sich nach den Kontext.</span><span class="sxs-lookup"><span data-stu-id="a5e3b-144">Properties returned from an actual call depend on the context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
    "id": "40118d08-8d08-4011-088d-1140088d1140",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "computerNameStaticPrefix": "Computer Name Static Prefix value",
    "computerNameSuffixRandomCharCount": 1,
    "activeDirectoryDomainName": "Active Directory Domain Name value"
  }
}
```



