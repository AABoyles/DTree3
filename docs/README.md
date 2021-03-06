<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [TidyTree][1]
    -   [Parameters][2]
    -   [setData][3]
        -   [Parameters][4]
    -   [setTree][5]
        -   [Parameters][6]
    -   [draw][7]
        -   [Parameters][8]
    -   [redraw][9]
    -   [recenter][10]
    -   [setLayout][11]
        -   [Parameters][12]
    -   [setMode][13]
        -   [Parameters][14]
    -   [setType][15]
        -   [Parameters][16]
    -   [setRotation][17]
        -   [Parameters][18]
    -   [setHStretch][19]
        -   [Parameters][20]
    -   [setVStretch][21]
        -   [Parameters][22]
    -   [setAnimation][23]
        -   [Parameters][24]
    -   [setBranchNodes][25]
        -   [Parameters][26]
    -   [eachBranchNode][27]
        -   [Parameters][28]
    -   [setBranchLabels][29]
        -   [Parameters][30]
    -   [eachBranchLabel][31]
        -   [Parameters][32]
    -   [setBranchDistances][33]
        -   [Parameters][34]
    -   [eachBranchDistance][35]
        -   [Parameters][36]
    -   [setLeafNodes][37]
        -   [Parameters][38]
    -   [eachLeafNode][39]
        -   [Parameters][40]
    -   [setLeafLabels][41]
        -   [Parameters][42]
    -   [eachLeafLabel][43]
        -   [Parameters][44]
    -   [setRuler][45]
        -   [Parameters][46]
    -   [search][47]
        -   [Parameters][48]
    -   [on][49]
        -   [Parameters][50]
    -   [off][51]
        -   [Parameters][52]
    -   [trigger][53]
        -   [Parameters][54]
    -   [destroy][55]
    -   [validLayouts][56]
    -   [validTypes][57]
    -   [validModes][58]

## TidyTree

This class function creates a TidyTree object.

### Parameters

-   `data`  
-   `options` **[Object][59]** A Javascript object containing options to set up the tree
-   `events`  
-   `newick` **[String][60]** A valid newick string

### setData

Update the TidyTree's underlying data structure
There are two contexts in which you should call this:
	1\. You wish to replace the tree with a completely different tree, given by a different newick string
	2\. Your underlying tree data has changed (e.g. the tree has been re-rooted)

#### Parameters

-   `data` **[Object][59]** A patristic.Branch object

Returns **[Object][59]** the TidyTree object

### setTree

Update the TidyTree's underlying data structure
There are two contexts in which you should call this:
	1\. You wish to replace the tree with a completely different tree, given by a different newick string
	2\. Your underlying tree data has changed (e.g. the tree has been re-rooted)

#### Parameters

-   `newick` **[String][60]** A valid newick string

Returns **[Object][59]** the TidyTree object

### draw

Draws a Phylogenetic on the element referred to by selector

#### Parameters

-   `selector` **[String][60]** A CSS selector

Returns **[TidyTree][61]** the TidyTree object

### redraw

Redraws the links and relocates the nodes accordingly

Returns **[TidyTree][61]** The TidyTree Object

### recenter

Recenters the tree in the center of the view

Returns **[TidyTree][61]** The TidyTree object

### setLayout

Set the TidyTree's layout

#### Parameters

-   `newLayout` **[String][60]** The new layout

Returns **[TidyTree][61]** The TidyTree Object

### setMode

Set the TidyTree's mode

#### Parameters

-   `newMode` **[String][60]** The new mode

Returns **[TidyTree][61]** The TidyTree object

### setType

Set the TidyTree's type

#### Parameters

-   `newType` **[Boolean][62]** The new type

Returns **[TidyTree][61]** the TidyTree object

### setRotation

Set the TidyTree's rotation

#### Parameters

-   `degrees` **[Number][63]** The new number of degrees by which to rotate the tree

Returns **[TidyTree][61]** the TidyTree object

### setHStretch

Set the TidyTree's Horizontal Stretch

#### Parameters

-   `proportion` **[Number][63]** The new proportion by which to stretch the tree

Returns **[TidyTree][61]** the TidyTree object

### setVStretch

Set the TidyTree's Vertical Stretch

#### Parameters

-   `proportion` **[Number][63]** The new proportion by which to stretch the tree

Returns **[TidyTree][61]** the TidyTree object

### setAnimation

Set the TidyTree's animation time. Note that this does not trigger a
redraw.

#### Parameters

-   `time` **[number][63]** The desired duration of an animation, in ms. Set to 0
    to turn animations off completely.

Returns **[TidyTree][61]** The TidyTree object

### setBranchNodes

Shows or hides the Branch Nodes

#### Parameters

-   `show` **[Boolean][62]** Should Branch nodes be shown?

Returns **[TidyTree][61]** the TidyTree object

### eachBranchNode

Restyles Leaf Nodes

#### Parameters

-   `styler` **[Function][64]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][61]** the TidyTree Object

### setBranchLabels

Set the TidyTree's branchLabels

#### Parameters

-   `show` **[Boolean][62]** Should the TidyTree show branchLabels?

Returns **[TidyTree][61]** the TidyTree Object

### eachBranchLabel

Restyles Branch Label

#### Parameters

-   `styler` **[Function][64]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][61]** the TidyTree Object

### setBranchDistances

Shows or hides the TidyTree's branch labels

#### Parameters

-   `show` **[Boolean][62]** Should the TidyTree show branch distances?

Returns **[TidyTree][61]** The TidyTree Object

### eachBranchDistance

Restyles Branch Distances

#### Parameters

-   `styler` **[Function][64]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][61]** the TidyTree Object

### setLeafNodes

Shows or Hides the Leaf Nodes

#### Parameters

-   `show` **[Boolean][62]** Should leaf nodes be visible?

Returns **[TidyTree][61]** The TidyTree Object

### eachLeafNode

Restyles Leaf Nodes

#### Parameters

-   `styler` **[Function][64]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][61]** the TidyTree Object

### setLeafLabels

Shows or Hides the TidyTree's Leaf Labels

#### Parameters

-   `show` **[Boolean][62]** Should the TidyTree show leafLabels?

Returns **[TidyTree][61]** the TidyTree Object

### eachLeafLabel

Restyles Leaf Labels

#### Parameters

-   `styler` **[Function][64]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][61]** the TidyTree Object

### setRuler

Shows or hides the TidyTree's branch labels

#### Parameters

-   `show` **[Boolean][62]** Should the TidyTree show branchLabels?

Returns **[TidyTree][61]** The TidyTree Object

### search

Searches the tree, returns Search Results

#### Parameters

-   `test` **[Function][64]** A function which takes a Branch and returns a Truthy
    or Falsy value.

Returns **[Array][65]** The array of results

### on

Attaches a new event listener
Please note that this is not yet functioning.

#### Parameters

-   `events` **[String][60]** A space-delimited list of event names
-   `callback` **[Function][64]** The function to run when one of the `events` occurs.

Returns **[TidyTree][61]** The TidyTree on which this method was called.

### off

Removes all event listeners from the given events

#### Parameters

-   `events` **[String][60]** A space-delimited list of event names

Returns **[TidyTree][61]** The TidyTree on which this method was called.

### trigger

Forces the tree to respond as though an `event` has occurred

#### Parameters

-   `events` **[String][60]** space-delimited list of names of events to trigger.
-   `args` **Spread** Any arguments which should be passed to the event
    handler(s).

Returns **any** The output of the callback run on `event`

### destroy

Destroys the TidyTree

Returns **[undefined][66]** 

### validLayouts

The available layouts for rendering trees.

Type: [Array][65]

### validTypes

The available types for rendering branches.

Type: [Array][65]

### validModes

The available modes for rendering branches.

Type: [Array][65]

[1]: #tidytree

[2]: #parameters

[3]: #setdata

[4]: #parameters-1

[5]: #settree

[6]: #parameters-2

[7]: #draw

[8]: #parameters-3

[9]: #redraw

[10]: #recenter

[11]: #setlayout

[12]: #parameters-4

[13]: #setmode

[14]: #parameters-5

[15]: #settype

[16]: #parameters-6

[17]: #setrotation

[18]: #parameters-7

[19]: #sethstretch

[20]: #parameters-8

[21]: #setvstretch

[22]: #parameters-9

[23]: #setanimation

[24]: #parameters-10

[25]: #setbranchnodes

[26]: #parameters-11

[27]: #eachbranchnode

[28]: #parameters-12

[29]: #setbranchlabels

[30]: #parameters-13

[31]: #eachbranchlabel

[32]: #parameters-14

[33]: #setbranchdistances

[34]: #parameters-15

[35]: #eachbranchdistance

[36]: #parameters-16

[37]: #setleafnodes

[38]: #parameters-17

[39]: #eachleafnode

[40]: #parameters-18

[41]: #setleaflabels

[42]: #parameters-19

[43]: #eachleaflabel

[44]: #parameters-20

[45]: #setruler

[46]: #parameters-21

[47]: #search

[48]: #parameters-22

[49]: #on

[50]: #parameters-23

[51]: #off

[52]: #parameters-24

[53]: #trigger

[54]: #parameters-25

[55]: #destroy

[56]: #validlayouts

[57]: #validtypes

[58]: #validmodes

[59]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[60]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

[61]: #tidytree

[62]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean

[63]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number

[64]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Statements/function

[65]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array

[66]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/undefined
