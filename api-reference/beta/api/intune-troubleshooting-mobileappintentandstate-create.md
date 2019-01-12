---
title: Erstellen von mobileAppIntentAndState
description: Erstellen eines neuen MobileAppIntentAndState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 513c7ad7b6c3defdea325a1cb80161d5d554fb12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983989"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="ca4a9-103">Erstellen von mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="ca4a9-103">Create mobileAppIntentAndState</span></span>

> <span data-ttu-id="ca4a9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca4a9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca4a9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca4a9-107">Erstellen eines neuen [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-107">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca4a9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ca4a9-108">Prerequisites</span></span>
<span data-ttu-id="ca4a9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca4a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca4a9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ca4a9-111">Permission type</span></span>|<span data-ttu-id="ca4a9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ca4a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca4a9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ca4a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca4a9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca4a9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ca4a9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ca4a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca4a9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca4a9-116">Not supported.</span></span>|
|<span data-ttu-id="ca4a9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ca4a9-117">Application</span></span>|<span data-ttu-id="ca4a9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca4a9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca4a9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca4a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="ca4a9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ca4a9-120">Request headers</span></span>
|<span data-ttu-id="ca4a9-121">Header</span><span class="sxs-lookup"><span data-stu-id="ca4a9-121">Header</span></span>|<span data-ttu-id="ca4a9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ca4a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca4a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca4a9-123">Authorization</span></span>|<span data-ttu-id="ca4a9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ca4a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca4a9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ca4a9-125">Accept</span></span>|<span data-ttu-id="ca4a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca4a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca4a9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ca4a9-127">Request body</span></span>
<span data-ttu-id="ca4a9-128">Geben Sie im Textkörper Anforderung für das Objekt MobileAppIntentAndState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-128">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="ca4a9-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MobileAppIntentAndState erstellen.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-129">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="ca4a9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ca4a9-130">Property</span></span>|<span data-ttu-id="ca4a9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ca4a9-131">Type</span></span>|<span data-ttu-id="ca4a9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca4a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca4a9-133">id</span><span class="sxs-lookup"><span data-stu-id="ca4a9-133">id</span></span>|<span data-ttu-id="ca4a9-134">String</span><span class="sxs-lookup"><span data-stu-id="ca4a9-134">String</span></span>|<span data-ttu-id="ca4a9-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="ca4a9-135">UUID for the object</span></span>|
|<span data-ttu-id="ca4a9-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ca4a9-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="ca4a9-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca4a9-137">String</span></span>|<span data-ttu-id="ca4a9-138">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="ca4a9-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="ca4a9-139">userId</span><span class="sxs-lookup"><span data-stu-id="ca4a9-139">userId</span></span>|<span data-ttu-id="ca4a9-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca4a9-140">String</span></span>|<span data-ttu-id="ca4a9-141">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="ca4a9-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="ca4a9-142">mobileAppList</span></span>|<span data-ttu-id="ca4a9-143">[MobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ca4a9-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="ca4a9-144">Die Liste der Nutzlast Intents und Status für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="ca4a9-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca4a9-145">Response</span></span>
<span data-ttu-id="ca4a9-146">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-146">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca4a9-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ca4a9-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca4a9-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca4a9-148">Request</span></span>
<span data-ttu-id="ca4a9-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
Content-type: application/json
Content-length: 831

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ca4a9-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca4a9-150">Response</span></span>
<span data-ttu-id="ca4a9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca4a9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 880

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "45a775d6-75d6-45a7-d675-a745d675a745",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```





