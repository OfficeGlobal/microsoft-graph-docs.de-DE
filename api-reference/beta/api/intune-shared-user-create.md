---
title: Benutzer erstellen
description: Dient zum Erstellen eines neuen Benutzerobjekts.
author: tfitzmac
ms.openlocfilehash: dddfa5e6788aa56c1a983a889f692fc7cbdc4d94
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307672"
---
# <a name="create-user"></a><span data-ttu-id="8aea5-103">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="8aea5-103">Create user</span></span>

> <span data-ttu-id="8aea5-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8aea5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8aea5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8aea5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8aea5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8aea5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8aea5-107">Dient zum Erstellen eines neuen [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8aea5-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8aea5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8aea5-108">Prerequisites</span></span>

<span data-ttu-id="8aea5-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="8aea5-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8aea5-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aea5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="8aea5-111">Die spezifische erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="8aea5-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="8aea5-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8aea5-112">Permission type</span></span>|<span data-ttu-id="8aea5-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8aea5-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aea5-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8aea5-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8aea5-115">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="8aea5-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8aea5-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aea5-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="8aea5-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8aea5-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8aea5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aea5-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="8aea5-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="8aea5-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="8aea5-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aea5-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="8aea5-121">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="8aea5-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8aea5-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aea5-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8aea5-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8aea5-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aea5-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8aea5-124">Not supported.</span></span>|
|<span data-ttu-id="8aea5-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8aea5-125">Application</span></span>|<span data-ttu-id="8aea5-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8aea5-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aea5-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8aea5-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="8aea5-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8aea5-128">Request headers</span></span>

|<span data-ttu-id="8aea5-129">Header</span><span class="sxs-lookup"><span data-stu-id="8aea5-129">Header</span></span>|<span data-ttu-id="8aea5-130">Wert</span><span class="sxs-lookup"><span data-stu-id="8aea5-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8aea5-131">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8aea5-131">Authorization</span></span>|<span data-ttu-id="8aea5-132">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8aea5-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8aea5-133">Accept</span><span class="sxs-lookup"><span data-stu-id="8aea5-133">Accept</span></span>|<span data-ttu-id="8aea5-134">application/json</span><span class="sxs-lookup"><span data-stu-id="8aea5-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aea5-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8aea5-135">Request body</span></span>

<span data-ttu-id="8aea5-136">Geben Sie im Anforderungstext eine JSON-Darstellung des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="8aea5-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="8aea5-137">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8aea5-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="8aea5-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8aea5-138">Property</span></span>|<span data-ttu-id="8aea5-139">Typ</span><span class="sxs-lookup"><span data-stu-id="8aea5-139">Type</span></span>|<span data-ttu-id="8aea5-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8aea5-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aea5-141">id</span><span class="sxs-lookup"><span data-stu-id="8aea5-141">id</span></span>|<span data-ttu-id="8aea5-142">String</span><span class="sxs-lookup"><span data-stu-id="8aea5-142">String</span></span>|<span data-ttu-id="8aea5-143">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="8aea5-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="8aea5-144">**Klicken Sie auf mittels Fingereingabe**</span><span class="sxs-lookup"><span data-stu-id="8aea5-144">**On-boarding**</span></span>||
|<span data-ttu-id="8aea5-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="8aea5-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="8aea5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8aea5-146">Int32</span></span>|<span data-ttu-id="8aea5-147">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="8aea5-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="8aea5-148">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="8aea5-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="8aea5-149">Anforderung Body-Eigenschaft Unterstützung variiert je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="8aea5-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="8aea5-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="8aea5-150">Response</span></span>

<span data-ttu-id="8aea5-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/intune-shared-user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8aea5-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8aea5-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8aea5-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="8aea5-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8aea5-153">Request</span></span>

<span data-ttu-id="8aea5-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8aea5-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="8aea5-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="8aea5-155">Response</span></span>

<span data-ttu-id="8aea5-156">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8aea5-156">Here is an example of the response.</span></span> <span data-ttu-id="8aea5-157">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="8aea5-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8aea5-158">Eigenschaften von einer tatsächlichen Aufruf zurückgegeben variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="8aea5-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



