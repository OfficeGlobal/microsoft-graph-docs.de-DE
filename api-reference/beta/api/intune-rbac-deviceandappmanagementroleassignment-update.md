---
title: DeviceAndAppManagementRoleAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines deviceAndAppManagementRoleAssignment-Objekts.
ms.openlocfilehash: 4844d13c21e3371385531d43c1160cf34d7a1a50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060771"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="0bd2c-103">DeviceAndAppManagementRoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0bd2c-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="0bd2c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bd2c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bd2c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bd2c-107">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bd2c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0bd2c-108">Prerequisites</span></span>
<span data-ttu-id="0bd2c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bd2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bd2c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0bd2c-111">Permission type</span></span>|<span data-ttu-id="0bd2c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0bd2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bd2c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0bd2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bd2c-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bd2c-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0bd2c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0bd2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bd2c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bd2c-116">Not supported.</span></span>|
|<span data-ttu-id="0bd2c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0bd2c-117">Application</span></span>|<span data-ttu-id="0bd2c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bd2c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bd2c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bd2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0bd2c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0bd2c-120">Request headers</span></span>
|<span data-ttu-id="0bd2c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0bd2c-121">Header</span></span>|<span data-ttu-id="0bd2c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0bd2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bd2c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bd2c-123">Authorization</span></span>|<span data-ttu-id="0bd2c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0bd2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bd2c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0bd2c-125">Accept</span></span>|<span data-ttu-id="0bd2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bd2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bd2c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0bd2c-127">Request body</span></span>
<span data-ttu-id="0bd2c-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="0bd2c-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="0bd2c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0bd2c-130">Property</span></span>|<span data-ttu-id="0bd2c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0bd2c-131">Type</span></span>|<span data-ttu-id="0bd2c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bd2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bd2c-133">id</span><span class="sxs-lookup"><span data-stu-id="0bd2c-133">id</span></span>|<span data-ttu-id="0bd2c-134">String</span><span class="sxs-lookup"><span data-stu-id="0bd2c-134">String</span></span>|<span data-ttu-id="0bd2c-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0bd2c-135">Key of the entity.</span></span> <span data-ttu-id="0bd2c-136">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="0bd2c-137">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0bd2c-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0bd2c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0bd2c-138">displayName</span></span>|<span data-ttu-id="0bd2c-139">String</span><span class="sxs-lookup"><span data-stu-id="0bd2c-139">String</span></span>|<span data-ttu-id="0bd2c-140">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="0bd2c-141">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0bd2c-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0bd2c-142">description</span><span class="sxs-lookup"><span data-stu-id="0bd2c-142">description</span></span>|<span data-ttu-id="0bd2c-143">String</span><span class="sxs-lookup"><span data-stu-id="0bd2c-143">String</span></span>|<span data-ttu-id="0bd2c-144">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-144">Description of the Role Assignment.</span></span> <span data-ttu-id="0bd2c-145">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0bd2c-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0bd2c-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="0bd2c-146">scopeMembers</span></span>|<span data-ttu-id="0bd2c-147">String collection</span><span class="sxs-lookup"><span data-stu-id="0bd2c-147">String collection</span></span>|<span data-ttu-id="0bd2c-148">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0bd2c-149">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="0bd2c-150">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0bd2c-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0bd2c-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="0bd2c-151">scopeType</span></span>|[<span data-ttu-id="0bd2c-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="0bd2c-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="0bd2c-153">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="0bd2c-154">Standardtyp 'ResourceScope' ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="0bd2c-155">Für 'AllDevices', 'AllLicensedUsers' und 'AllDevicesAndLicensedUsers' sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="0bd2c-156">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0bd2c-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="0bd2c-157">Mögliche Werte: sind `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="0bd2c-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="0bd2c-158">resourceScopes</span></span>|<span data-ttu-id="0bd2c-159">String collection</span><span class="sxs-lookup"><span data-stu-id="0bd2c-159">String collection</span></span>|<span data-ttu-id="0bd2c-160">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0bd2c-161">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="0bd2c-162">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0bd2c-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0bd2c-163">Elemente</span><span class="sxs-lookup"><span data-stu-id="0bd2c-163">members</span></span>|<span data-ttu-id="0bd2c-164">String collection</span><span class="sxs-lookup"><span data-stu-id="0bd2c-164">String collection</span></span>|<span data-ttu-id="0bd2c-165">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="0bd2c-166">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="0bd2c-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bd2c-167">Response</span></span>
<span data-ttu-id="0bd2c-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bd2c-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0bd2c-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bd2c-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bd2c-170">Request</span></span>
<span data-ttu-id="0bd2c-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 267

{
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0bd2c-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bd2c-172">Response</span></span>
<span data-ttu-id="0bd2c-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bd2c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```





