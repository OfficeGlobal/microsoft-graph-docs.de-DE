---
title: WindowsDomainJoinConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsDomainJoinConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 89d6f6c2a53a1a00e6458fd155f2e6b45fe212ce
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572208"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="d821c-103">WindowsDomainJoinConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="d821c-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="d821c-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d821c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d821c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d821c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d821c-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d821c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d821c-107">Lesen von Eigenschaften und Beziehungen des [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d821c-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d821c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d821c-108">Prerequisites</span></span>

<span data-ttu-id="d821c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d821c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d821c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d821c-111">Permission type</span></span>|<span data-ttu-id="d821c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d821c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d821c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d821c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d821c-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="d821c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d821c-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d821c-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d821c-116">&nbsp;&nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="d821c-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d821c-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d821c-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="d821c-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d821c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d821c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d821c-119">Not supported.</span></span>|
|<span data-ttu-id="d821c-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d821c-120">Application</span></span>|<span data-ttu-id="d821c-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d821c-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d821c-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d821c-122">HTTP Request</span></span>
<span data-ttu-id="d821c-123">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="d821c-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="d821c-124">**Registrierungs**</span><span class="sxs-lookup"><span data-stu-id="d821c-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d821c-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d821c-125">Optional query parameters</span></span>

<span data-ttu-id="d821c-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d821c-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d821c-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d821c-127">Request headers</span></span>

|<span data-ttu-id="d821c-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d821c-128">Header</span></span>|<span data-ttu-id="d821c-129">Wert</span><span class="sxs-lookup"><span data-stu-id="d821c-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d821c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d821c-130">Authorization</span></span>|<span data-ttu-id="d821c-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d821c-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d821c-132">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d821c-132">Accept</span></span>|<span data-ttu-id="d821c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="d821c-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d821c-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d821c-134">Request body</span></span>

<span data-ttu-id="d821c-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d821c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d821c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d821c-136">Response</span></span>

<span data-ttu-id="d821c-137">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d821c-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d821c-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d821c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d821c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d821c-139">Request</span></span>

<span data-ttu-id="d821c-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d821c-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d821c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="d821c-141">Response</span></span>

<span data-ttu-id="d821c-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d821c-142">Here is an example of the response.</span></span> <span data-ttu-id="d821c-143">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="d821c-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d821c-144">Von einem tatsächlichen Aufruf zurückgegebene Eigenschaften hängen vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="d821c-144">Properties returned from an actual call depend on the context.</span></span>

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



