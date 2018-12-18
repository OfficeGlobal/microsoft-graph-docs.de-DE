---
title: Abrufen von windows10EasEmailProfileConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des windows10EasEmailProfileConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 9990b00d68c0fd61fce0461a09574939dd52fe13
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352136"
---
# <a name="get-windows10easemailprofileconfiguration"></a><span data-ttu-id="b2b3e-103">Abrufen von windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="b2b3e-103">Get windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="b2b3e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b2b3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2b3e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2b3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2b3e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b2b3e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2b3e-107">Lesen Sie Eigenschaften und Beziehungen des [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2b3e-107">Read properties and relationships of the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2b3e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b2b3e-108">Prerequisites</span></span>
<span data-ttu-id="b2b3e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2b3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2b3e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b2b3e-111">Permission type</span></span>|<span data-ttu-id="b2b3e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b2b3e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2b3e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b2b3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2b3e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2b3e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b2b3e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b2b3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2b3e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2b3e-116">Not supported.</span></span>|
|<span data-ttu-id="b2b3e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b2b3e-117">Application</span></span>|<span data-ttu-id="b2b3e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2b3e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2b3e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2b3e-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b2b3e-120">Optional query parameters</span></span>
<span data-ttu-id="b2b3e-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b2b3e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b2b3e-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b2b3e-122">Request headers</span></span>
|<span data-ttu-id="b2b3e-123">Header</span><span class="sxs-lookup"><span data-stu-id="b2b3e-123">Header</span></span>|<span data-ttu-id="b2b3e-124">Wert</span><span class="sxs-lookup"><span data-stu-id="b2b3e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2b3e-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b2b3e-125">Authorization</span></span>|<span data-ttu-id="b2b3e-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b2b3e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2b3e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b2b3e-127">Accept</span></span>|<span data-ttu-id="b2b3e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b2b3e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2b3e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b2b3e-129">Request body</span></span>
<span data-ttu-id="b2b3e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b2b3e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2b3e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b3e-131">Response</span></span>
<span data-ttu-id="b2b3e-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b2b3e-132">If successful, this method returns a `200 OK` response code and [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2b3e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b2b3e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2b3e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b3e-134">Request</span></span>
<span data-ttu-id="b2b3e-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b2b3e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b2b3e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b3e-136">Response</span></span>
<span data-ttu-id="b2b3e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2b3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





