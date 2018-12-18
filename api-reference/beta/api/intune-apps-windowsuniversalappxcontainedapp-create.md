---
title: Erstellen von windowsUniversalAppXContainedApp
description: Erstellen eines neuen WindowsUniversalAppXContainedApp-Objekts.
author: tfitzmac
ms.openlocfilehash: 97f50a79194af878569327073ae8911bf08199f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302814"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="662fb-103">Erstellen von windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="662fb-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="662fb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="662fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="662fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="662fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="662fb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="662fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="662fb-107">Erstellen eines neuen [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="662fb-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="662fb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="662fb-108">Prerequisites</span></span>
<span data-ttu-id="662fb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="662fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="662fb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="662fb-111">Permission type</span></span>|<span data-ttu-id="662fb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="662fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="662fb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="662fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="662fb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="662fb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="662fb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="662fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="662fb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="662fb-116">Not supported.</span></span>|
|<span data-ttu-id="662fb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="662fb-117">Application</span></span>|<span data-ttu-id="662fb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="662fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="662fb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="662fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="662fb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="662fb-120">Request headers</span></span>
|<span data-ttu-id="662fb-121">Header</span><span class="sxs-lookup"><span data-stu-id="662fb-121">Header</span></span>|<span data-ttu-id="662fb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="662fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="662fb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="662fb-123">Authorization</span></span>|<span data-ttu-id="662fb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="662fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="662fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="662fb-125">Accept</span></span>|<span data-ttu-id="662fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="662fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="662fb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="662fb-127">Request body</span></span>
<span data-ttu-id="662fb-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsUniversalAppXContainedApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="662fb-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="662fb-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsUniversalAppXContainedApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="662fb-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="662fb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="662fb-130">Property</span></span>|<span data-ttu-id="662fb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="662fb-131">Type</span></span>|<span data-ttu-id="662fb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="662fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="662fb-133">id</span><span class="sxs-lookup"><span data-stu-id="662fb-133">id</span></span>|<span data-ttu-id="662fb-134">String</span><span class="sxs-lookup"><span data-stu-id="662fb-134">String</span></span>|<span data-ttu-id="662fb-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="662fb-135">Key of the entity.</span></span> <span data-ttu-id="662fb-136">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="662fb-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="662fb-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="662fb-137">appUserModelId</span></span>|<span data-ttu-id="662fb-138">String</span><span class="sxs-lookup"><span data-stu-id="662fb-138">String</span></span>|<span data-ttu-id="662fb-139">Die app Benutzer Modell-ID der app enthaltenen einer WindowsUniversalAppX-App.</span><span class="sxs-lookup"><span data-stu-id="662fb-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="662fb-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="662fb-140">Response</span></span>
<span data-ttu-id="662fb-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="662fb-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="662fb-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="662fb-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="662fb-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="662fb-143">Request</span></span>
<span data-ttu-id="662fb-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="662fb-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="662fb-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="662fb-145">Response</span></span>
<span data-ttu-id="662fb-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="662fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





