---
title: Erstellen von sideLoadingKey
description: Erstellen eines neuen SideLoadingKey-Objekts.
author: tfitzmac
ms.openlocfilehash: 6edce1838499a73c2c28199a87c46fa44a10fe1f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356308"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="15670-103">Erstellen von sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="15670-103">Create sideLoadingKey</span></span>

> <span data-ttu-id="15670-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15670-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15670-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15670-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15670-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15670-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15670-107">Erstellen eines neuen [SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="15670-107">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15670-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15670-108">Prerequisites</span></span>
<span data-ttu-id="15670-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15670-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15670-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15670-111">Permission type</span></span>|<span data-ttu-id="15670-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15670-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15670-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15670-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15670-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15670-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15670-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15670-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15670-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15670-116">Not supported.</span></span>|
|<span data-ttu-id="15670-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15670-117">Application</span></span>|<span data-ttu-id="15670-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15670-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15670-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15670-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="15670-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15670-120">Request headers</span></span>
|<span data-ttu-id="15670-121">Header</span><span class="sxs-lookup"><span data-stu-id="15670-121">Header</span></span>|<span data-ttu-id="15670-122">Wert</span><span class="sxs-lookup"><span data-stu-id="15670-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15670-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="15670-123">Authorization</span></span>|<span data-ttu-id="15670-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15670-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15670-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15670-125">Accept</span></span>|<span data-ttu-id="15670-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15670-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15670-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15670-127">Request body</span></span>
<span data-ttu-id="15670-128">Geben Sie im Textkörper Anforderung für das Objekt SideLoadingKey eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="15670-128">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="15670-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die SideLoadingKey erstellen.</span><span class="sxs-lookup"><span data-stu-id="15670-129">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="15670-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15670-130">Property</span></span>|<span data-ttu-id="15670-131">Typ</span><span class="sxs-lookup"><span data-stu-id="15670-131">Type</span></span>|<span data-ttu-id="15670-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15670-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15670-133">id</span><span class="sxs-lookup"><span data-stu-id="15670-133">id</span></span>|<span data-ttu-id="15670-134">String</span><span class="sxs-lookup"><span data-stu-id="15670-134">String</span></span>|<span data-ttu-id="15670-135">Seite laden wichtige eindeutigen Bezeichner ab.</span><span class="sxs-lookup"><span data-stu-id="15670-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="15670-136">Wert</span><span class="sxs-lookup"><span data-stu-id="15670-136">value</span></span>|<span data-ttu-id="15670-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15670-137">String</span></span>|<span data-ttu-id="15670-138">Seite Laden von Schlüssel-Wert ist es 5 x 5-Wert durch Hiphens getrennt.</span><span class="sxs-lookup"><span data-stu-id="15670-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="15670-139">displayName</span><span class="sxs-lookup"><span data-stu-id="15670-139">displayName</span></span>|<span data-ttu-id="15670-140">String</span><span class="sxs-lookup"><span data-stu-id="15670-140">String</span></span>|<span data-ttu-id="15670-141">Seite laden Schlüsselname der ITPro Admins angezeigt.</span><span class="sxs-lookup"><span data-stu-id="15670-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="15670-142">description</span><span class="sxs-lookup"><span data-stu-id="15670-142">description</span></span>|<span data-ttu-id="15670-143">String</span><span class="sxs-lookup"><span data-stu-id="15670-143">String</span></span>|<span data-ttu-id="15670-144">Seite laden Schlüssel Beschreibung der ITPro Admins angezeigt.</span><span class="sxs-lookup"><span data-stu-id="15670-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="15670-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="15670-145">totalActivation</span></span>|<span data-ttu-id="15670-146">Int32</span><span class="sxs-lookup"><span data-stu-id="15670-146">Int32</span></span>|<span data-ttu-id="15670-147">Seite laden Key insgesamt Aktivierung der ITPro Admins angezeigt.</span><span class="sxs-lookup"><span data-stu-id="15670-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="15670-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="15670-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="15670-149">String</span><span class="sxs-lookup"><span data-stu-id="15670-149">String</span></span>|<span data-ttu-id="15670-150">Seite laden Schlüssel aktualisiert Datum der letzten die ITPro Admins angezeigt.</span><span class="sxs-lookup"><span data-stu-id="15670-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="15670-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="15670-151">Response</span></span>
<span data-ttu-id="15670-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="15670-152">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15670-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15670-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="15670-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15670-154">Request</span></span>
<span data-ttu-id="15670-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15670-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="15670-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="15670-156">Response</span></span>
<span data-ttu-id="15670-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15670-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```





