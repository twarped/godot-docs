:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the XRPositionalTracker.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_XRPositionalTracker:

XRPositionalTracker
===================

**Inherits:** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A tracked object.

Description
-----------

An instance of this object represents a device that is tracked, such as a controller or anchor point. HMDs aren't represented here as they are handled internally.

As controllers are turned on and the AR/VR interface detects them, instances of this object are automatically added to this list of active tracking objects accessible through the :ref:`XRServer<class_XRServer>`.

The :ref:`XRController3D<class_XRController3D>` and :ref:`XRAnchor3D<class_XRAnchor3D>` both consume objects of this type and should be used in your project. The positional trackers are just under-the-hood objects that make this all work. These are mostly exposed so that GDNative-based interfaces can interact with them.

Tutorials
---------

- :doc:`../tutorials/vr/index`

Properties
----------

+---------------------------+----------------------------------------------------------+---------+
| :ref:`float<class_float>` | :ref:`rumble<class_XRPositionalTracker_property_rumble>` | ``0.0`` |
+---------------------------+----------------------------------------------------------+---------+

Methods
-------

+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                                    | :ref:`get_joy_id<class_XRPositionalTracker_method_get_joy_id>` **(** **)** |const|                                                         |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Mesh<class_Mesh>`                                  | :ref:`get_mesh<class_XRPositionalTracker_method_get_mesh>` **(** **)** |const|                                                             |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Basis<class_Basis>`                                | :ref:`get_orientation<class_XRPositionalTracker_method_get_orientation>` **(** **)** |const|                                               |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>`                            | :ref:`get_position<class_XRPositionalTracker_method_get_position>` **(** **)** |const|                                                     |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`TrackerHand<enum_XRPositionalTracker_TrackerHand>` | :ref:`get_tracker_hand<class_XRPositionalTracker_method_get_tracker_hand>` **(** **)** |const|                                             |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                                    | :ref:`get_tracker_id<class_XRPositionalTracker_method_get_tracker_id>` **(** **)** |const|                                                 |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`StringName<class_StringName>`                      | :ref:`get_tracker_name<class_XRPositionalTracker_method_get_tracker_name>` **(** **)** |const|                                             |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`TrackerType<enum_XRServer_TrackerType>`            | :ref:`get_tracker_type<class_XRPositionalTracker_method_get_tracker_type>` **(** **)** |const|                                             |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Transform3D<class_Transform3D>`                    | :ref:`get_transform<class_XRPositionalTracker_method_get_transform>` **(** :ref:`bool<class_bool>` adjust_by_reference_frame **)** |const| |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                                  | :ref:`is_tracking_orientation<class_XRPositionalTracker_method_is_tracking_orientation>` **(** **)** |const|                               |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                                  | :ref:`is_tracking_position<class_XRPositionalTracker_method_is_tracking_position>` **(** **)** |const|                                     |
+----------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+

Enumerations
------------

.. _enum_XRPositionalTracker_TrackerHand:

.. _class_XRPositionalTracker_constant_TRACKER_HAND_UNKNOWN:

.. _class_XRPositionalTracker_constant_TRACKER_HAND_LEFT:

.. _class_XRPositionalTracker_constant_TRACKER_HAND_RIGHT:

enum **TrackerHand**:

- **TRACKER_HAND_UNKNOWN** = **0** --- The hand this tracker is held in is unknown or not applicable.

- **TRACKER_HAND_LEFT** = **1** --- This tracker is the left hand controller.

- **TRACKER_HAND_RIGHT** = **2** --- This tracker is the right hand controller.

Property Descriptions
---------------------

.. _class_XRPositionalTracker_property_rumble:

- :ref:`float<class_float>` **rumble**

+-----------+-------------------+
| *Default* | ``0.0``           |
+-----------+-------------------+
| *Setter*  | set_rumble(value) |
+-----------+-------------------+
| *Getter*  | get_rumble()      |
+-----------+-------------------+

The degree to which the tracker rumbles. Ranges from ``0.0`` to ``1.0`` with precision ``.01``.

Method Descriptions
-------------------

.. _class_XRPositionalTracker_method_get_joy_id:

- :ref:`int<class_int>` **get_joy_id** **(** **)** |const|

If this is a controller that is being tracked, the controller will also be represented by a joystick entry with this ID.

----

.. _class_XRPositionalTracker_method_get_mesh:

- :ref:`Mesh<class_Mesh>` **get_mesh** **(** **)** |const|

Returns the mesh related to a controller or anchor point if one is available.

----

.. _class_XRPositionalTracker_method_get_orientation:

- :ref:`Basis<class_Basis>` **get_orientation** **(** **)** |const|

Returns the controller's orientation matrix.

----

.. _class_XRPositionalTracker_method_get_position:

- :ref:`Vector3<class_Vector3>` **get_position** **(** **)** |const|

Returns the world-space controller position.

----

.. _class_XRPositionalTracker_method_get_tracker_hand:

- :ref:`TrackerHand<enum_XRPositionalTracker_TrackerHand>` **get_tracker_hand** **(** **)** |const|

Returns the hand holding this tracker, if known. See :ref:`TrackerHand<enum_XRPositionalTracker_TrackerHand>` constants.

----

.. _class_XRPositionalTracker_method_get_tracker_id:

- :ref:`int<class_int>` **get_tracker_id** **(** **)** |const|

Returns the internal tracker ID. This uniquely identifies the tracker per tracker type and matches the ID you need to specify for nodes such as the :ref:`XRController3D<class_XRController3D>` and :ref:`XRAnchor3D<class_XRAnchor3D>` nodes.

----

.. _class_XRPositionalTracker_method_get_tracker_name:

- :ref:`StringName<class_StringName>` **get_tracker_name** **(** **)** |const|

Returns the controller or anchor point's name, if applicable.

----

.. _class_XRPositionalTracker_method_get_tracker_type:

- :ref:`TrackerType<enum_XRServer_TrackerType>` **get_tracker_type** **(** **)** |const|

Returns the tracker's type, which will be one of the values from the :ref:`TrackerType<enum_XRServer_TrackerType>` enum.

----

.. _class_XRPositionalTracker_method_get_transform:

- :ref:`Transform3D<class_Transform3D>` **get_transform** **(** :ref:`bool<class_bool>` adjust_by_reference_frame **)** |const|

Returns the transform combining this device's orientation and position.

----

.. _class_XRPositionalTracker_method_is_tracking_orientation:

- :ref:`bool<class_bool>` **is_tracking_orientation** **(** **)** |const|

Returns ``true`` if this device is tracking orientation.

----

.. _class_XRPositionalTracker_method_is_tracking_position:

- :ref:`bool<class_bool>` **is_tracking_position** **(** **)** |const|

Returns ``true`` if this device is tracking position.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
