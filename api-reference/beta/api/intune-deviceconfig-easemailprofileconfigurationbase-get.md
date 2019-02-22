---
title: EasEmailProfileConfigurationBase abrufen
description: Lesen von Eigenschaften und Beziehungen des easEmailProfileConfigurationBase-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bd62426d66a8aeb5d5a5869856c83d365833ee4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148524"
---
# <a name="get-easemailprofileconfigurationbase"></a><span data-ttu-id="9ce1b-103">EasEmailProfileConfigurationBase abrufen</span><span class="sxs-lookup"><span data-stu-id="9ce1b-103">Get easEmailProfileConfigurationBase</span></span>

> <span data-ttu-id="9ce1b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ce1b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ce1b-106">Lesen von Eigenschaften und Beziehungen des [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-106">Read properties and relationships of the [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ce1b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9ce1b-107">Prerequisites</span></span>
<span data-ttu-id="9ce1b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ce1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9ce1b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ce1b-110">Permission type</span></span>|<span data-ttu-id="9ce1b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ce1b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ce1b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ce1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ce1b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ce1b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9ce1b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ce1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ce1b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ce1b-115">Not supported.</span></span>|
|<span data-ttu-id="9ce1b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ce1b-116">Application</span></span>|<span data-ttu-id="9ce1b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ce1b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ce1b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ce1b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ce1b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9ce1b-119">Optional query parameters</span></span>
<span data-ttu-id="9ce1b-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ce1b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ce1b-121">Request headers</span></span>
|<span data-ttu-id="9ce1b-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9ce1b-122">Header</span></span>|<span data-ttu-id="9ce1b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9ce1b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ce1b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ce1b-124">Authorization</span></span>|<span data-ttu-id="9ce1b-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ce1b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ce1b-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9ce1b-126">Accept</span></span>|<span data-ttu-id="9ce1b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ce1b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ce1b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ce1b-128">Request body</span></span>
<span data-ttu-id="9ce1b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ce1b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ce1b-130">Response</span></span>
<span data-ttu-id="9ce1b-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-131">If successful, this method returns a `200 OK` response code and [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ce1b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ce1b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ce1b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ce1b-133">Request</span></span>
<span data-ttu-id="9ce1b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9ce1b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ce1b-135">Response</span></span>
<span data-ttu-id="9ce1b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ce1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "value": {
    "@odata.type": "#microsoft.graph.easEmailProfileConfigurationBase",
    "id": "a3f96310-6310-a3f9-1063-f9a31063f9a3",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "usernameSource": "primarySmtpAddress",
    "usernameAADSource": "primarySmtpAddress",
    "userDomainNameSource": "netBiosDomainName",
    "customDomainName": "Custom Domain Name value"
  }
}
```




