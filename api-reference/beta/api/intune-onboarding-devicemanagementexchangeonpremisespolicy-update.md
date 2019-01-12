---
title: DeviceManagementExchangeOnPremisesPolicy aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementExchangeOnPremisesPolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3698a258f6d0dd5c84f430c8690a7f58ffd88b0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974665"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="355cf-103">DeviceManagementExchangeOnPremisesPolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="355cf-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="355cf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="355cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="355cf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="355cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="355cf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="355cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="355cf-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="355cf-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="355cf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="355cf-108">Prerequisites</span></span>
<span data-ttu-id="355cf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="355cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="355cf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="355cf-111">Permission type</span></span>|<span data-ttu-id="355cf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="355cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="355cf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="355cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="355cf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="355cf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="355cf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="355cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="355cf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="355cf-116">Not supported.</span></span>|
|<span data-ttu-id="355cf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="355cf-117">Application</span></span>|<span data-ttu-id="355cf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="355cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="355cf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="355cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="355cf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="355cf-120">Request headers</span></span>
|<span data-ttu-id="355cf-121">Header</span><span class="sxs-lookup"><span data-stu-id="355cf-121">Header</span></span>|<span data-ttu-id="355cf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="355cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="355cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="355cf-123">Authorization</span></span>|<span data-ttu-id="355cf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="355cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="355cf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="355cf-125">Accept</span></span>|<span data-ttu-id="355cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="355cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="355cf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="355cf-127">Request body</span></span>
<span data-ttu-id="355cf-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="355cf-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="355cf-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="355cf-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="355cf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="355cf-130">Property</span></span>|<span data-ttu-id="355cf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="355cf-131">Type</span></span>|<span data-ttu-id="355cf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="355cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="355cf-133">id</span><span class="sxs-lookup"><span data-stu-id="355cf-133">id</span></span>|<span data-ttu-id="355cf-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="355cf-134">String</span></span>|<span data-ttu-id="355cf-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="355cf-135">Not yet documented</span></span>|
|<span data-ttu-id="355cf-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="355cf-136">notificationContent</span></span>|<span data-ttu-id="355cf-137">Binär</span><span class="sxs-lookup"><span data-stu-id="355cf-137">Binary</span></span>|<span data-ttu-id="355cf-138">Der Text der Benachrichtigung, die Benutzern unter Quarantäne gestellte e-Mails durch diese Richtlinie gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="355cf-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="355cf-139">Hierbei handelt es sich um UTF8 codiert HTML-Byte-Array.</span><span class="sxs-lookup"><span data-stu-id="355cf-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="355cf-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="355cf-140">defaultAccessLevel</span></span>|[<span data-ttu-id="355cf-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="355cf-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="355cf-142">Access-Standardzustand in Exchange.</span><span class="sxs-lookup"><span data-stu-id="355cf-142">Default access state in Exchange.</span></span> <span data-ttu-id="355cf-143">Diese Regel gilt global für die gesamte Exchange-Organisation.</span><span class="sxs-lookup"><span data-stu-id="355cf-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="355cf-144">Mögliche Werte: sind `none`, `allow`, `block` und `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="355cf-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="355cf-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="355cf-145">accessRules</span></span>|<span data-ttu-id="355cf-146">[DeviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="355cf-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="355cf-147">Die Liste der Gerätezugriffs Regeln im Exchange.</span><span class="sxs-lookup"><span data-stu-id="355cf-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="355cf-148">Die Access-Regeln gelten global für die gesamte Exchange-Organisation</span><span class="sxs-lookup"><span data-stu-id="355cf-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="355cf-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="355cf-149">knownDeviceClasses</span></span>|<span data-ttu-id="355cf-150">[DeviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="355cf-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="355cf-151">Die Liste der Geräteklassen bekannt, dass Exchange</span><span class="sxs-lookup"><span data-stu-id="355cf-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="355cf-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="355cf-152">Response</span></span>
<span data-ttu-id="355cf-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="355cf-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="355cf-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="355cf-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="355cf-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="355cf-155">Request</span></span>
<span data-ttu-id="355cf-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="355cf-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 586

{
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

### <a name="response"></a><span data-ttu-id="355cf-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="355cf-157">Response</span></span>
<span data-ttu-id="355cf-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="355cf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





