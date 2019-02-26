---
title: WindowsUniversalAppXContainedApp erstellen
description: Erstellen eines neuen windowsUniversalAppXContainedApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72e171d4a967b9b8dcc7a5271ba09c2afe8c6744
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164855"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="c3373-103">WindowsUniversalAppXContainedApp erstellen</span><span class="sxs-lookup"><span data-stu-id="c3373-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="c3373-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c3373-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3373-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c3373-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3373-106">Erstellen eines neuen [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c3373-106">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3373-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c3373-107">Prerequisites</span></span>
<span data-ttu-id="c3373-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c3373-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c3373-110">Permission type</span></span>|<span data-ttu-id="c3373-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c3373-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3373-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c3373-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3373-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3373-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3373-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c3373-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3373-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3373-115">Not supported.</span></span>|
|<span data-ttu-id="c3373-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3373-116">Application</span></span>|<span data-ttu-id="c3373-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3373-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3373-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3373-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="c3373-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c3373-119">Request headers</span></span>
|<span data-ttu-id="c3373-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c3373-120">Header</span></span>|<span data-ttu-id="c3373-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c3373-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3373-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3373-122">Authorization</span></span>|<span data-ttu-id="c3373-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c3373-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3373-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c3373-124">Accept</span></span>|<span data-ttu-id="c3373-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3373-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3373-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c3373-126">Request body</span></span>
<span data-ttu-id="c3373-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsUniversalAppXContainedApp-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c3373-127">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="c3373-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsUniversalAppXContainedApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c3373-128">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="c3373-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3373-129">Property</span></span>|<span data-ttu-id="c3373-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c3373-130">Type</span></span>|<span data-ttu-id="c3373-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3373-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3373-132">id</span><span class="sxs-lookup"><span data-stu-id="c3373-132">id</span></span>|<span data-ttu-id="c3373-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c3373-133">String</span></span>|<span data-ttu-id="c3373-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c3373-134">Key of the entity.</span></span> <span data-ttu-id="c3373-135">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3373-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="c3373-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="c3373-136">appUserModelId</span></span>|<span data-ttu-id="c3373-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c3373-137">String</span></span>|<span data-ttu-id="c3373-138">Die APP-Benutzermodell-ID der enthaltenen App einer WindowsUniversalAppX-app.</span><span class="sxs-lookup"><span data-stu-id="c3373-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="c3373-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3373-139">Response</span></span>
<span data-ttu-id="c3373-140">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c3373-140">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3373-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c3373-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3373-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3373-142">Request</span></span>
<span data-ttu-id="c3373-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c3373-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="c3373-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3373-144">Response</span></span>
<span data-ttu-id="c3373-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3373-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```




