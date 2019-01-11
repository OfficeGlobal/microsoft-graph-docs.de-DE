---
title: Erstellen von microsoftStoreForBusinessContainedApp
description: Erstellen eines neuen MicrosoftStoreForBusinessContainedApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ac782261c00008bf9b4ab552932f8f841a9965bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843295"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="75fce-103">Erstellen von microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="75fce-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="75fce-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="75fce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75fce-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="75fce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75fce-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="75fce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75fce-107">Erstellen eines neuen [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="75fce-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75fce-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="75fce-108">Prerequisites</span></span>
<span data-ttu-id="75fce-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75fce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75fce-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75fce-111">Permission type</span></span>|<span data-ttu-id="75fce-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="75fce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75fce-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75fce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75fce-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75fce-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="75fce-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="75fce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75fce-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75fce-116">Not supported.</span></span>|
|<span data-ttu-id="75fce-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75fce-117">Application</span></span>|<span data-ttu-id="75fce-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75fce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75fce-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75fce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="75fce-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75fce-120">Request headers</span></span>
|<span data-ttu-id="75fce-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="75fce-121">Header</span></span>|<span data-ttu-id="75fce-122">Wert</span><span class="sxs-lookup"><span data-stu-id="75fce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75fce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75fce-123">Authorization</span></span>|<span data-ttu-id="75fce-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="75fce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75fce-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="75fce-125">Accept</span></span>|<span data-ttu-id="75fce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75fce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75fce-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75fce-127">Request body</span></span>
<span data-ttu-id="75fce-128">Geben Sie im Textkörper Anforderung für das Objekt MicrosoftStoreForBusinessContainedApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="75fce-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="75fce-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MicrosoftStoreForBusinessContainedApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="75fce-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="75fce-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="75fce-130">Property</span></span>|<span data-ttu-id="75fce-131">Typ</span><span class="sxs-lookup"><span data-stu-id="75fce-131">Type</span></span>|<span data-ttu-id="75fce-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75fce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75fce-133">id</span><span class="sxs-lookup"><span data-stu-id="75fce-133">id</span></span>|<span data-ttu-id="75fce-134">String</span><span class="sxs-lookup"><span data-stu-id="75fce-134">String</span></span>|<span data-ttu-id="75fce-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="75fce-135">Key of the entity.</span></span> <span data-ttu-id="75fce-136">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="75fce-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="75fce-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="75fce-137">appUserModelId</span></span>|<span data-ttu-id="75fce-138">String</span><span class="sxs-lookup"><span data-stu-id="75fce-138">String</span></span>|<span data-ttu-id="75fce-139">Die app Benutzer Modell-ID der app enthaltenen von einer MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="75fce-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="75fce-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="75fce-140">Response</span></span>
<span data-ttu-id="75fce-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="75fce-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75fce-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75fce-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="75fce-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75fce-143">Request</span></span>
<span data-ttu-id="75fce-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75fce-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="75fce-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="75fce-145">Response</span></span>
<span data-ttu-id="75fce-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75fce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```





