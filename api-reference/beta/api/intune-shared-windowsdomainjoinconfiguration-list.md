---
title: WindowsDomainJoinConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der windowsDomainJoinConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 19f4687039e2a07b32994d855f3e215da2af85c8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960265"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="8d369-103">WindowsDomainJoinConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="8d369-103">List windowsDomainJoinConfigurations</span></span>

> <span data-ttu-id="8d369-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="8d369-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8d369-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d369-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d369-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8d369-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d369-107">AufListen von Eigenschaften und Beziehungen der [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="8d369-107">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d369-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d369-108">Prerequisites</span></span>
<span data-ttu-id="8d369-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d369-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d369-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d369-111">Permission type</span></span>|<span data-ttu-id="8d369-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d369-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d369-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d369-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8d369-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="8d369-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8d369-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d369-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8d369-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d369-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d369-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d369-117">Not supported.</span></span>|
|<span data-ttu-id="8d369-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d369-118">Application</span></span>|<span data-ttu-id="8d369-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d369-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d369-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d369-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8d369-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d369-121">Request headers</span></span>
|<span data-ttu-id="8d369-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d369-122">Header</span></span>|<span data-ttu-id="8d369-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8d369-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d369-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d369-124">Authorization</span></span>|<span data-ttu-id="8d369-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d369-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d369-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8d369-126">Accept</span></span>|<span data-ttu-id="8d369-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8d369-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d369-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d369-128">Request body</span></span>
<span data-ttu-id="8d369-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8d369-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d369-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d369-130">Response</span></span>
<span data-ttu-id="8d369-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8d369-131">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d369-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d369-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d369-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d369-133">Request</span></span>
<span data-ttu-id="8d369-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d369-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8d369-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d369-135">Response</span></span>
<span data-ttu-id="8d369-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d369-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
      "id": "40118d08-8d08-4011-088d-1140088d1140",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "computerNameStaticPrefix": "Computer Name Static Prefix value",
      "computerNameSuffixRandomCharCount": 1,
      "activeDirectoryDomainName": "Active Directory Domain Name value",
      "organizationalUnit": "Organizational Unit value"
    }
  ]
}
```



