>Question Bank for MAD - First Internals
# 1.Android Development Architecture

Android provides a rich development architecture. You don’t need to know much about the components of this architecture,
but it is useful to know what is available in the system for your app to use. The following diagram shows the major components of the Android stack — the operating system and development architecture.

<img src = "archi.png">
<br><br>

1. Apps: Your apps live at this level, along with core system apps for email, SMS messaging, calendars, Internet browsing, or contacts.
2. Java API Framework: All features of Android are available to developers through application programming interfaces (APIs) written in the Java language. You don't need to know the details of all of the APIs to learn how to develop
Android	apps,	but	you	can	learn	more	about	the	following	APIs,	which	are	useful	for	creating	apps:
* View	System	used	to	build	an	app's	UI,	including	lists,	buttons,	and	menus.
* Resource	Manager	used	to	access	to	non-code	resources	such	as	localized	strings,	graphics,	and	layout	files.
* Notification	Manager	used	to	display	custom	alerts	in	the	status	bar.
* Activity	Manager	that	manages	the	lifecycle	of	apps.
* Content	Providers	that	enable	apps	to	access	data	from	other	apps.
* All	framework	APIs	that	Android	system	apps	use.
3.	Libraries	and	Android	Runtime:	Each	app	runs	in	its	own	process	and	with	its	own	instance	of	the	Android	Runtime,
which	enables	multiple	virtual	machines	on	low-memory	devices.	Android	also	includes	a	set	of	core	runtime	libraries
that	provide	most	of	the	functionality	of	the	Java	programming	language,	including	some	Java	8	language	features	that
the	Java	API	framework	uses.	Many	core	Android	system	components	and	services	are	built	from	native	code	that
require	native	libraries	written	in	C	and	C++.	These	native	libraries	are	available	to	apps	through	the	Java	API
framework.
4.	Hardware	Abstraction	Layer	(HAL):	This	layer	provides	standard	interfaces	that	expose	device	hardware	capabilities
to	the	higher-level	Java	API	framework.	The	HAL	consists	of	multiple	library	modules,	each	of	which	implements	an
interface	for	a	specific	type	of	hardware	component,	such	as	the	camera	or	bluetooth	module.
5.	Linux	Kernel:	The	foundation	of	the	Android	platform	is	the	Linux	kernel.	The	above	layers	rely	on	the	Linux	kernel	for
underlying	functionalities	such	as	threading	and	low-level	memory	management.	Using	a	Linux	kernel	enables	Android
to	take	advantage	of	key	security	features	and	allows	device	manufacturers	to	develop	hardware	drivers	for	a	well
known	kernel.

# 2.Challenges of Android App Development

 While	the	Android	platform	provide	rich	functionality	for	app	development,	there	are	still	a	number	of	challenges	you	need
 to	address,	such	as:
 * Building	for	a	multi-screen	world
 * Getting	performance	right
 * Keeping	your	code	and	your	users	secure
 * Remaining	compatible	with	older	platform	versions
 * Understanding	the	market	and	the	user.
 ### Building	for	a	multi-screen	world
 Android	runs	on	billions	of	handheld	devices	around	the	world,	and	supports	various	form	factors	including	wearable
 devices	and	televisions.	Devices	can	come	in	different	sizes	and	shapes	that	affect	the	screen	designs	for	UI	elements	in
 your	apps.	
In	addition,	device	manufacturers	may	add	their	own	UI	elements,	styles,	and	colors	to	differentiate	their	products.	Each
 manufacturer	offers	different	features	with	respect	to	keyboard	forms,	screen	size,	or	camera	buttons.	An	app	running	on
 one	device	may	look	a	bit	different	on	another.	The	challenge	for	many	developers	is	to	design	UI	elements	that	can	work
 on	all	devices	It	is	also	the	developer’s	responsibility	to	provide	an	app’s	resources	such	as	icons,	logos,	other	graphics,
 and	text	styles	to	maintain	uniformity	of	appearance	across	different	devices.
 ### Maximizing	app	performance
 An	app's	performance—how	fast	it	runs,	how	easily	it	connects	to	the	network,	and	how	well	it	manages	battery	and
 memory	usage—is	affected	by	factors	such	as	battery	life,	multimedia	content,	and	Internet	access.	You	must	be	aware	of
 these	limitations	and	write	code	in	such	a	way	that	the	resource	utilization	is	balanced	and	distributed	optimally.	For
 example,	you	will	have	to	balance	the	background	services	by	enabling	them	only	when	necessary;	this	will	save	battery
 life	of	the	user’s	device.
 ### Keeping	your	code	and	your	users	secure
 You	need	to	take	precautions	to	secure	your	code	and	the	user’s	experience	when	using	your	app.	Use	tools	such	as
 ProGuard	(provided	in	Android	Studio),	which	detects	and	removes	unused	classes,	fields,	methods,	and	attributes,	and
 encrypt	all	of	your	app's	code	and	resources	while	packaging	the	app.	To	protect	your	user's	critical	information	such	as
 logins	and	passwords,	you	must	secure	the	communication	channel	to	protect	data	in	transit	(across	the	Internet)	as	well	as
 data	at	rest	(on	the	device).
 ### Remaining	compatible	with	older	platform	versions
 Consider	how	to	add	new	Android	platform	version	features	to	an	app,	while	ensuring	that	the	app	can	still	run	on	devices
 with	older	platform	versions.	It	is	impractical	to	focus	only	on	the	most	recent	Android	version,	as	not	all	users	may	have
 upgraded	or	may	be	able	to	upgrade	their	devices

# 3.Building projects using android studio
Ans:
-Project Creation
-Palette
-Component Tree
-Code and Design Section
-Attribute Section

# 4.Exploring project - android studio
Ans: 
-manifest
-java
-resource

# 5.Creating virtual device
 
# 6.Running the app on a physical device

# 7.Types of Layout

# 8.Explain XML attributes

# 9.The onClick attribute

# 10.Design a XML Page for the given Application.