---
title: Azure AD-Synchronisierung API (Übersicht)
description: ') können Sie die Erstellung automatisieren Wartung und Entfernen von Identitäten in cloud (Software als Dienst oder SaaS) Anwendungen wie Ablage, Vertriebs, ServiceNow und vieles mehr. Die Synchronisierung-APIs können in Microsoft Graph Sie programmgesteuert verwalten Identität Synchronisierung einschließlich:'
localization_priority: Normal
ms.openlocfilehash: aada94f39c67fb1174924d49c6e57650f4961cc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884686"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="56281-104">Azure AD-Synchronisierung API (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="56281-104">Azure AD synchronization API overview</span></span>

> <span data-ttu-id="56281-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56281-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56281-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56281-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56281-107">Azure Active Directory (AD Azure) Identität Synchronisierung (auch als "Bereitstellung" bezeichnet) können Sie die Erstellung, Wartung und Entfernen von Identitäten in der Cloud (Software als Dienst oder SaaS) automatisieren Applications wie Ablage, Vertriebs, ServiceNow, und vieles mehr.</span><span class="sxs-lookup"><span data-stu-id="56281-107">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="56281-108">Die Synchronisierung-APIs können in Microsoft Graph Sie programmgesteuert verwalten Identität Synchronisierung einschließlich:</span><span class="sxs-lookup"><span data-stu-id="56281-108">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="56281-109">Erstellen Sie, starten Sie und beenden Sie der Aufträge für die Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="56281-109">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="56281-110">Vornehmen von Änderungen an der Synchronisierungsschema für Aufträge</span><span class="sxs-lookup"><span data-stu-id="56281-110">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="56281-111">Überprüfen Sie den aktuellen Synchronisierungsstatus</span><span class="sxs-lookup"><span data-stu-id="56281-111">Verify the current synchronization status</span></span> 

<span data-ttu-id="56281-112">Weitere Informationen zur Synchronisierung in Azure Active Directory finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="56281-112">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="56281-113">Automatisieren der Benutzer bereitstellen und entziehen für SaaS Clientanwendungen mit Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="56281-113">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="56281-114">Verwalten von Benutzerkonto für Enterprise-apps im Azure-Portal-Bereitstellung</span><span class="sxs-lookup"><span data-stu-id="56281-114">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="56281-115">Sie können auch die API im [Graph-Explorer](https://developer.microsoft.com/graph/graph-explorer) in einer Beispiel-Mandanten oder Ihre eigene Mandanten versuchen.</span><span class="sxs-lookup"><span data-stu-id="56281-115">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="56281-116">Synchronisierungsauftrag</span><span class="sxs-lookup"><span data-stu-id="56281-116">Synchronization job</span></span>

<span data-ttu-id="56281-117">Aufträge für die Synchronisierung ausführen Synchronisierung von in regelmäßigen Abständen im Hintergrund ausgeführt, abrufen, damit die Änderungen in ein Verzeichnis und pushen von in ein anderes Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="56281-117">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="56281-118">Der Synchronisierungsauftrag ist immer spezifisch für eine bestimmte Instanz einer Anwendung in Ihrem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="56281-118">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="56281-119">Im Rahmen der Synchronisierung Einrichtung müssen Sie die Autorisierung zum Lesen und Schreiben von Objekten in Ihrem Zielverzeichnis übergeben, und passen den Auftrag Synchronisierungsschema.</span><span class="sxs-lookup"><span data-stu-id="56281-119">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="56281-120">Weitere Informationen finden Sie unter [Synchronisierungsauftrag](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="56281-120">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="56281-121">Synchronisierungsschema</span><span class="sxs-lookup"><span data-stu-id="56281-121">Synchronization schema</span></span>

<span data-ttu-id="56281-122">Das Synchronisierungsschema definiert, welche Objekte werden synchronisiert, und wie diese synchronisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="56281-122">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="56281-123">Das Synchronisierungsschema enthält die meisten der Setupinformationen für einen bestimmten Synchronisierungsauftrag.</span><span class="sxs-lookup"><span data-stu-id="56281-123">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="56281-124">Sie werden in der Regel anpassen einiger [Attribut Zuordnungen](synchronization-attributemapping.md)oder Hinzufügen eines [Gültigkeitsbereichs Filter](synchronization-filter.md) , um nur die Objekte zu synchronisieren, die eine bestimmte Bedingung erfüllen.</span><span class="sxs-lookup"><span data-stu-id="56281-124">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="56281-125">Das Synchronisierungsschema umfasst die folgenden Komponenten:</span><span class="sxs-lookup"><span data-stu-id="56281-125">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="56281-126">Directory-Definitionen</span><span class="sxs-lookup"><span data-stu-id="56281-126">Directory definitions</span></span>
- <span data-ttu-id="56281-127">Synchronisierungsregeln</span><span class="sxs-lookup"><span data-stu-id="56281-127">Synchronization rules</span></span>
- <span data-ttu-id="56281-128">Objekt-Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="56281-128">Object mappings</span></span>

<span data-ttu-id="56281-129">Weitere Informationen finden Sie unter [Synchronisierungsschema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="56281-129">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="56281-130">Synchronisierung-Vorlage</span><span class="sxs-lookup"><span data-stu-id="56281-130">Synchronization template</span></span>

<span data-ttu-id="56281-131">Die Synchronisierung Vorlage enthält vorkonfigurierte synchronisierungseinstellungen für eine bestimmte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="56281-131">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="56281-132">Diese Einstellungen (vor allem [Synchronisierungsschema](synchronization-synchronizationschema.md)) werden standardmäßig für alle [Synchronisierungsauftrag](synchronization-synchronizationjob.md) verwendet werden, die auf der Vorlage basiert.</span><span class="sxs-lookup"><span data-stu-id="56281-132">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="56281-133">Vorlagen, die vom Anwendungsentwickler festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="56281-133">Templates are specified by the application developer.</span></span>

<span data-ttu-id="56281-134">Weitere Informationen finden Sie unter [Synchronisierung Vorlage](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="56281-134">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="56281-135">Arbeiten mit der API-Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="56281-135">Working with the synchronization API</span></span>

<span data-ttu-id="56281-136">Arbeiten mit Synchronisierung umfasst API in erster Linie den Zugriff auf die [SynchronizationJob](synchronization-synchronizationjob.md) und [SynchronizationSchema](synchronization-synchronizationschema.md) Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="56281-136">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="56281-137">Damit die Ressource [SynchronizationJob](synchronization-synchronizationjob.md) ermittelt wird, müssen Sie die ID des Service principal-Objekts wissen, zu der der Synchronisierungsauftrag gehört.</span><span class="sxs-lookup"><span data-stu-id="56281-137">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="56281-138">Die folgenden Beispiele zeigen, wie die Ressourcen **SynchronizationJob** und **SynchronizationSchema** entwickelt.</span><span class="sxs-lookup"><span data-stu-id="56281-138">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="56281-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="56281-139">Authorization</span></span>

<span data-ttu-id="56281-140">Die Azure AD-Synchronisierung API verwendet OAuth 2.0 für die Autorisierung.</span><span class="sxs-lookup"><span data-stu-id="56281-140">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="56281-141">Vor der Durchführung von alle Anforderungen an die API, müssen Sie ein Zugriffstoken abzurufen.</span><span class="sxs-lookup"><span data-stu-id="56281-141">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="56281-142">Weitere Informationen finden Sie unter [Get Access tokens Microsoft Graph aufrufen](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="56281-142">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="56281-143">Um den Zugriff auf Ressourcen Synchronisierung benötigt Ihre Anwendung Directory.ReadWrite.All Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="56281-143">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="56281-144">Weitere Informationen finden Sie unter [Directory-Berechtigungen](/graph/permissions-reference#directory-permissions).</span><span class="sxs-lookup"><span data-stu-id="56281-144">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="56281-145">Hier finden Sie das principal-Objekt nach Anzeigename</span><span class="sxs-lookup"><span data-stu-id="56281-145">Find the service principal object by display name</span></span>

<span data-ttu-id="56281-146">Im folgenden Beispiel wird gezeigt, wie Service principal-Objekt nach dem Anzeigenamen zu suchen.</span><span class="sxs-lookup"><span data-stu-id="56281-146">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="56281-147">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="56281-147">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="56281-148">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="56281-148">**Response**</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="56281-149">Hier finden Sie das principal-Objekt von app-ID</span><span class="sxs-lookup"><span data-stu-id="56281-149">Find the service principal object by app ID</span></span>

<span data-ttu-id="56281-150">Das folgende Beispiel zeigt, wie Sie finden das principal-Objekt nach app-ID.</span><span class="sxs-lookup"><span data-stu-id="56281-150">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="56281-151">**Anforderung** 
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="56281-151">**Request** 
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="56281-152">**Antwort**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="56281-152">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="56281-153">Liste der vorhandenen Aufträge für die Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="56281-153">List existing synchronization jobs</span></span>

<span data-ttu-id="56281-154">Das folgende Beispiel veranschaulicht das Auflisten der vorhandenen Aufträge für die Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="56281-154">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="56281-155">**Anforderung**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="56281-155">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="56281-156">**Antwort**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="56281-156">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a><span data-ttu-id="56281-157">Erste Synchronisierung Auftragsstatus</span><span class="sxs-lookup"><span data-stu-id="56281-157">Get synchronization job status</span></span>
<span data-ttu-id="56281-158">Im folgende Beispiel wird das Abrufen des Status eines Auftrags zur Synchronisierung veranschaulicht.</span><span class="sxs-lookup"><span data-stu-id="56281-158">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="56281-159">**Anforderung**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="56281-159">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="56281-160">**Antwort**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="56281-160">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a><span data-ttu-id="56281-161">Erste Synchronisierungsschema</span><span class="sxs-lookup"><span data-stu-id="56281-161">Get synchronization schema</span></span>
<span data-ttu-id="56281-162">Im folgende Beispiel wird das Abrufen des Synchronisierungsschemas veranschaulicht.</span><span class="sxs-lookup"><span data-stu-id="56281-162">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="56281-163">**Anforderung**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="56281-163">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="56281-164">**Antwort**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="56281-164">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="56281-165">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="56281-165">See also</span></span>

* [<span data-ttu-id="56281-166">Konfigurieren der Synchronisierung mit Verzeichnis Extension-Attribute</span><span class="sxs-lookup"><span data-stu-id="56281-166">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="56281-167">Konfigurieren der Synchronisierung mit benutzerdefinierten Ziel-Attribute</span><span class="sxs-lookup"><span data-stu-id="56281-167">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



