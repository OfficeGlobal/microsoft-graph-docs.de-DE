---
title: AssignedAccessMultiModeProfiles Aktion
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d379fce448f9bdc2191c6038117384ba6a73a042
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415859"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="e5f87-103">AssignedAccessMultiModeProfiles Aktion</span><span class="sxs-lookup"><span data-stu-id="e5f87-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="e5f87-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e5f87-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e5f87-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5f87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5f87-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e5f87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5f87-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e5f87-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5f87-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e5f87-108">Prerequisites</span></span>
<span data-ttu-id="e5f87-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e5f87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e5f87-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e5f87-111">Permission type</span></span>|<span data-ttu-id="e5f87-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e5f87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5f87-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e5f87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5f87-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5f87-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e5f87-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e5f87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5f87-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5f87-116">Not supported.</span></span>|
|<span data-ttu-id="e5f87-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e5f87-117">Application</span></span>|<span data-ttu-id="e5f87-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5f87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5f87-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5f87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e5f87-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e5f87-120">Request headers</span></span>
|<span data-ttu-id="e5f87-121">Header</span><span class="sxs-lookup"><span data-stu-id="e5f87-121">Header</span></span>|<span data-ttu-id="e5f87-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e5f87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5f87-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e5f87-123">Authorization</span></span>|<span data-ttu-id="e5f87-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e5f87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5f87-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e5f87-125">Accept</span></span>|<span data-ttu-id="e5f87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5f87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5f87-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e5f87-127">Request body</span></span>
<span data-ttu-id="e5f87-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="e5f87-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e5f87-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e5f87-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e5f87-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e5f87-130">Property</span></span>|<span data-ttu-id="e5f87-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e5f87-131">Type</span></span>|<span data-ttu-id="e5f87-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5f87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5f87-133">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="e5f87-133">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="e5f87-134">**WindowsAssignedAccessProfile** -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e5f87-134">**windowsAssignedAccessProfile** collection</span></span>|<span data-ttu-id="e5f87-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e5f87-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e5f87-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5f87-136">Response</span></span>
<span data-ttu-id="e5f87-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="e5f87-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e5f87-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5f87-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5f87-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5f87-139">Request</span></span>
<span data-ttu-id="e5f87-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e5f87-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles

Content-type: application/json
Content-length: 528

{
  "assignedAccessMultiModeProfiles": [
    {
      "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
      "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
      "profileName": "Profile Name value",
      "showTaskBar": true,
      "appUserModelIds": [
        "App User Model Ids value"
      ],
      "desktopAppPaths": [
        "Desktop App Paths value"
      ],
      "userAccounts": [
        "User Accounts value"
      ],
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e5f87-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5f87-141">Response</span></span>
<span data-ttu-id="e5f87-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5f87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




