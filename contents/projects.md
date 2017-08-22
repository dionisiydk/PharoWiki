# Pharo projects on Github

- Tealight: Tealight is a project defining a few extensions to the Teapot framework to make the (tea) time you spend with the Pharo Teapot system even easier. https://github.com/astares/Tealight

- Iceberg: Iceberg is a set of tools that allow one to handle git repositories directly from a Pharo image. Right now we support only git, but Iceberg is designed to allow other code versioning systems in the future. The final aim of Iceberg is to become the default repository manager for Pharo-core, allowing for smoother and faster integration of contributions, as well as better branch and version management. https://github.com/pharo-vcs/iceberg

- SmaCC: Smalltalk Compiler Compiler : a parser generator. https://github.com/ThierryGoubier/SmaCC

# Pharo 6 projects in Package Catalog
These projects are downloadable from inside Pharo 6 using the ``` World Menu -> Tools -> Catalog Browser ```

## Animation
Adds a delay operator turning any message send into a smooth transition.

keywords: animation fun time

## Artefact
Artefact is a library to generate PDF documents. It provides a
document model and support the generation of PDF

keywords: PDF document layout

## AstaresDistribution
Several Pharo goodies like Pomodoro, DesktopManager, QuickAccess,
HubCap, ScriptManager, ... written by Torsten Bergmann (astares.com)
bundled for easy installation

keywords: custom distribution goodies pharo

## Atlas
A Python bridge (IPC - stream sockets) for Pharo, allowing Pharo to
use Python libraries , mix with Python code and vice versa

keywords: Atlas IPC atlas pharo python sockets

## BitmapCharacterSet
BitmapCharacterSet is a set for characters that uses a bitmap for
storing wide characters and an array of truth values for byte
characters. Used by XMLParser.

keywords: character collection set unicode

## Bootstrap
"Bootstrap for Seaside" is a project combining Seaside and Twitter
Bootstrap and easily use them to write professional looking web
applications.

keywords: Bootstrap HTML Seaside query web

## Bugzilla
Pharo wrapper for Bugzilla REST API

keywords: api bugzilla rest

## CPPBridge
CPP is a library that allows Pharo to share memory with a C++
application. This means that both can share the exact same data and
modify it. This also can allow Pharo and C++ to exacute one another
library and code. Example provided

keywords: ++ ++ C IPC bridge c cpp file mapped memory shared

## Calypso
Calypso is a new system browser based on new navigation model

keywords: IDE systemBrowser

## CheatSheet

Pharo Cheat Sheet.

Project main page: *http://www.smalltalkhub.com/#!/~PharoExtras/CheatSheet*

keywords: examples syntax

## ChronosManager
ChronosManager is a time managment tool based on the pomodoro
technique offering a stopwatch and timer for keeping track of time
with tasks and goals

keywords: ChronosManager managment pomodoro time

## Citezen
Citezen is a library to parse, query and manage bibtex scientific citations.

keywords: bibtex latex parser printer query

## CommandShell
nil

keywords:

## Commander
Commander models application actions as first class objects.

Every action is implemented as separate command class (subclass of
CmdCommand) with #execute method and all state required for execution.

Commands are reusable objects and applications provide various ways to
access them. Such information is attached to command classes as
activator objects. Currently there are three types of activators:
- CmdShortcutCommandActivator
- CmdContextMenuCommandActivator
- CmdDragAndDropCommandActivator

Activators are declared in command class side methods marked with
pragma #commandActivator. For example following method will allow
RenamePackageCommand to be executed by shortcut in possible system
```smalltalk
browser:
        RenamePackageCommand class>>packageBrowserShortcutActivator
                <commandActivator>
                ^CmdShortcutCommandActivator by: $r meta for: PackageBrowserContext
And for context menu:
        RenamePackageCommand class>>packageBrowserMenuActivator
                <commandActivator>
                ^CmdContextMenuCommandActivator byRootGroupItemFor: PackageBrowserContext
```
Activators are always declared with application context where they can
be applied (PackageBrowserContext in example). Application should
provide such contexts as subclasses of CmdToolContext with information
about application state. Every widget can bring own context to
interact with application as separate tool. For example system browser
shows multiple panes which provide package context, class context and
method context. And depending on context browser shows different menu
and provides different shortcuts

keywords: command command pattern tools

## Community
Community is a project to add some world menues to easily access some
community pages

keywords: community pharo

## Complex
Math-Complex brings back to Pharo the complex numbers like (1+2i)
which used to be in Squeak Kernel.

keywords: complex math number

## DacapoEnergyConsumption
This project run the Dacapo benchmarks, and monitor the energy
consumption of the CPU. It is for research purposes.

keywords: consumption energy java

## DarkMetalTheme
An alternative to DarkTheme, DarkMetalTheme offers "metalic" tonalities :)

keywords: theme ui

## DebuggerCritiques
Add inlined critiques into Pharo debugger

keywords: critiques debugger smallLint

## DesktopManager
A goodie to be able to manage multiple desktops in Pharo.

keywords: desktop goodie pharo tools

## DiscordSt
DiscordSt is a library for Discord service, see https://discordapp.com
for basic information about Discord and
https://discordapp.com/developers/docs/intro for developer
information.

        The stable version supports Discord Webhooks. See
https://github.com/JurajKubelka/DiscordSt for examples.

keywords: api chat client discord rest web webhook

## EventRecorder
Record and replay screen events.

keywords: recording screen

## FamixDiff
nil

keywords:

## FlatQA
Hi, I'm your personal quality assistant. I run Smalllint rules on the
code that you modify, and notify you about quality changes.
https://github.com/Uko/QualityAssistant#qualityassistant

keywords: automatic critics quality smallint validation

## FogBugz
Access to FogBugz from within Pharo environment.

keywords: fun web

## Garage
Garage is the relational database driver for Pharo. Garage provides a
common API to connect with several database servers in a coherent way
(JDBC like). Along with Garage, we provide implementations of several
database drivers.

keywords: api database drivers

## GarageGlorp
This configuration loads the Garage database drivers along with the
Glorp Object-Relational Mapper. It is a convenience configuration used
to load both projects using a single config.

keywords: database driver orm persistence

## Gettext
Gettext is an implementaion of https://www.gnu.org/software/gettext,
the standard l17n package.

keywords: gettext i18n internationalization l10n localization

## Ghost
nil

keywords:

## GitFileTree
GitFileTree is an integration of Git commands below Monticello,
allowing a very simple and powerfull integration with a git repository
for tracking Monticello packages, allowing for example one to work
from github.com (including with configurations support) without any
use of the command line and with perfect support of whatever is the
structure of the project under git.

Works with any possible organisation of the git repository related to
the package (single language, multi language, single package, multiple
packages, single remote repo, multiple remote repositories, branches,
you name it).

GitFileTree: is integrated into FileTree, but not easily available.
This configuration allow for a one step loading with the dependencies.

keywords: FileTree Monticello OSProcess OSSubprocess Packages Pharo5 Pharo6 git

## GitHubAPI
A GitHub API Wrapper for Pharo to easily access informations from
GitHub right from your Pharo image.

keywords: api git github

## GitHubcello
Have it happened to you that you have your project on GitHub and it
has a baseline but now you have to write down the Metacello script to
load it? Not any more! Simply paste your repo URI into GTSpotter, wait
a bit, select the baseline you want to load, and you're done!
https://github.com/Uko/GitHubcello#githubcello-

keywords: github metacello spotter

## GlorpSQLite
GlorpSQLite is the integration of Glorp with SQLite. This
configuration loads UDBC, which contains SQLite, then loads Glorp.
Once GlorpSQLite is loaded, provided Pharo can find the SQLite
so/dylib/dll file on your system, start Test Runner and run the tests.

keywords: database orm persistence relational

## Grafoscopio
Grafoscopio is a tool to create interactive notebooks and
documentation for computer narratives and data visualization.
        They are structured as outlines/trees containing textual and code
nodes that can be exported to several formats: LaTeX, HTML
        and pdf (via pandoc).
        It can be used in several endeavors like: reproductible open research
and science, data journalism, data activism among others

keywords: data-activism data-journalism data-science
data-visualization documentation interactive-notebook markdown markup
open-data open-research open-science reproducible-research
[Home page](http://mutabit.com/grafoscopio/index.en.html#intro)

## Grease
The Grease Portability Library

keywords: framework portability

## Grid
This package provides a grid (2D array) implementation.

keywords: 2D-array collection container matrix

## Hashids
Hashids allow you to create URL friendly ids from sequential integer
ids.  NB it is should not be considered as encryption but it does
provide a lightweight obfuscation of the underlying id.
https://github.com/alacap/hashids-pharo

keywords: hashing

## Hubcap
nil

keywords:

## INIFile
A Parser for .INI files (as usually used on Windows)

keywords: configurations ini settings windows

## Iceberg
Iceberg is a set of tools that allow one to handle git repositories
directly from a Pharo image.

keywords: git vcs version control

## LightPhaser
nil

keywords:

## MacroRecorder
MacroRecorder is a tool that allows the developer to
        (i) record a sequence of transformations while they are applied a
first time, either manually or with the assistance of refactoring
tools;
        (ii) store and parameterize the transformations to allow their
generalization; and
        (iii) apply automatically the sequence of transformations afterwards
on different code locations.

        For the last step, the developer could explicitly point to the
entities to transform.

keywords: code change code manipulation programming by demonstration
source code transformations

## MatchTool
MatchTool is a simple UI for experimenting with the matching
functionality of pattern code.
MatchTool can be open from the World Menu > Tools category. More
information can be read from within the tool by pressing help button.

keywords: code inspect match pattern rewrite rules

## MessageFlowBrowser
A message flow browse to browser senders, implementors and messages of
methods in a single window and folow the message flow

keywords: browser messageflow methods tools

## Mocketry
Mocketry is mock objects framework. It provides simplest way to stub
any message to any object and to verify any occurred behaviour.
```smalltalk
        mock := Mock new.
        mock stub someMessage willReturn: 1000.

        mock someMessage should be: 1000.
        mock should receive someMessage.

        rect := 0@0 corner: 2@3.
        rect stub width willReturn: 1000.

        rect area should be: 3000 "area = width * height".
        rect should receive width.

keywords: BDD SUnit TDD framework mocks
```
## MooseProject
MooseProject is a library to store many differents versions for a
project. It will persist everything on the disk and allow you easily
to recover the model associated to the desired version

keywords: Moose project version

## Mustache
nil

keywords:

## NPMJS
Spotter search of NPM packages

keywords: javascript nodejs

## Neo4reSt
Neo4reSt is a rest client of Neo4j graph database. (http://neo4j.org/)

Neo4reSt will provide:

- Raw rest client
- Wrapper client which handles JSON well
- Object level wrapper classes (Node, Relationship, Property)


keywords: Neo4j database graph persistence

## NeoCSV
CSV (Comma Separated Values) is a popular data-interchange format.
NeoCSV is an elegant and efficient standalone framework to read and
write CSV converting to or from Smalltalk objects.

keywords: ascii comma-separated-values csv fields format input output
records rfc-4180 tab-separated-values tabular-data text tsv

## NeoJSON
JSON (JavaScript Object Notation) is a popular data-interchange
format. NeoJSON is an elegant and efficient standalone Smalltalk
framework to read and write JSON converting to or from Smalltalk
objects.

keywords: encoding format input javascript json output serialization text

## Nginx
Utility project to work with nginx from Pharo image (Windows only so far)

keywords: nginx server web windows

## OSLinuxCentOS
A part of the OS-XXX series to easier work with native operating
system platforms. Here for using CentOS Linux environments in Pharo.

keywords: centos linux native os unix

## OSLinuxUbuntu
A part of the OS-XXX series to easier work with native operating
system platforms. Here for using Ubuntu Linux environments in Pharo.

keywords: linux native os ubuntu unix

## OSOSX
nil

keywords:

## OSProcess
nil

keywords:

## OSRaspbian
A part of the OS-XXX series to easier work with native operating
system platforms. Here for using Raspbian environments in Pharo.

keywords: linux native os raspbian unix

## OSUnix
A part of the OS-XXX series to easier work with native operating
system platforms. Here for using Unix environments in Pharo.

keywords: native os unix

## OSWindows
API wrappers and tools for the Windows operating system

keywords: api native win32 windows

## ObjectStatistics
ObjectStatistics is tool to analyse set of objects by computing
different kind of metrics and look at them from different angles.
Imaging that we have collection of message sends and we want to know
number of message sends in dimension of receiver, receiver class and
message selector. We have different angles to look at this data: from
receiver class to selector and receiver or from selector to receiver
class and receiver or any other combination.
We also could analyze different kind of metrics which could be
computed on given objects. It could be number of unique receivers,
execution time, executed lines of code, etc.
This package implements computation of object statistics over declared
metrics and dimensions space.
Described example could be look like:
```smalltalk
        stat := ObjectStatistics.
        stat
                countAllAs: 'sends';
                countDifferent: [ :message | message receiver ] as: 'instances'.
        stat
                dimension: [ :message | message receiver class ] named: 'classes';
                with: [
                        stat dimension: [ :message | message selector ] named: 'msgs';
                        with: [
                                stat
                                        dimension: [ :r | r ] named: 'receivers';
                                        ignoreMetrics: #('instances')]];
                dimension: [ :message | message selector ] named: 'msgs';
                with: [
                        stat dimension: [ :message | message receiver class ] named: 'classes';
                        with: [
                                stat
                                        dimension: [ :r | r ] named: 'receivers']].

        stat accumulateAll: messageSends.

```

keywords: analysis framework

## ObjectTravel
ObjectTravel implements traversal of full object graph. It enumerates
each reference in breadth-first direction and visit every reference
only once.
```smalltalk
        traveler := ObjectTraveler on: 10@30.
        traveler moveToNextReference. "true".
        traveler currentReference. "10"
        traveler nextReference. "30"

        traveler := ObjectTraveler on: #(10 20 30).
        traveler nextReference "10"
        traveler nextReference "20"

Also ObjectTravel can replace references with new values:

        traveler replaceCurrentReferenceWith:  #newReference.
```

keywords: objectsTraversal stream tool

## Octopus
A pharo tool that utilises Pillar library to process pillar text
copied to the clipboard and convert it to HTML

keywords: HTML markdown pillar

## OrderPreservingDictionary
This package has two ordered dictionary classes that behave like
OrderedDictionary and OrderedIdentityDictionary in Pharo but are
portable to Squeak and Gemstone, and other ordered dictionary classes
needed by XMLParser.

keywords: collection dictionary order-preserving ordered

## Orion
Orion is an interactive prototyping tool for reengineering, to
simulate changes and compare their impact on multiple versions of
software source code models.

keywords: Moose delta model versioning

## Pastell
Pastell is an add-on for XMLParser which adds some methods that make
navigation of an XML DOM tree much easier, it is a XMLPath-like
library.

keywords: xml xpath

## PharoSprint
The Pharo community regularly organize Pharo Sprint events. The Pharo
Sprint is a regular (monthly) event when developers and users meet
together to fix bugs. This usually takes place in a physical location,
but people are welcomed to participate from any place. This is a great
opportunity for novices to get involved and learn from experts!

For more information: http://bit.ly/SprintWeb and
http://pharo.org/contribute-events

keywords: Bug Discord FogBugz PharoSprint Sprint SprintDay

## Pillar
Pillar is a wiki-like syntax, its document model, a parser for it, and
a set of exporters (e.g., HTML, LaTeX, Markdown...). Pillar is
primarily used as the wiki syntax behind the *Pier
CMS>http://piercms.com*. Pillar is also being used to write books:
e.g., *the Enterprise Pharo book>http://books.pharo.org/*.

keywords: book document html latex markdown pier wiki

## PlotMorph
PlotMorph is a nice plotting system. It can plot multiple series with
different graphical attributes.

keywords: Morph UI graph plotting point series

## PolyMath
Tools for scientific computation in Smalltalk

keywords: ODE mathematics science

## Pomodoro
A pomodoro timer

keywords: GTD morphic pomodoro

## PunQLite
UnQLite binding for Pharo Smalltalk. UnQLite is a fast, lightweight,
portable, embedded KVS with a simple scripting engine (Jx9). By using
PunQLite, you can store/load lots of data as if just using a normal
Dictionary.

PunQLite uses UnQLite shared library. If you have no time to compile,
just get pre-built binary from the github project page
(https://github.com/mumez/PunQLite).



keywords: KVS NoSQL UFFI UnQLite database persistence

## QualityAssistant
Hi, I'm your personal quality assistant. I run Smalllint rules on the
code that you modify, and notify you about quality changes.
https://github.com/Uko/QualityAssistant#qualityassistant

keywords: automatic critics quality smallint validation

## QuickAccess
A manager for scripts with Quick access.

keywords: fun web

## RProjectConnector
nil

keywords:

## RediStick
RediStick is a redis client which supports auto-reconnecting.

Other features:
- Minimum dependencies (runs on Pharo without other libraries)
- Supports unicode strings


keywords: KVS NoSQL Redis database persistence

## ReferenceFinder
Finds reference paths between objects to help find memory leaks.

keywords: memory objects references tracing

## RegexTools
A tool to test and verify regular expressions

keywords: regex utilities

## Roassal2
Roassal is an agile visualization engine. Roassal graphically renders
objects using short and expressive Smalltalk expressions. A large set
of interaction facilities are provided for a better user experience.
Painting, brushing, interconnecting, zooming, drag and dropping will
just make you more intimate with any arbitrary object model.

keywords: charting data visualization

## SRT2VTT
This package convert SRT to VTT (subtitles for videos plugins)

keywords: browser plugin srt videos vtt web

## ScriptManager
A simple tool to manage scripts. Still based on Morphic. We would
recommend users to switch to QuickAccess which is a better script
manager than this tool.

keywords: fun script

## Seaside3
The framework for developing sophisticated web applications in
Smalltalk. See http://www.seaside.st

keywords: framework seaside web

## SimilarityFlooding
This project is an implementation of a FAMIX model difference
algorithm based on Similarity Flooding algorithm as defined by Sergey
Melnik, Hector Garcia-Molina, and Erhard Rahm in 'Similarity flooding:
A versatile graph matching algorithm and its application to schema
matching' and in the technical report associated.
Check the github repository for documentation
[https://github.com/juliendelplanque/SFDiff].

keywords: FAMIX SFDiff difference model similarity similarity flooding

## Spy2
Spy2 is a profiling framework. You can easily create profilers. You
can have a look at a description
http://bergel.eu/download/papers/Berg10f-Spy.pdf

The Hapao test coverage tool is included.

keywords: Hapao Memory Performance Profiling Roassal Spy

## Stamp
Stamp is an implementation of STOMP 1.2, a protocol to access message
oriented middleware like RabbitMQ.

keywords: client format messaging middleware queueing rabbitmq stomp

## StateSpecs
StateSpecs is object state specification framework. It describes
particular object states by first class specifications. For example
there are SpecOfCollectionItem, SpecOfObjectClass and
SpecOfObjectSuperclass. They can match and validate given objects. In
case when object is not satisfied specification you will get failure
result with detailed information about problem.
```smalltalk
        spec matches: anObject.
        spec validate: anObject. "it returns validation result which can be
success or particular failure"
```
To easily create specifications and validate objects by them
StateSpecs provides two kind DSL: should expressions and "word"
classes.
First allows you to write "assertions":
```smalltalk
        1 should be: 2
        1 should equal: 10
```
And second allows you to instantiate specs by natural readable words:
```smalltalk
        Kind of: Number
        Instance of: String
        Equal to: 'test'
```
keywords: BDD SUnit TDD framework validation

## Ston
Smalltalk Object Notation (STON) is a lightweight, text-based,
human-readable data interchange format for class-based object-oriented
languages like Smalltalk. It can be used to serialize domain level
objects, either for persistency or network transport. As its name
suggests, it is based on JSON (Javascript Object Notation). It adds
symbols as a primitive value, class tags for object values and
references.

keywords: encoding format input json output serialization ston text

## SublimishTheme

A dark theme for Pharo. If you like Sublime then you'll like Sublimish theme.
Project main page: *https://github.com/sebastianconcept/SublimishTheme*

keywords: GUI IDE

## Tarantalk
Tarantalk is a Tarantool (Lua with DBMS) connector.

You can:
- Store/load tuples.
- Find tuples by multiple indices
- Evaluate Lua programs


keywords: KVS Lua NoSQL Tarantool Tuple database persistence

## Tarantube
Tarantool message queue wrapper based on Tarantalk.

- Supporting FIFO queue with priority, TTL, TTR, delay and sub queues.
- Need to install Tarantool + Tarantool queue module
(https://github.com/tarantool/queue)



keywords: Lua MQ NoSQL Tarantalk Tarantool queue

## Tealight
Tealight is a project defining a few extensions to the Teapot
framework to make the (tea) time you spend with the Pharo Teapot
system even easier..

keywords: api git github

## Teapot
Teapot is micro web framework on top of the Zinc HTTP components, that
focuses on simplicity and ease of use.

keywords: framework http micro sinatra web

## TestsUsageAnalyser
nil

keywords:

## Trie
This package provides a trie implementation (as developed by Benoit
St-Jean. See https://en.wikipedia.org/wiki/Trie

keywords: collection containers retrieval trie

## Units
Units is a simple and powerful library to manage different units.

keywords: Comparison Meter Points Units

## VMProfiler
VMProfiler is a sampling profiler tracking down where the time is
spent in the VM when executing a specific portion of code. It computes
where the time is spent in the compiled C code of the VM, in the VM
plugins and in the native functions.
The results are available as a statistical report.

keywords: cog jit profiling virtual machine

## VerStix
A Vert.x TCP EventBus client for Pharo Smalltalk.

You can:
- interact with various Vert.x components (Web, Auth, DB, MQ, etc).
- interact with other Smalltalk images
- interact with various languages which support Vert.x EventBus


keywords: microservices network vertx

## VistaCursors
Provide a better looking cursor (similar to Windows Vista).

keywords: cursor theming ui windows

## VoyageMongo
Voyage-Mongo is an object persistence layer made for easy the work
with *MongoDB>http://www.mongodb.org*. It is an "ODM" (Object-Document
Mapper), in the same spirit of the ORMs for relational approaches.

keywords: database mongodb nosql persistence

## VoyageUnqlite
Voyage-UnQLite is an object persistence layer made for easy the work
with *UnQLite>https://unqlite.org*. It is an "ODM" (Object-Document
Mapper), in the same spirit of the ORMs for relational approaches.

keywords: database nosql persistence unqlite

## WKHTML2PDF
Render HTML into PDF and various image formats using the (external) Qt
WebKit rendering engine directly from Pharo.

keywords: html pdf reporting

## WebBrowser
General and platform independent WebBrowser access for Pharo 4.0
onwards based on NativeBoost, for Pharo 5.0 onwards based on UFFI

keywords: internet platform url utility web webbrowser

## XMI
A XMI wrapper for Pharo to easily access XML Metadata informations.

keywords: omg uml xmi xml

## XMLParser
XMLParser provides validating SAX and DOM parsers for well-formed XML
documents on Pharo, Squeak, and Gemstone. It also provides a DOM API
for manipulating documents, namespace support, and an optional
XMLWriter for writing documents. Validation and namespace checking are
enabled by default, but not resolution of external entities.

Implements:
        http://www.w3.org/TR/REC-xml/
        http://www.w3.org/TR/REC-xml-names/
        http://www.w3.org/TR/xml-id/
        http://www.w3.org/TR/xmlbase/
        https://www.w3.org/TR/xml-c14n


keywords: DOM DTD HTML SAX XHTML XML document markup parser validation web

## XMLParserHTML
XMLParserHTML provides SAX and DOM parsers for HTML that convert
possibly malformed HTML into well-formed XML.

keywords: DOM HTML SAX document markup parser web

## XMLParserStAX
XMLParserStAX is a pull parser for XMLParser that provides a streaming
interface for "pulling" XML events and also supports pull-style DOM
parsing for dynamically converting events into DOM nodes.

keywords: DOM DTD HTML StAX XHTML XML XMLPullParser document markup
parser pull pull-parser validation web

## XMLWriter
XMLWriter allows you to generate well-formed XML documents using an
API based on Seaside's canvas and tag brushes so all tags will be
nested properly and not left unclosed.

keywords: HTML XHTML XML document markup web writer

## XPath
An XPath library for Pharo, Squeak, and Gemstone leveraging the XML
parsing capabilities of XMLParser. Supports XPath 1.0 syntax with
extensions.

keywords: DOM HTML XHTML XML XPath document markup parser query web

## ZTimestamp
The ZTimestamp project groups a number of classes that form an
addition/alternative to DateAndTime/Timestamp. The core ZTimestamp
class represents a point in time, with second precision and always in
the UTC/GTM/Zulu timezone. It is faster and smaller. ZTimestampFormat
is a formatter and parser that is example based. ZTimezone uses the
standard Olsone timezone database to compute the offset for local time
at specific points in time for a specified timezone.
ZTimestampSNTPClient is an SNTP client to check the local clock
against network time servers. This project is small and has no further
dependencies. It runs in Pharo 2 and 3.

keywords: chronology date formatting parsing sntp time timestamp timezone

## ZincHTTPComponents
Zinc HTTP Components is an open source Smalltalk framework to deal
with HTTP. It models most concepts of HTTP and its related standards
and offers both client and server functionality. One of its key goals
is to offer understandability (Smalltalk’s design principle number
one). Anyone with a basic understanding of Smalltalk and the HTTP
principles should be able to understand what is going on and learn, by
looking at the implementation.

keywords: character-encoding client http internet mime-type networking
request response server url
