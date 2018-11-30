---
title: onPremisesConditionalAccessSettings aktualisieren
description: Aktualisieren der Eigenschaften eines onPremisesConditionalAccessSettings-Objekts.
ms.openlocfilehash: 31679b6c698903083675e926fa77e0c56be49a38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066202"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="e75e0-103">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e75e0-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="e75e0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e75e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e75e0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e75e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e75e0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e75e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e75e0-107">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e75e0-107">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e75e0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e75e0-108">Prerequisites</span></span>
<span data-ttu-id="e75e0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e75e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e75e0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e75e0-111">Permission type</span></span>|<span data-ttu-id="e75e0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e75e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e75e0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e75e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e75e0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e75e0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e75e0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e75e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e75e0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e75e0-116">Not supported.</span></span>|
|<span data-ttu-id="e75e0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e75e0-117">Application</span></span>|<span data-ttu-id="e75e0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e75e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e75e0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e75e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="e75e0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e75e0-120">Request headers</span></span>
|<span data-ttu-id="e75e0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e75e0-121">Header</span></span>|<span data-ttu-id="e75e0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e75e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e75e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e75e0-123">Authorization</span></span>|<span data-ttu-id="e75e0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e75e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e75e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e75e0-125">Accept</span></span>|<span data-ttu-id="e75e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e75e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e75e0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e75e0-127">Request body</span></span>
<span data-ttu-id="e75e0-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e75e0-128">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="e75e0-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e75e0-129">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="e75e0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e75e0-130">Property</span></span>|<span data-ttu-id="e75e0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e75e0-131">Type</span></span>|<span data-ttu-id="e75e0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e75e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e75e0-133">id</span><span class="sxs-lookup"><span data-stu-id="e75e0-133">id</span></span>|<span data-ttu-id="e75e0-134">String</span><span class="sxs-lookup"><span data-stu-id="e75e0-134">String</span></span>|<span data-ttu-id="e75e0-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e75e0-135">Not yet documented</span></span>|
|<span data-ttu-id="e75e0-136">enabled</span><span class="sxs-lookup"><span data-stu-id="e75e0-136">enabled</span></span>|<span data-ttu-id="e75e0-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e75e0-137">Boolean</span></span>|<span data-ttu-id="e75e0-138">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="e75e0-138">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="e75e0-139">includedGroups</span><span class="sxs-lookup"><span data-stu-id="e75e0-139">includedGroups</span></span>|<span data-ttu-id="e75e0-140">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e75e0-140">Guid collection</span></span>|<span data-ttu-id="e75e0-141">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="e75e0-141">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="e75e0-142">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="e75e0-142">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="e75e0-143">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="e75e0-143">excludedGroups</span></span>|<span data-ttu-id="e75e0-144">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e75e0-144">Guid collection</span></span>|<span data-ttu-id="e75e0-145">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="e75e0-145">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="e75e0-146">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="e75e0-146">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="e75e0-147">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="e75e0-147">overrideDefaultRule</span></span>|<span data-ttu-id="e75e0-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e75e0-148">Boolean</span></span>|<span data-ttu-id="e75e0-149">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="e75e0-149">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="e75e0-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="e75e0-150">Response</span></span>
<span data-ttu-id="e75e0-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e75e0-151">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e75e0-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e75e0-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="e75e0-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e75e0-153">Request</span></span>
<span data-ttu-id="e75e0-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e75e0-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 201

{
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="e75e0-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="e75e0-155">Response</span></span>
<span data-ttu-id="e75e0-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e75e0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```





