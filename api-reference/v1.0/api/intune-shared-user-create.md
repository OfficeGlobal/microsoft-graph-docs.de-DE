---
title: Benutzer erstellen
description: Dient zum Erstellen eines neuen Benutzerobjekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1b1789cbf0743384780147ce8c50f5472f9f2d64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981504"
---
# <a name="create-user"></a><span data-ttu-id="70ce6-103">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="70ce6-103">Create user</span></span>

> <span data-ttu-id="70ce6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="70ce6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70ce6-105">Dient zum Erstellen eines neuen [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="70ce6-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70ce6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="70ce6-106">Prerequisites</span></span>
<span data-ttu-id="70ce6-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="70ce6-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="70ce6-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70ce6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="70ce6-109">Die spezifische erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="70ce6-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="70ce6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70ce6-110">Permission type</span></span>|<span data-ttu-id="70ce6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70ce6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70ce6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70ce6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="70ce6-113">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="70ce6-113">_varies by context_</span></span> |
| <span data-ttu-id="70ce6-114">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="70ce6-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="70ce6-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70ce6-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="70ce6-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="70ce6-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="70ce6-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70ce6-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="70ce6-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="70ce6-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="70ce6-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70ce6-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="70ce6-120">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="70ce6-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="70ce6-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70ce6-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="70ce6-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70ce6-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70ce6-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70ce6-123">Not supported.</span></span>|
|<span data-ttu-id="70ce6-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70ce6-124">Application</span></span>|<span data-ttu-id="70ce6-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70ce6-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70ce6-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70ce6-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="70ce6-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70ce6-127">Request headers</span></span>
|<span data-ttu-id="70ce6-128">Header</span><span class="sxs-lookup"><span data-stu-id="70ce6-128">Header</span></span>|<span data-ttu-id="70ce6-129">Wert</span><span class="sxs-lookup"><span data-stu-id="70ce6-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70ce6-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="70ce6-130">Authorization</span></span>|<span data-ttu-id="70ce6-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="70ce6-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70ce6-132">Annehmen</span><span class="sxs-lookup"><span data-stu-id="70ce6-132">Accept</span></span>|<span data-ttu-id="70ce6-133">application/json</span><span class="sxs-lookup"><span data-stu-id="70ce6-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70ce6-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70ce6-134">Request body</span></span>
<span data-ttu-id="70ce6-135">Geben Sie im Anforderungstext eine JSON-Darstellung des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="70ce6-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="70ce6-136">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="70ce6-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="70ce6-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70ce6-137">Property</span></span>|<span data-ttu-id="70ce6-138">Typ</span><span class="sxs-lookup"><span data-stu-id="70ce6-138">Type</span></span>|<span data-ttu-id="70ce6-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70ce6-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70ce6-140">id</span><span class="sxs-lookup"><span data-stu-id="70ce6-140">id</span></span>|<span data-ttu-id="70ce6-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70ce6-141">String</span></span>|<span data-ttu-id="70ce6-142">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="70ce6-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="70ce6-143">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="70ce6-143">**Onboarding**</span></span>|
|<span data-ttu-id="70ce6-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="70ce6-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="70ce6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="70ce6-145">Int32</span></span>|<span data-ttu-id="70ce6-146">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="70ce6-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="70ce6-147">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="70ce6-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="70ce6-148">Anforderung Body-Eigenschaft Unterstützung variiert je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="70ce6-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="70ce6-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="70ce6-149">Response</span></span>
<span data-ttu-id="70ce6-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/intune-shared-user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70ce6-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70ce6-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70ce6-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="70ce6-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70ce6-152">Request</span></span>
<span data-ttu-id="70ce6-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70ce6-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="70ce6-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="70ce6-154">Response</span></span>
<span data-ttu-id="70ce6-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70ce6-155">Here is an example of the response.</span></span> <span data-ttu-id="70ce6-156">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="70ce6-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="70ce6-157">Eigenschaften von einer tatsächlichen Aufruf zurückgegeben variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="70ce6-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



