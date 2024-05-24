auto_link.py
=============

Define the auto link policies between different waveguide type.

For example:

``(type(WG.SusSi.MWIR.WIRE) >> type(WG.SusSi.MWIR.WIRE), StraightPrefer(WG.SusSi.MWIR.WIRE), BendUsing(WG.SusSi.MWIR.WIRE.BEND_EULER))``

It means that when the start and end waveguide are both ``WG.SusSi.MWIR.WIRE``, the automated waveguide type for routing will be ``WG.SusSi.MWIR.WIRE`` and an automated bend ``WG.SusSi.MWIR.WIRE.BEND_EULER`` will be added at a 90 degree turn.


Users are allowed to define and set ``DEFAULT`` to their own specific linking policy.

