

#FWS webidents


### Summary
The ellipse is the basic element. The basic dynamic here is static / intermittent. So our ellipse shape changes from one state to the other. The ellipse is rendered as a fixed width stroke. It can rotate, shift and scale and change colour. It has a lifetime. (shift meaning an offset in position from the default position). It can animate from one set of attributes to another. Based on random or other input the ellipse will change and/or generate more ellipses.


##Structure



We use grandcentral / controller / event structure and textconsole

* grand central
* set controller
* agent controller
* deus controller
* observe controller


##Objects

ellipse object, that can be told to do things, like animating towards a given value for an attribute. when created, an object with geometry is created in the project tree, and a monobehaviour c# script attached to it.

ellipses can have ellipses as their children. an ellipse contains a reference to its (single) parent, to a master collection (all the way up) and a children collection

ellipses have triggers, like reaching the values it was told to go to, or reaching the end of its lifetime. when that happens it performs an action that was assigned to that trigger

ellipses can subscribe to events from otther ellipses



PSEUDO


class ellipse

attributes
size, position, rotation, rotationspeed, colour, thickness
parentobject, childrencollection, mastercollection

initiate (parent, master)
set parent, master

methods
set rotationspeed
kill


update

rotate
lifetime



