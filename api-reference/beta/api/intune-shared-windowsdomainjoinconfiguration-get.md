---
title: Abrufen von windowsDomainJoinConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des WindowsDomainJoinConfiguration-Objekts.
ms.openlocfilehash: b3b76a902b4a740d142e1027f04d1f98f5fb32aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060695"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="d51dc-103">Abrufen von windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="d51dc-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="d51dc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d51dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d51dc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d51dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d51dc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d51dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d51dc-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d51dc-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d51dc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d51dc-108">Prerequisites</span></span>

<span data-ttu-id="d51dc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d51dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d51dc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d51dc-111">Permission type</span></span>|<span data-ttu-id="d51dc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d51dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d51dc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d51dc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d51dc-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="d51dc-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d51dc-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d51dc-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d51dc-116">&nbsp; &nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="d51dc-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d51dc-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d51dc-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="d51dc-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d51dc-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d51dc-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d51dc-119">Not supported.</span></span>|
|<span data-ttu-id="d51dc-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d51dc-120">Application</span></span>|<span data-ttu-id="d51dc-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d51dc-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d51dc-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d51dc-122">HTTP Request</span></span>
<span data-ttu-id="d51dc-123">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="d51dc-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="d51dc-124">**Registrierung**</span><span class="sxs-lookup"><span data-stu-id="d51dc-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d51dc-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d51dc-125">Optional query parameters</span></span>

<span data-ttu-id="d51dc-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d51dc-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d51dc-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d51dc-127">Request headers</span></span>

|<span data-ttu-id="d51dc-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d51dc-128">Header</span></span>|<span data-ttu-id="d51dc-129">Wert</span><span class="sxs-lookup"><span data-stu-id="d51dc-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d51dc-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d51dc-130">Authorization</span></span>|<span data-ttu-id="d51dc-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d51dc-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d51dc-132">Accept</span><span class="sxs-lookup"><span data-stu-id="d51dc-132">Accept</span></span>|<span data-ttu-id="d51dc-133">application/json</span><span class="sxs-lookup"><span data-stu-id="d51dc-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d51dc-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d51dc-134">Request body</span></span>

<span data-ttu-id="d51dc-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d51dc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d51dc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d51dc-136">Response</span></span>

<span data-ttu-id="d51dc-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d51dc-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d51dc-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d51dc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d51dc-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d51dc-139">Request</span></span>

<span data-ttu-id="d51dc-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d51dc-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d51dc-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="d51dc-141">Response</span></span>

<span data-ttu-id="d51dc-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d51dc-142">Here is an example of the response.</span></span> <span data-ttu-id="d51dc-143">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="d51dc-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d51dc-144">Eigenschaften von einer tatsächlichen Aufruf zurückgegeben richten sich nach den Kontext.</span><span class="sxs-lookup"><span data-stu-id="d51dc-144">Properties returned from an actual call depend on the context.</span></span>

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



