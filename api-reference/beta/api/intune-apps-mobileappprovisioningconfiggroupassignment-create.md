---
title: MobileAppProvisioningConfigGroupAssignment erstellen
description: Erstellen eines neuen mobileAppProvisioningConfigGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbb0a1190eb24bf0a00510061e6c71f238f7c84f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164715"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="c0bc0-103">MobileAppProvisioningConfigGroupAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="c0bc0-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="c0bc0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0bc0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0bc0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c0bc0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0bc0-106">Erstellen eines neuen [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c0bc0-106">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0bc0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0bc0-107">Prerequisites</span></span>
<span data-ttu-id="c0bc0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0bc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c0bc0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0bc0-110">Permission type</span></span>|<span data-ttu-id="c0bc0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0bc0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0bc0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0bc0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0bc0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0bc0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c0bc0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0bc0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0bc0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0bc0-115">Not supported.</span></span>|
|<span data-ttu-id="c0bc0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0bc0-116">Application</span></span>|<span data-ttu-id="c0bc0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0bc0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0bc0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0bc0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c0bc0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0bc0-119">Request headers</span></span>
|<span data-ttu-id="c0bc0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c0bc0-120">Header</span></span>|<span data-ttu-id="c0bc0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c0bc0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0bc0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0bc0-122">Authorization</span></span>|<span data-ttu-id="c0bc0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0bc0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0bc0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c0bc0-124">Accept</span></span>|<span data-ttu-id="c0bc0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0bc0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0bc0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0bc0-126">Request body</span></span>
<span data-ttu-id="c0bc0-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das mobileAppProvisioningConfigGroupAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c0bc0-127">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="c0bc0-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der mobileAppProvisioningConfigGroupAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c0bc0-128">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="c0bc0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0bc0-129">Property</span></span>|<span data-ttu-id="c0bc0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c0bc0-130">Type</span></span>|<span data-ttu-id="c0bc0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0bc0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0bc0-132">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="c0bc0-132">targetGroupId</span></span>|<span data-ttu-id="c0bc0-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0bc0-133">String</span></span>|<span data-ttu-id="c0bc0-134">Die ID der AAD-Gruppe, in der die APP-Konfigurations Konfiguration gezielt wird.</span><span class="sxs-lookup"><span data-stu-id="c0bc0-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="c0bc0-135">id</span><span class="sxs-lookup"><span data-stu-id="c0bc0-135">id</span></span>|<span data-ttu-id="c0bc0-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0bc0-136">String</span></span>|<span data-ttu-id="c0bc0-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c0bc0-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c0bc0-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0bc0-138">Response</span></span>
<span data-ttu-id="c0bc0-139">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c0bc0-139">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0bc0-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0bc0-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0bc0-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0bc0-141">Request</span></span>
<span data-ttu-id="c0bc0-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0bc0-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="c0bc0-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0bc0-143">Response</span></span>
<span data-ttu-id="c0bc0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0bc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```




