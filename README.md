# [FHIR Resource List](https://www.hl7.org/fhir/resourcelist.html)

The FHIR Specification is rather large but OrthoFi only requires several of the structures to be able to map data. This repository provides example data and a list of properties that require special consideration to limit your need to refer to the FHIR spec linked in the header above.

JSON example files are found in the FHIR Structures folder and this README calls out some specific properties that require further explanation.


# FHIR Resource Quick Links
[Patient](https://www.hl7.org/fhir/patient.html)

[Related Person](https://www.hl7.org/fhir/relatedperson.html)

[Appointment](https://www.hl7.org/fhir/appointment.html)

[Practitioner](https://www.hl7.org/fhir/practitioner.html)

[Organization](https://www.hl7.org/fhir/organization.html)

[Location](https://www.hl7.org/fhir/location.html)


# Property Call Outs
The following properties may be found in multiple structures and have extra clarification on how they are formatted because conveying their full use in the examples is not possible.

## `telecom[].system`
**Found in**: Patient, Related Person, Practitioner, Location

**Allowed values**: [ phone | fax | email | pager | url | sms | other ]

A `telecom` object is a specific implementation of the [ContactPoint](https://www.hl7.org/fhir/datatypes.html#ContactPoint) resource.

## `name.use` or `name[].use`
**Found in**: Patient, Related Person, Practitioner

**Allowed Values**: [ usual | official | temp | nickname | anonymous | old | maiden ]

A `name` object is a specific implementation of the [HumanName](https://www.hl7.org/fhir/datatypes.html#HumanName) resource.

## `status`
**Found in**: Appointment

**Allowed Values**: [ proposed | pending | booked | arrived | fulfilled | cancelled | noshow | entered-in-error | checked-in | waitlist ]

**Found in**: Location

**Allowed Values**: [ active | suspended | inactive ]

