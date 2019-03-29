---
title: Windows10EasEmailProfileConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des windows10EasEmailProfileConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef0e7d2871dd4e0b883fd3c07d4a037b1040e47b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979445"
---
# <a name="get-windows10easemailprofileconfiguration"></a><span data-ttu-id="afd68-103">Windows10EasEmailProfileConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="afd68-103">Get windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="afd68-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="afd68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afd68-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="afd68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afd68-106">Lesen von Eigenschaften und Beziehungen des [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="afd68-106">Read properties and relationships of the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afd68-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="afd68-107">Prerequisites</span></span>
<span data-ttu-id="afd68-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afd68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afd68-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="afd68-110">Permission type</span></span>|<span data-ttu-id="afd68-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="afd68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afd68-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="afd68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afd68-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="afd68-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="afd68-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="afd68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afd68-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afd68-115">Not supported.</span></span>|
|<span data-ttu-id="afd68-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="afd68-116">Application</span></span>|<span data-ttu-id="afd68-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afd68-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afd68-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="afd68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afd68-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="afd68-119">Optional query parameters</span></span>
<span data-ttu-id="afd68-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="afd68-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afd68-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="afd68-121">Request headers</span></span>
|<span data-ttu-id="afd68-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="afd68-122">Header</span></span>|<span data-ttu-id="afd68-123">Wert</span><span class="sxs-lookup"><span data-stu-id="afd68-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afd68-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="afd68-124">Authorization</span></span>|<span data-ttu-id="afd68-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="afd68-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afd68-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="afd68-126">Accept</span></span>|<span data-ttu-id="afd68-127">application/json</span><span class="sxs-lookup"><span data-stu-id="afd68-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afd68-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="afd68-128">Request body</span></span>
<span data-ttu-id="afd68-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="afd68-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afd68-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="afd68-130">Response</span></span>
<span data-ttu-id="afd68-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="afd68-131">If successful, this method returns a `200 OK` response code and [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afd68-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="afd68-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="afd68-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="afd68-133">Request</span></span>
<span data-ttu-id="afd68-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="afd68-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="afd68-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="afd68-135">Response</span></span>
<span data-ttu-id="afd68-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afd68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 992

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
    "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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
    "customDomainName": "Custom Domain Name value",
    "accountName": "Account Name value",
    "syncCalendar": true,
    "syncContacts": true,
    "syncTasks": true,
    "durationOfEmailToSync": "oneDay",
    "emailAddressSource": "primarySmtpAddress",
    "emailSyncSchedule": "asMessagesArrive",
    "hostName": "Host Name value",
    "requireSsl": true
  }
}
```




