# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="d18d1-101">Arbeiten mit Benutzern in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d18d1-101">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="d18d1-102">Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.</span><span class="sxs-lookup"><span data-stu-id="d18d1-102">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="d18d1-103">Sie können auf zwei Arten über Microsoft Graph auf [Benutzer](user.md) zugreifen:</span><span class="sxs-lookup"><span data-stu-id="d18d1-103">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="d18d1-104">Anhand der ID, `/users/{id | userPrincipalName}`</span><span class="sxs-lookup"><span data-stu-id="d18d1-104">By their ID, `/users/{id | userPrincipalName}`</span></span> 
- <span data-ttu-id="d18d1-105">Anhand des `/me`-Alias für den angemeldeten Benutzer, welcher `/users/{signed-in user's id}` entspricht</span><span class="sxs-lookup"><span data-stu-id="d18d1-105">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="d18d1-106">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d18d1-106">Authorization</span></span>

<span data-ttu-id="d18d1-107">Für den Zugriff auf Benutzervorgänge ist eine der folgenden [Berechtigungen](https://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes) erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d18d1-107">One of the following [permissions](https://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes) is required to access user operations.</span></span> <span data-ttu-id="d18d1-108">Die ersten drei Berechtigungen können einer App durch einen Benutzer gewährt werden.</span><span class="sxs-lookup"><span data-stu-id="d18d1-108">The first three permissions can be granted to an app by a user.</span></span> <span data-ttu-id="d18d1-109">Die übrigen können der App nur durch einen Administrator gewährt werden.</span><span class="sxs-lookup"><span data-stu-id="d18d1-109">The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="d18d1-110">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="d18d1-110">User.ReadBasic.All</span></span>
- <span data-ttu-id="d18d1-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="d18d1-111">User.Read</span></span>
- <span data-ttu-id="d18d1-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d18d1-112">User.ReadWrite</span></span>
- <span data-ttu-id="d18d1-113">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d18d1-113">User.Read.All</span></span>
- <span data-ttu-id="d18d1-114">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d18d1-114">User.ReadWrite.All</span></span>
- <span data-ttu-id="d18d1-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d18d1-115">Directory.Read.All</span></span>
- <span data-ttu-id="d18d1-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d18d1-116">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="d18d1-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d18d1-117">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="d18d1-118">Allgemeine Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d18d1-118">Common properties</span></span>

<span data-ttu-id="d18d1-119">Im Folgenden werden standardmäßige Eigenschaften dargestellt, die beim Abrufen eines Benutzers oder beim Auflisten von Benutzern zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="d18d1-119">The following represent the default set of properties that are returned when getting a user or listing users.  These are a subset of all available properties. To get more user properties, use the  query parameter.</span></span> <span data-ttu-id="d18d1-120">Diese stellen eine Teilmenge aller verfügbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="d18d1-120">These are a subset of all available properties.</span></span> <span data-ttu-id="d18d1-121">Verwenden Sie zum Abrufen weiterer Benutzereigenschaften den `$select`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="d18d1-121">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="d18d1-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d18d1-122">Property</span></span> |<span data-ttu-id="d18d1-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d18d1-123">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="d18d1-124">id</span><span class="sxs-lookup"><span data-stu-id="d18d1-124">id</span></span> | <span data-ttu-id="d18d1-125">Die eindeutige ID des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d18d1-125">The unique identifier for the user.</span></span>|
|<span data-ttu-id="d18d1-126">businessPhones</span><span class="sxs-lookup"><span data-stu-id="d18d1-126">businessPhones</span></span> | <span data-ttu-id="d18d1-127">Telefonnummern des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d18d1-127">The user's phone numbers.</span></span>|
|<span data-ttu-id="d18d1-128">displayName</span><span class="sxs-lookup"><span data-stu-id="d18d1-128">displayName</span></span> | <span data-ttu-id="d18d1-129">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d18d1-129">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="d18d1-130">givenName</span><span class="sxs-lookup"><span data-stu-id="d18d1-130">givenName</span></span>| <span data-ttu-id="d18d1-131">Der Vorname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d18d1-131">The first name of the user.</span></span> |
|<span data-ttu-id="d18d1-132">jobTitle</span><span class="sxs-lookup"><span data-stu-id="d18d1-132">jobTitle</span></span> | <span data-ttu-id="d18d1-133">Die Position des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d18d1-133">The user's job title.</span></span>|
|<span data-ttu-id="d18d1-134">mail</span><span class="sxs-lookup"><span data-stu-id="d18d1-134">mail</span></span>| <span data-ttu-id="d18d1-135">Die E-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d18d1-135">The user's email address.</span></span> |
|<span data-ttu-id="d18d1-136">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="d18d1-136">mobilePhone</span></span> | <span data-ttu-id="d18d1-137">Die Mobiltelefonnummern des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d18d1-137">The user's cellphone number.</span></span>|
|<span data-ttu-id="d18d1-138">officeLocation</span><span class="sxs-lookup"><span data-stu-id="d18d1-138">officeLocation</span></span> | <span data-ttu-id="d18d1-139">Der Bürostandort des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d18d1-139">The user's physical office location.</span></span>|
|<span data-ttu-id="d18d1-140">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="d18d1-140">preferredLanguage</span></span> | <span data-ttu-id="d18d1-141">Die vom Benutzer bevorzugte Sprache.</span><span class="sxs-lookup"><span data-stu-id="d18d1-141">The user's language of preference.</span></span>|
|<span data-ttu-id="d18d1-142">surname</span><span class="sxs-lookup"><span data-stu-id="d18d1-142">surname</span></span>| <span data-ttu-id="d18d1-143">Der Nachname des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d18d1-143">The last name of the user.</span></span> |
|<span data-ttu-id="d18d1-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d18d1-144">userPrincipalName</span></span>| <span data-ttu-id="d18d1-145">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="d18d1-145">The user's principal name.</span></span> |

<br/>

<span data-ttu-id="d18d1-146">Weitere Informationen und eine Liste aller Eigenschaften finden Sie unter [user](user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d18d1-146">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="d18d1-147">Allgemeine Vorgänge</span><span class="sxs-lookup"><span data-stu-id="d18d1-147">Common operations</span></span>

> <span data-ttu-id="d18d1-148">**Hinweis:** Einige dieser Vorgänge erfordern zusätzliche Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="d18d1-148">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="d18d1-149">Pfad</span><span class="sxs-lookup"><span data-stu-id="d18d1-149">Path</span></span>    | <span data-ttu-id="d18d1-150">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d18d1-150">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user_list.md) | <span data-ttu-id="d18d1-151">Listet die Benutzer in der Organisation auf.</span><span class="sxs-lookup"><span data-stu-id="d18d1-151">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user_get.md) | <span data-ttu-id="d18d1-152">Ruft einen bestimmten Benutzer anhand der ID ab.</span><span class="sxs-lookup"><span data-stu-id="d18d1-152">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto_get.md)| <span data-ttu-id="d18d1-153">Ruft das Profilfoto des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="d18d1-153">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user_list_manager.md) | <span data-ttu-id="d18d1-154">Ruft den Vorgesetzten des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="d18d1-154">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user_list_messages.md)| <span data-ttu-id="d18d1-155">Listet die E-Mails des Benutzers im primären Posteingang auf.</span><span class="sxs-lookup"><span data-stu-id="d18d1-155">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user_list_events.md) | <span data-ttu-id="d18d1-156">Listet bevorstehende Ereignisse des Benutzers im Kalender auf.</span><span class="sxs-lookup"><span data-stu-id="d18d1-156">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive_get.md)| <span data-ttu-id="d18d1-157">Ruft den OneDrive-Dateispeicher des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="d18d1-157">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user_list_memberof.md)| <span data-ttu-id="d18d1-158">Listet die Gruppen auf, deren Mitglied der Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="d18d1-158">Lists the groups that the user is a member of.</span></span> |
