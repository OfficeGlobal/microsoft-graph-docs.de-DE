---
title: Liste androidWorkProfileNineWorkEasConfigurations
description: Listeneigenschaften und Beziehungen der AndroidWorkProfileNineWorkEasConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5654cc7125337d356c0395273a54e7b451bca92e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891910"
---
# <a name="list-androidworkprofilenineworkeasconfigurations"></a><span data-ttu-id="44e37-103">Liste androidWorkProfileNineWorkEasConfigurations</span><span class="sxs-lookup"><span data-stu-id="44e37-103">List androidWorkProfileNineWorkEasConfigurations</span></span>

> <span data-ttu-id="44e37-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="44e37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44e37-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44e37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44e37-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="44e37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44e37-107">Listeneigenschaften und Beziehungen der [AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="44e37-107">List properties and relationships of the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44e37-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="44e37-108">Prerequisites</span></span>
<span data-ttu-id="44e37-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44e37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44e37-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44e37-111">Permission type</span></span>|<span data-ttu-id="44e37-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44e37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44e37-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44e37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44e37-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e37-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="44e37-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44e37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44e37-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44e37-116">Not supported.</span></span>|
|<span data-ttu-id="44e37-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44e37-117">Application</span></span>|<span data-ttu-id="44e37-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44e37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44e37-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44e37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="44e37-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44e37-120">Request headers</span></span>
|<span data-ttu-id="44e37-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="44e37-121">Header</span></span>|<span data-ttu-id="44e37-122">Wert</span><span class="sxs-lookup"><span data-stu-id="44e37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44e37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44e37-123">Authorization</span></span>|<span data-ttu-id="44e37-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="44e37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44e37-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="44e37-125">Accept</span></span>|<span data-ttu-id="44e37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44e37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44e37-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44e37-127">Request body</span></span>
<span data-ttu-id="44e37-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="44e37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44e37-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="44e37-129">Response</span></span>
<span data-ttu-id="44e37-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="44e37-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44e37-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44e37-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="44e37-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44e37-132">Request</span></span>
<span data-ttu-id="44e37-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44e37-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="44e37-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="44e37-134">Response</span></span>
<span data-ttu-id="44e37-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44e37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
      "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "authenticationMethod": "certificate",
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "hostName": "Host Name value",
      "requireSsl": true,
      "usernameSource": "userPrincipalName",
      "syncCalendar": true,
      "syncContacts": true,
      "syncTasks": true
    }
  ]
}
```





