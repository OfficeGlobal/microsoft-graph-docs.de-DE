---
title: Erstellen von microsoftStoreForBusinessContainedApp
description: Erstellen eines neuen MicrosoftStoreForBusinessContainedApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1286ccdd3f87f7669b13c63063c0bc78e8cc633
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421137"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="1b972-103">Erstellen von microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="1b972-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="1b972-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1b972-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1b972-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b972-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b972-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1b972-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b972-107">Erstellen eines neuen [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b972-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b972-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1b972-108">Prerequisites</span></span>
<span data-ttu-id="1b972-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b972-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1b972-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b972-111">Permission type</span></span>|<span data-ttu-id="1b972-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b972-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b972-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b972-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b972-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b972-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b972-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b972-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b972-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b972-116">Not supported.</span></span>|
|<span data-ttu-id="1b972-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b972-117">Application</span></span>|<span data-ttu-id="1b972-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b972-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b972-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b972-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="1b972-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b972-120">Request headers</span></span>
|<span data-ttu-id="1b972-121">Header</span><span class="sxs-lookup"><span data-stu-id="1b972-121">Header</span></span>|<span data-ttu-id="1b972-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1b972-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b972-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1b972-123">Authorization</span></span>|<span data-ttu-id="1b972-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1b972-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b972-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1b972-125">Accept</span></span>|<span data-ttu-id="1b972-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b972-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b972-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b972-127">Request body</span></span>
<span data-ttu-id="1b972-128">Geben Sie im Textkörper Anforderung für das Objekt MicrosoftStoreForBusinessContainedApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1b972-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="1b972-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MicrosoftStoreForBusinessContainedApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="1b972-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="1b972-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b972-130">Property</span></span>|<span data-ttu-id="1b972-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1b972-131">Type</span></span>|<span data-ttu-id="1b972-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b972-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b972-133">id</span><span class="sxs-lookup"><span data-stu-id="1b972-133">id</span></span>|<span data-ttu-id="1b972-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b972-134">String</span></span>|<span data-ttu-id="1b972-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1b972-135">Key of the entity.</span></span> <span data-ttu-id="1b972-136">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b972-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="1b972-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="1b972-137">appUserModelId</span></span>|<span data-ttu-id="1b972-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b972-138">String</span></span>|<span data-ttu-id="1b972-139">Die app Benutzer Modell-ID der app enthaltenen von einer MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="1b972-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="1b972-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b972-140">Response</span></span>
<span data-ttu-id="1b972-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1b972-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b972-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b972-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b972-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b972-143">Request</span></span>
<span data-ttu-id="1b972-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b972-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="1b972-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b972-145">Response</span></span>
<span data-ttu-id="1b972-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b972-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




