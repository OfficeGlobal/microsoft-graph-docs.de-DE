---
title: WindowsPrivacyDataAccessControlItem abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsPrivacyDataAccessControlItem-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1620c645c55f3802923b89db4728ccb4af8c3487
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960482"
---
# <a name="get-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="f2595-103">WindowsPrivacyDataAccessControlItem abrufen</span><span class="sxs-lookup"><span data-stu-id="f2595-103">Get windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="f2595-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f2595-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2595-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f2595-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2595-106">Lesen von Eigenschaften und Beziehungen des [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f2595-106">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2595-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f2595-107">Prerequisites</span></span>
<span data-ttu-id="f2595-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2595-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2595-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2595-110">Permission type</span></span>|<span data-ttu-id="f2595-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2595-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2595-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2595-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2595-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2595-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f2595-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2595-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2595-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2595-115">Not supported.</span></span>|
|<span data-ttu-id="f2595-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2595-116">Application</span></span>|<span data-ttu-id="f2595-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2595-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2595-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2595-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2595-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f2595-119">Optional query parameters</span></span>
<span data-ttu-id="f2595-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f2595-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2595-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2595-121">Request headers</span></span>
|<span data-ttu-id="f2595-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f2595-122">Header</span></span>|<span data-ttu-id="f2595-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f2595-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2595-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2595-124">Authorization</span></span>|<span data-ttu-id="f2595-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f2595-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2595-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f2595-126">Accept</span></span>|<span data-ttu-id="f2595-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f2595-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2595-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2595-128">Request body</span></span>
<span data-ttu-id="f2595-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f2595-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2595-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2595-130">Response</span></span>
<span data-ttu-id="f2595-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f2595-131">If successful, this method returns a `200 OK` response code and [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2595-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2595-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2595-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2595-133">Request</span></span>
<span data-ttu-id="f2595-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2595-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

### <a name="response"></a><span data-ttu-id="f2595-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2595-135">Response</span></span>
<span data-ttu-id="f2595-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2595-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
    "id": "03b15556-5556-03b1-5655-b1035655b103",
    "accessLevel": "forceAllow",
    "dataCategory": "accountInfo",
    "appPackageFamilyName": "App Package Family Name value",
    "appDisplayName": "App Display Name value"
  }
}
```




