:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualShaderNodeFloatOp.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualShaderNodeFloatOp:

VisualShaderNodeFloatOp
=======================

**Inherits:** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A floating-point scalar operator to be used within the visual shader graph.

Description
-----------

Applies :ref:`operator<class_VisualShaderNodeFloatOp_property_operator>` to two floating-point inputs: ``a`` and ``b``.

Properties
----------

+--------------------------------------------------------+------------------------------------------------------------------+-------+
| :ref:`Operator<enum_VisualShaderNodeFloatOp_Operator>` | :ref:`operator<class_VisualShaderNodeFloatOp_property_operator>` | ``0`` |
+--------------------------------------------------------+------------------------------------------------------------------+-------+

Enumerations
------------

.. _enum_VisualShaderNodeFloatOp_Operator:

.. _class_VisualShaderNodeFloatOp_constant_OP_ADD:

.. _class_VisualShaderNodeFloatOp_constant_OP_SUB:

.. _class_VisualShaderNodeFloatOp_constant_OP_MUL:

.. _class_VisualShaderNodeFloatOp_constant_OP_DIV:

.. _class_VisualShaderNodeFloatOp_constant_OP_MOD:

.. _class_VisualShaderNodeFloatOp_constant_OP_POW:

.. _class_VisualShaderNodeFloatOp_constant_OP_MAX:

.. _class_VisualShaderNodeFloatOp_constant_OP_MIN:

.. _class_VisualShaderNodeFloatOp_constant_OP_ATAN2:

.. _class_VisualShaderNodeFloatOp_constant_OP_STEP:

.. _class_VisualShaderNodeFloatOp_constant_OP_ENUM_SIZE:

enum **Operator**:

- **OP_ADD** = **0** --- Sums two numbers using ``a + b``.

- **OP_SUB** = **1** --- Subtracts two numbers using ``a - b``.

- **OP_MUL** = **2** --- Multiplies two numbers using ``a * b``.

- **OP_DIV** = **3** --- Divides two numbers using ``a / b``.

- **OP_MOD** = **4** --- Calculates the remainder of two numbers. Translates to ``mod(a, b)`` in the Godot Shader Language.

- **OP_POW** = **5** --- Raises the ``a`` to the power of ``b``. Translates to ``pow(a, b)`` in the Godot Shader Language.

- **OP_MAX** = **6** --- Returns the greater of two numbers. Translates to ``max(a, b)`` in the Godot Shader Language.

- **OP_MIN** = **7** --- Returns the lesser of two numbers. Translates to ``min(a, b)`` in the Godot Shader Language.

- **OP_ATAN2** = **8** --- Returns the arc-tangent of the parameters. Translates to ``atan(a, b)`` in the Godot Shader Language.

- **OP_STEP** = **9** --- Generates a step function by comparing ``b``\ (x) to ``a``\ (edge). Returns 0.0 if ``x`` is smaller than ``edge`` and otherwise 1.0. Translates to ``step(a, b)`` in the Godot Shader Language.

- **OP_ENUM_SIZE** = **10** --- Represents the size of the :ref:`Operator<enum_VisualShaderNodeFloatOp_Operator>` enum.

Property Descriptions
---------------------

.. _class_VisualShaderNodeFloatOp_property_operator:

- :ref:`Operator<enum_VisualShaderNodeFloatOp_Operator>` **operator**

+-----------+---------------------+
| *Default* | ``0``               |
+-----------+---------------------+
| *Setter*  | set_operator(value) |
+-----------+---------------------+
| *Getter*  | get_operator()      |
+-----------+---------------------+

An operator to be applied to the inputs. See :ref:`Operator<enum_VisualShaderNodeFloatOp_Operator>` for options.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
