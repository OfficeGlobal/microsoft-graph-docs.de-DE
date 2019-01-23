---
title: iosMobileAppConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des iosMobileAppConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42d2da4e18d59a6dbb2b27f954b280af5a1b4e19
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394341"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="e7c4d-103">iosMobileAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="e7c4d-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="e7c4d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e7c4d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e7c4d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e7c4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7c4d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e7c4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7c4d-107">Lesen von Eigenschaften und Beziehungen des [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e7c4d-107">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7c4d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e7c4d-108">Prerequisites</span></span>
<span data-ttu-id="e7c4d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7c4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7c4d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7c4d-111">Permission type</span></span>|<span data-ttu-id="e7c4d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7c4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c4d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7c4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7c4d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c4d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e7c4d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7c4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c4d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7c4d-116">Not supported.</span></span>|
|<span data-ttu-id="e7c4d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7c4d-117">Application</span></span>|<span data-ttu-id="e7c4d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7c4d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c4d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7c4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7c4d-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e7c4d-120">Optional query parameters</span></span>
<span data-ttu-id="e7c4d-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e7c4d-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7c4d-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7c4d-122">Request headers</span></span>
|<span data-ttu-id="e7c4d-123">Header</span><span class="sxs-lookup"><span data-stu-id="e7c4d-123">Header</span></span>|<span data-ttu-id="e7c4d-124">Wert</span><span class="sxs-lookup"><span data-stu-id="e7c4d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c4d-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e7c4d-125">Authorization</span></span>|<span data-ttu-id="e7c4d-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e7c4d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c4d-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e7c4d-127">Accept</span></span>|<span data-ttu-id="e7c4d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c4d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c4d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7c4d-129">Request body</span></span>
<span data-ttu-id="e7c4d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e7c4d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7c4d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7c4d-131">Response</span></span>
<span data-ttu-id="e7c4d-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e7c4d-132">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c4d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7c4d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7c4d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7c4d-134">Request</span></span>
<span data-ttu-id="e7c4d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e7c4d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e7c4d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7c4d-136">Response</span></span>
<span data-ttu-id="e7c4d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7c4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 831

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
    "settings": [
      {
        "@odata.type": "microsoft.graph.appConfigurationSettingItem",
        "appConfigKey": "App Config Key value",
        "appConfigKeyType": "integerType",
        "appConfigKeyValue": "App Config Key Value value"
      }
    ]
  }
}
```




