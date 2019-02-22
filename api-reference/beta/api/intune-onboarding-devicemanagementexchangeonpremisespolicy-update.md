---
title: DeviceManagementExchangeOnPremisesPolicy aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementExchangeOnPremisesPolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a94f22aa4d7dffcd448ad5e742198ddca809d781
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168026"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="d98e2-103">DeviceManagementExchangeOnPremisesPolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d98e2-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="d98e2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d98e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d98e2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d98e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d98e2-106">Aktualisieren der Eigenschaften eines [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d98e2-106">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d98e2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d98e2-107">Prerequisites</span></span>
<span data-ttu-id="d98e2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d98e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d98e2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d98e2-110">Permission type</span></span>|<span data-ttu-id="d98e2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d98e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d98e2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d98e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d98e2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98e2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d98e2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d98e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d98e2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d98e2-115">Not supported.</span></span>|
|<span data-ttu-id="d98e2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d98e2-116">Application</span></span>|<span data-ttu-id="d98e2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d98e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d98e2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d98e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="d98e2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d98e2-119">Request headers</span></span>
|<span data-ttu-id="d98e2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d98e2-120">Header</span></span>|<span data-ttu-id="d98e2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d98e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d98e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d98e2-122">Authorization</span></span>|<span data-ttu-id="d98e2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d98e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d98e2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d98e2-124">Accept</span></span>|<span data-ttu-id="d98e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d98e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d98e2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d98e2-126">Request body</span></span>
<span data-ttu-id="d98e2-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d98e2-127">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="d98e2-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d98e2-128">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="d98e2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d98e2-129">Property</span></span>|<span data-ttu-id="d98e2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d98e2-130">Type</span></span>|<span data-ttu-id="d98e2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d98e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d98e2-132">id</span><span class="sxs-lookup"><span data-stu-id="d98e2-132">id</span></span>|<span data-ttu-id="d98e2-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d98e2-133">String</span></span>|<span data-ttu-id="d98e2-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d98e2-134">Not yet documented</span></span>|
|<span data-ttu-id="d98e2-135">notificationContent</span><span class="sxs-lookup"><span data-stu-id="d98e2-135">notificationContent</span></span>|<span data-ttu-id="d98e2-136">Binär</span><span class="sxs-lookup"><span data-stu-id="d98e2-136">Binary</span></span>|<span data-ttu-id="d98e2-137">Benachrichtigungstext, der an Benutzer gesendet wird, die von dieser Richtlinie isoliert werden.</span><span class="sxs-lookup"><span data-stu-id="d98e2-137">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="d98e2-138">Dies ist ein UTF8-codiertes Bytearray.</span><span class="sxs-lookup"><span data-stu-id="d98e2-138">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="d98e2-139">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="d98e2-139">defaultAccessLevel</span></span>|[<span data-ttu-id="d98e2-140">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="d98e2-140">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="d98e2-141">Standardzugriffsstatus in Exchange.</span><span class="sxs-lookup"><span data-stu-id="d98e2-141">Default access state in Exchange.</span></span> <span data-ttu-id="d98e2-142">Diese Regel gilt global für die gesamte Exchange-Organisation.</span><span class="sxs-lookup"><span data-stu-id="d98e2-142">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="d98e2-143">Mögliche Werte: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="d98e2-143">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="d98e2-144">accessRules</span><span class="sxs-lookup"><span data-stu-id="d98e2-144">accessRules</span></span>|<span data-ttu-id="d98e2-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d98e2-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="d98e2-146">Die Liste der Gerätezugriffsregeln in Exchange.</span><span class="sxs-lookup"><span data-stu-id="d98e2-146">The list of device access rules in Exchange.</span></span> <span data-ttu-id="d98e2-147">Die Zugriffsregeln gelten global für die gesamte Exchange-Organisation.</span><span class="sxs-lookup"><span data-stu-id="d98e2-147">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="d98e2-148">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="d98e2-148">knownDeviceClasses</span></span>|<span data-ttu-id="d98e2-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d98e2-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="d98e2-150">Die Liste der Geräteklassen, die Exchange bekannt ist</span><span class="sxs-lookup"><span data-stu-id="d98e2-150">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="d98e2-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="d98e2-151">Response</span></span>
<span data-ttu-id="d98e2-152">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d98e2-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d98e2-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d98e2-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d98e2-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d98e2-154">Request</span></span>
<span data-ttu-id="d98e2-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d98e2-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 665

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d98e2-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="d98e2-156">Response</span></span>
<span data-ttu-id="d98e2-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d98e2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "16e76336-6336-16e7-3663-e7163663e716",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```




