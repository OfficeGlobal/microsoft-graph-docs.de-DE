---
title: DeviceConfigurationUserStateSummary aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceConfigurationUserStateSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7bce2ebe487805526ab51199c13dc5d65215175d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933169"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="2d31e-103">DeviceConfigurationUserStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2d31e-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="2d31e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2d31e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d31e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d31e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d31e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2d31e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d31e-107">Aktualisieren Sie die Eigenschaften eines [DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2d31e-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d31e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2d31e-108">Prerequisites</span></span>
<span data-ttu-id="2d31e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d31e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d31e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d31e-111">Permission type</span></span>|<span data-ttu-id="2d31e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d31e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d31e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d31e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d31e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d31e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d31e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d31e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d31e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d31e-116">Not supported.</span></span>|
|<span data-ttu-id="2d31e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d31e-117">Application</span></span>|<span data-ttu-id="2d31e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d31e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d31e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d31e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2d31e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d31e-120">Request headers</span></span>
|<span data-ttu-id="2d31e-121">Header</span><span class="sxs-lookup"><span data-stu-id="2d31e-121">Header</span></span>|<span data-ttu-id="2d31e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2d31e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d31e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d31e-123">Authorization</span></span>|<span data-ttu-id="2d31e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2d31e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d31e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2d31e-125">Accept</span></span>|<span data-ttu-id="2d31e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d31e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d31e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d31e-127">Request body</span></span>
<span data-ttu-id="2d31e-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2d31e-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="2d31e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="2d31e-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="2d31e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d31e-130">Property</span></span>|<span data-ttu-id="2d31e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2d31e-131">Type</span></span>|<span data-ttu-id="2d31e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d31e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d31e-133">id</span><span class="sxs-lookup"><span data-stu-id="2d31e-133">id</span></span>|<span data-ttu-id="2d31e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2d31e-134">String</span></span>|<span data-ttu-id="2d31e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2d31e-135">Key of the entity.</span></span>|
|<span data-ttu-id="2d31e-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="2d31e-136">unknownUserCount</span></span>|<span data-ttu-id="2d31e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2d31e-137">Int32</span></span>|<span data-ttu-id="2d31e-138">Unbekannte Benutzeranzahl</span><span class="sxs-lookup"><span data-stu-id="2d31e-138">Number of unknown users</span></span>|
|<span data-ttu-id="2d31e-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="2d31e-139">notApplicableUserCount</span></span>|<span data-ttu-id="2d31e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2d31e-140">Int32</span></span>|<span data-ttu-id="2d31e-141">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="2d31e-141">Number of not applicable users</span></span>|
|<span data-ttu-id="2d31e-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="2d31e-142">compliantUserCount</span></span>|<span data-ttu-id="2d31e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2d31e-143">Int32</span></span>|<span data-ttu-id="2d31e-144">Kompatible Benutzeranzahl</span><span class="sxs-lookup"><span data-stu-id="2d31e-144">Number of compliant users</span></span>|
|<span data-ttu-id="2d31e-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="2d31e-145">remediatedUserCount</span></span>|<span data-ttu-id="2d31e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2d31e-146">Int32</span></span>|<span data-ttu-id="2d31e-147">Für gewartete Benutzeranzahl</span><span class="sxs-lookup"><span data-stu-id="2d31e-147">Number of remediated users</span></span>|
|<span data-ttu-id="2d31e-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="2d31e-148">nonCompliantUserCount</span></span>|<span data-ttu-id="2d31e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2d31e-149">Int32</span></span>|<span data-ttu-id="2d31e-150">Nicht konformer Benutzeranzahl</span><span class="sxs-lookup"><span data-stu-id="2d31e-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="2d31e-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="2d31e-151">errorUserCount</span></span>|<span data-ttu-id="2d31e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2d31e-152">Int32</span></span>|<span data-ttu-id="2d31e-153">Anzahl der Fehler Benutzer</span><span class="sxs-lookup"><span data-stu-id="2d31e-153">Number of error users</span></span>|
|<span data-ttu-id="2d31e-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="2d31e-154">conflictUserCount</span></span>|<span data-ttu-id="2d31e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="2d31e-155">Int32</span></span>|<span data-ttu-id="2d31e-156">Anzahl der Conflict-Benutzer</span><span class="sxs-lookup"><span data-stu-id="2d31e-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="2d31e-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d31e-157">Response</span></span>
<span data-ttu-id="2d31e-158">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2d31e-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d31e-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d31e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d31e-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d31e-160">Request</span></span>
<span data-ttu-id="2d31e-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d31e-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 201

{
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a><span data-ttu-id="2d31e-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d31e-162">Response</span></span>
<span data-ttu-id="2d31e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d31e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "e8957887-7887-e895-8778-95e8877895e8",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```





