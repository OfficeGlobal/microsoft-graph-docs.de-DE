---
title: Abrufen von windowsPrivacyDataAccessControlItem
description: Lesen Sie Eigenschaften und Beziehungen des WindowsPrivacyDataAccessControlItem-Objekts.
ms.openlocfilehash: e349240a82bdd292b7f94c25a57475b2fdcce468
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059493"
---
# <a name="get-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="159c0-103">Abrufen von windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="159c0-103">Get windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="159c0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="159c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="159c0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="159c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="159c0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="159c0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="159c0-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="159c0-107">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="159c0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="159c0-108">Prerequisites</span></span>
<span data-ttu-id="159c0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="159c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="159c0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="159c0-111">Permission type</span></span>|<span data-ttu-id="159c0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="159c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="159c0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="159c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="159c0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="159c0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="159c0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="159c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="159c0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="159c0-116">Not supported.</span></span>|
|<span data-ttu-id="159c0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="159c0-117">Application</span></span>|<span data-ttu-id="159c0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="159c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="159c0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="159c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="159c0-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="159c0-120">Optional query parameters</span></span>
<span data-ttu-id="159c0-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="159c0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="159c0-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="159c0-122">Request headers</span></span>
|<span data-ttu-id="159c0-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="159c0-123">Header</span></span>|<span data-ttu-id="159c0-124">Wert</span><span class="sxs-lookup"><span data-stu-id="159c0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="159c0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="159c0-125">Authorization</span></span>|<span data-ttu-id="159c0-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="159c0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="159c0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="159c0-127">Accept</span></span>|<span data-ttu-id="159c0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="159c0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="159c0-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="159c0-129">Request body</span></span>
<span data-ttu-id="159c0-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="159c0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="159c0-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="159c0-131">Response</span></span>
<span data-ttu-id="159c0-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="159c0-132">If successful, this method returns a `200 OK` response code and [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="159c0-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="159c0-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="159c0-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="159c0-134">Request</span></span>
<span data-ttu-id="159c0-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="159c0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

### <a name="response"></a><span data-ttu-id="159c0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="159c0-136">Response</span></span>
<span data-ttu-id="159c0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="159c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





