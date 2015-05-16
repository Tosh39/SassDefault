# Sass-Default
To build readable css


# CSS Naming Rule Guidelines

###### Author: Toshiki Yamamoto
###### Date: 2014/11/21

### Purpose
* To make class names short as possible.
* To reduce times for naming and coding, or maintenance when alone and also team.
* To let easy to understand what the class stands for.

### Basic Rules
#####Block is one conponent. Block is consisted by 2 kinds of groups, 'Layout', and 'Module'. Layout means how to display and Module means how to style.


| Kind | Include | Prefix | Rules |
|------|---------|--------|-------|
| Blockname | Anything which can affect all through this block. | None | Indicate specific roll for this block. |
| Layout | Margin, Padding, Box-sizing, Position, Display, Top/Left/Right/Bottom | 'l-' | Start from 'l-blockname' (layout). Going to be longer when deeper |
| Module | Font, Color, Ackground, Line-height, Transform, Transition, and so on. | 'c-' or 'g-' | This is separated by 3 parts, 'how deep', 'blockname', 'specific name'. How deep is 'c-blockname' (child: 1) or 'g-blockname' (grandchild: 2). Deeper than grand-child, its going to be like; 'cg-' (3), 'ggg-' (6).

###Supported Rules
##### Supported Rules are so important to prevent canceling of each classes.

| Kind | Include | Prefix | Rules |
|------|---------|--------|-------|
| State | Anything to add or remove when the state changes. | 'is-' or 'has-' | This make elements change style by added to or removed from the element. This could use '!important' because this has to affect.|
| Utility |Anything | 'u-' | Include only ONE or TWO styles |
| Icon | Only icon related styles | 'ic-' | This is intended to use with '< span >'|

### Detail Rules
#####Independent
CSS selectors should be only by class, and id in some case.DO NOT use html tags so often. Sometimes, for example 'li' elements with no child element, it can be used.

#####Capital Letters, NOT Hyphen(-)
If the name is consisted by 2 parts, such as 'side menu', **DO NOT** use hyphen(-) to make it separate, **USE** Capital letter.
'.sideMenu' is correct.
