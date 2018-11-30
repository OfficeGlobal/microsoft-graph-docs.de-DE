---
title: Liste androidEasEmailProfileConfigurations
description: Listeneigenschaften und Beziehungen der AndroidEasEmailProfileConfiguration-Objekte.
ms.openlocfilehash: f3c81df1f83a4f5094de3f252242a0fbd6340981
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065588"
---
# <a name="list-androideasemailprofileconfigurations"></a><span data-ttu-id="f6629-103">Liste androidEasEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="f6629-103">List androidEasEmailProfileConfigurations</span></span>

> <span data-ttu-id="f6629-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6629-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6629-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6629-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6629-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f6629-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6629-107">Listeneigenschaften und Beziehungen der [AndroidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="f6629-107">List properties and relationships of the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f6629-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f6629-108">Prerequisites</span></span>
<span data-ttu-id="f6629-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6629-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6629-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6629-111">Permission type</span></span>|<span data-ttu-id="f6629-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6629-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6629-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6629-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6629-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6629-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f6629-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6629-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6629-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6629-116">Not supported.</span></span>|
|<span data-ttu-id="f6629-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6629-117">Application</span></span>|<span data-ttu-id="f6629-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6629-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6629-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6629-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f6629-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6629-120">Request headers</span></span>
|<span data-ttu-id="f6629-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f6629-121">Header</span></span>|<span data-ttu-id="f6629-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f6629-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6629-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6629-123">Authorization</span></span>|<span data-ttu-id="f6629-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6629-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6629-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6629-125">Accept</span></span>|<span data-ttu-id="f6629-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6629-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6629-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6629-127">Request body</span></span>
<span data-ttu-id="f6629-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f6629-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6629-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6629-129">Response</span></span>
<span data-ttu-id="f6629-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f6629-130">If successful, this method returns a `200 OK` response code and a collection of [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6629-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6629-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6629-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6629-132">Request</span></span>
<span data-ttu-id="f6629-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6629-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f6629-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6629-134">Response</span></span>
<span data-ttu-id="f6629-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6629-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1102

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
      "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountName": "Account Name value",
      "authenticationMethod": "certificate",
      "syncCalendar": true,
      "syncContacts": true,
      "syncTasks": true,
      "syncNotes": true,
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "emailSyncSchedule": "asMessagesArrive",
      "hostName": "Host Name value",
      "requireSmime": true,
      "requireSsl": true,
      "usernameSource": "userPrincipalName",
      "userDomainNameSource": "netBiosDomainName",
      "customDomainName": "Custom Domain Name value"
    }
  ]
}
```





