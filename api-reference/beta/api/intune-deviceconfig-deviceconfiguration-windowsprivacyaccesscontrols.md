---
title: WindowsPrivacyAccessControls Aktion
description: Noch nicht dokumentiert
ms.openlocfilehash: b9b8a3e9d5042d4bb896ac4a0f310f78d7bd78a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063378"
---
# <a name="windowsprivacyaccesscontrols-action"></a><span data-ttu-id="14aaf-103">WindowsPrivacyAccessControls Aktion</span><span class="sxs-lookup"><span data-stu-id="14aaf-103">windowsPrivacyAccessControls action</span></span>

> <span data-ttu-id="14aaf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="14aaf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14aaf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="14aaf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14aaf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="14aaf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14aaf-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="14aaf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14aaf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="14aaf-108">Prerequisites</span></span>
<span data-ttu-id="14aaf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14aaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14aaf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="14aaf-111">Permission type</span></span>|<span data-ttu-id="14aaf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="14aaf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14aaf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="14aaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14aaf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14aaf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14aaf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="14aaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14aaf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14aaf-116">Not supported.</span></span>|
|<span data-ttu-id="14aaf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="14aaf-117">Application</span></span>|<span data-ttu-id="14aaf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14aaf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14aaf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="14aaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="14aaf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="14aaf-120">Request headers</span></span>
|<span data-ttu-id="14aaf-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="14aaf-121">Header</span></span>|<span data-ttu-id="14aaf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="14aaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14aaf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14aaf-123">Authorization</span></span>|<span data-ttu-id="14aaf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="14aaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14aaf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14aaf-125">Accept</span></span>|<span data-ttu-id="14aaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14aaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14aaf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="14aaf-127">Request body</span></span>
<span data-ttu-id="14aaf-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="14aaf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="14aaf-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="14aaf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="14aaf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14aaf-130">Property</span></span>|<span data-ttu-id="14aaf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="14aaf-131">Type</span></span>|<span data-ttu-id="14aaf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14aaf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14aaf-133">windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="14aaf-133">windowsPrivacyAccessControls</span></span>|<span data-ttu-id="14aaf-134">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="14aaf-134">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="14aaf-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="14aaf-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="14aaf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="14aaf-136">Response</span></span>
<span data-ttu-id="14aaf-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="14aaf-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="14aaf-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="14aaf-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="14aaf-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="14aaf-139">Request</span></span>
<span data-ttu-id="14aaf-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="14aaf-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls

Content-type: application/json
Content-length: 379

{
  "windowsPrivacyAccessControls": [
    {
      "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
      "id": "03b15556-5556-03b1-5655-b1035655b103",
      "accessLevel": "forceAllow",
      "dataCategory": "accountInfo",
      "appPackageFamilyName": "App Package Family Name value",
      "appDisplayName": "App Display Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="14aaf-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="14aaf-141">Response</span></span>
<span data-ttu-id="14aaf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14aaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





