---
title: WindowsPrivacyAccessControls Aktion
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 24d9b0160cbc21df62b846f20128e6c0733862fe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400872"
---
# <a name="windowsprivacyaccesscontrols-action"></a><span data-ttu-id="25339-103">WindowsPrivacyAccessControls Aktion</span><span class="sxs-lookup"><span data-stu-id="25339-103">windowsPrivacyAccessControls action</span></span>

> <span data-ttu-id="25339-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="25339-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="25339-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25339-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25339-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25339-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="25339-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25339-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="25339-108">Prerequisites</span></span>
<span data-ttu-id="25339-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="25339-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="25339-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25339-111">Permission type</span></span>|<span data-ttu-id="25339-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25339-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25339-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25339-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25339-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25339-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25339-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25339-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25339-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25339-116">Not supported.</span></span>|
|<span data-ttu-id="25339-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25339-117">Application</span></span>|<span data-ttu-id="25339-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25339-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25339-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25339-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="25339-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="25339-120">Request headers</span></span>
|<span data-ttu-id="25339-121">Header</span><span class="sxs-lookup"><span data-stu-id="25339-121">Header</span></span>|<span data-ttu-id="25339-122">Wert</span><span class="sxs-lookup"><span data-stu-id="25339-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25339-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="25339-123">Authorization</span></span>|<span data-ttu-id="25339-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="25339-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25339-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="25339-125">Accept</span></span>|<span data-ttu-id="25339-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25339-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25339-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25339-127">Request body</span></span>
<span data-ttu-id="25339-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="25339-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="25339-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="25339-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="25339-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="25339-130">Property</span></span>|<span data-ttu-id="25339-131">Typ</span><span class="sxs-lookup"><span data-stu-id="25339-131">Type</span></span>|<span data-ttu-id="25339-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25339-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25339-133">windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="25339-133">windowsPrivacyAccessControls</span></span>|<span data-ttu-id="25339-134">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="25339-134">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="25339-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="25339-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="25339-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="25339-136">Response</span></span>
<span data-ttu-id="25339-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="25339-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="25339-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="25339-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="25339-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25339-139">Request</span></span>
<span data-ttu-id="25339-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="25339-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25339-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="25339-141">Response</span></span>
<span data-ttu-id="25339-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25339-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




