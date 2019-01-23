---
title: Erstellen von windowsUniversalAppXContainedApp
description: Erstellen eines neuen WindowsUniversalAppXContainedApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a86c8c329bac55b6497a28f0aaa6096d6e9f4e94
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418435"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="2d593-103">Erstellen von windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="2d593-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="2d593-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2d593-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2d593-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d593-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d593-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d593-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d593-107">Erstellen eines neuen [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2d593-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d593-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2d593-108">Prerequisites</span></span>
<span data-ttu-id="2d593-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d593-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2d593-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d593-111">Permission type</span></span>|<span data-ttu-id="2d593-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d593-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d593-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d593-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d593-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d593-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d593-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d593-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d593-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d593-116">Not supported.</span></span>|
|<span data-ttu-id="2d593-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d593-117">Application</span></span>|<span data-ttu-id="2d593-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d593-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d593-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d593-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="2d593-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d593-120">Request headers</span></span>
|<span data-ttu-id="2d593-121">Header</span><span class="sxs-lookup"><span data-stu-id="2d593-121">Header</span></span>|<span data-ttu-id="2d593-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2d593-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d593-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2d593-123">Authorization</span></span>|<span data-ttu-id="2d593-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2d593-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d593-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2d593-125">Accept</span></span>|<span data-ttu-id="2d593-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d593-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d593-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d593-127">Request body</span></span>
<span data-ttu-id="2d593-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsUniversalAppXContainedApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2d593-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="2d593-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsUniversalAppXContainedApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="2d593-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="2d593-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d593-130">Property</span></span>|<span data-ttu-id="2d593-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2d593-131">Type</span></span>|<span data-ttu-id="2d593-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d593-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d593-133">id</span><span class="sxs-lookup"><span data-stu-id="2d593-133">id</span></span>|<span data-ttu-id="2d593-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d593-134">String</span></span>|<span data-ttu-id="2d593-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2d593-135">Key of the entity.</span></span> <span data-ttu-id="2d593-136">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d593-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="2d593-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="2d593-137">appUserModelId</span></span>|<span data-ttu-id="2d593-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d593-138">String</span></span>|<span data-ttu-id="2d593-139">Die app Benutzer Modell-ID der app enthaltenen einer WindowsUniversalAppX-App.</span><span class="sxs-lookup"><span data-stu-id="2d593-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="2d593-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d593-140">Response</span></span>
<span data-ttu-id="2d593-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2d593-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d593-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d593-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d593-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d593-143">Request</span></span>
<span data-ttu-id="2d593-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d593-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="2d593-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d593-145">Response</span></span>
<span data-ttu-id="2d593-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d593-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




