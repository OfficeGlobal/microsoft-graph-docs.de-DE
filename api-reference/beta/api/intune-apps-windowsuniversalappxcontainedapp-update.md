---
title: WindowsUniversalAppXContainedApp aktualisieren
description: Aktualisieren der Eigenschaften eines windowsUniversalAppXContainedApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4eeae30dd48689b2df656a5ea78139af01970c1b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959159"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="b9e0d-103">WindowsUniversalAppXContainedApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b9e0d-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="b9e0d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9e0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9e0d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b9e0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9e0d-106">Aktualisieren der Eigenschaften eines [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9e0d-106">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9e0d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9e0d-107">Prerequisites</span></span>
<span data-ttu-id="b9e0d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9e0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9e0d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9e0d-110">Permission type</span></span>|<span data-ttu-id="b9e0d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9e0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9e0d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9e0d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9e0d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e0d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b9e0d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9e0d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9e0d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9e0d-115">Not supported.</span></span>|
|<span data-ttu-id="b9e0d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9e0d-116">Application</span></span>|<span data-ttu-id="b9e0d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9e0d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9e0d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9e0d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b9e0d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9e0d-119">Request headers</span></span>
|<span data-ttu-id="b9e0d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b9e0d-120">Header</span></span>|<span data-ttu-id="b9e0d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b9e0d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9e0d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e0d-122">Authorization</span></span>|<span data-ttu-id="b9e0d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9e0d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9e0d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b9e0d-124">Accept</span></span>|<span data-ttu-id="b9e0d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9e0d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e0d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9e0d-126">Request body</span></span>
<span data-ttu-id="b9e0d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b9e0d-127">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="b9e0d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b9e0d-128">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="b9e0d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9e0d-129">Property</span></span>|<span data-ttu-id="b9e0d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b9e0d-130">Type</span></span>|<span data-ttu-id="b9e0d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9e0d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9e0d-132">id</span><span class="sxs-lookup"><span data-stu-id="b9e0d-132">id</span></span>|<span data-ttu-id="b9e0d-133">String</span><span class="sxs-lookup"><span data-stu-id="b9e0d-133">String</span></span>|<span data-ttu-id="b9e0d-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b9e0d-134">Key of the entity.</span></span> <span data-ttu-id="b9e0d-135">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9e0d-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="b9e0d-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="b9e0d-136">appUserModelId</span></span>|<span data-ttu-id="b9e0d-137">String</span><span class="sxs-lookup"><span data-stu-id="b9e0d-137">String</span></span>|<span data-ttu-id="b9e0d-138">Die APP-Benutzermodell-ID der enthaltenen App einer WindowsUniversalAppX-app.</span><span class="sxs-lookup"><span data-stu-id="b9e0d-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="b9e0d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9e0d-139">Response</span></span>
<span data-ttu-id="b9e0d-140">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b9e0d-140">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9e0d-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9e0d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9e0d-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9e0d-142">Request</span></span>
<span data-ttu-id="b9e0d-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9e0d-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="b9e0d-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9e0d-144">Response</span></span>
<span data-ttu-id="b9e0d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9e0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```




