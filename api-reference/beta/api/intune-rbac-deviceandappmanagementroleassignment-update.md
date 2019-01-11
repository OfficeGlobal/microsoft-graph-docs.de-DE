---
title: DeviceAndAppManagementRoleAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines deviceAndAppManagementRoleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3f669ac0c3758f2b96e4732fbbdd46966dd87b4c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838304"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="029f0-103">DeviceAndAppManagementRoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="029f0-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="029f0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="029f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="029f0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="029f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="029f0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="029f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="029f0-107">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="029f0-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="029f0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="029f0-108">Prerequisites</span></span>
<span data-ttu-id="029f0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="029f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="029f0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="029f0-111">Permission type</span></span>|<span data-ttu-id="029f0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="029f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="029f0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="029f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="029f0-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="029f0-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="029f0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="029f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="029f0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="029f0-116">Not supported.</span></span>|
|<span data-ttu-id="029f0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="029f0-117">Application</span></span>|<span data-ttu-id="029f0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="029f0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="029f0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="029f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="029f0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="029f0-120">Request headers</span></span>
|<span data-ttu-id="029f0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="029f0-121">Header</span></span>|<span data-ttu-id="029f0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="029f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="029f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="029f0-123">Authorization</span></span>|<span data-ttu-id="029f0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="029f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="029f0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="029f0-125">Accept</span></span>|<span data-ttu-id="029f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="029f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="029f0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="029f0-127">Request body</span></span>
<span data-ttu-id="029f0-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="029f0-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="029f0-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="029f0-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="029f0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="029f0-130">Property</span></span>|<span data-ttu-id="029f0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="029f0-131">Type</span></span>|<span data-ttu-id="029f0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="029f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="029f0-133">id</span><span class="sxs-lookup"><span data-stu-id="029f0-133">id</span></span>|<span data-ttu-id="029f0-134">String</span><span class="sxs-lookup"><span data-stu-id="029f0-134">String</span></span>|<span data-ttu-id="029f0-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="029f0-135">Key of the entity.</span></span> <span data-ttu-id="029f0-136">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="029f0-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="029f0-137">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="029f0-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="029f0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="029f0-138">displayName</span></span>|<span data-ttu-id="029f0-139">String</span><span class="sxs-lookup"><span data-stu-id="029f0-139">String</span></span>|<span data-ttu-id="029f0-140">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="029f0-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="029f0-141">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="029f0-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="029f0-142">description</span><span class="sxs-lookup"><span data-stu-id="029f0-142">description</span></span>|<span data-ttu-id="029f0-143">String</span><span class="sxs-lookup"><span data-stu-id="029f0-143">String</span></span>|<span data-ttu-id="029f0-144">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="029f0-144">Description of the Role Assignment.</span></span> <span data-ttu-id="029f0-145">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="029f0-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="029f0-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="029f0-146">scopeMembers</span></span>|<span data-ttu-id="029f0-147">String collection</span><span class="sxs-lookup"><span data-stu-id="029f0-147">String collection</span></span>|<span data-ttu-id="029f0-148">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="029f0-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="029f0-149">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="029f0-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="029f0-150">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="029f0-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="029f0-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="029f0-151">scopeType</span></span>|[<span data-ttu-id="029f0-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="029f0-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="029f0-153">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="029f0-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="029f0-154">Standardtyp 'ResourceScope' ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="029f0-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="029f0-155">Für 'AllDevices', 'AllLicensedUsers' und 'AllDevicesAndLicensedUsers' sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="029f0-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="029f0-156">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="029f0-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="029f0-157">Mögliche Werte: sind `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="029f0-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="029f0-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="029f0-158">resourceScopes</span></span>|<span data-ttu-id="029f0-159">String collection</span><span class="sxs-lookup"><span data-stu-id="029f0-159">String collection</span></span>|<span data-ttu-id="029f0-160">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="029f0-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="029f0-161">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="029f0-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="029f0-162">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="029f0-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="029f0-163">Elemente</span><span class="sxs-lookup"><span data-stu-id="029f0-163">members</span></span>|<span data-ttu-id="029f0-164">String collection</span><span class="sxs-lookup"><span data-stu-id="029f0-164">String collection</span></span>|<span data-ttu-id="029f0-165">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="029f0-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="029f0-166">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="029f0-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="029f0-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="029f0-167">Response</span></span>
<span data-ttu-id="029f0-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="029f0-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="029f0-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="029f0-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="029f0-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="029f0-170">Request</span></span>
<span data-ttu-id="029f0-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="029f0-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="029f0-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="029f0-172">Response</span></span>
<span data-ttu-id="029f0-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="029f0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





