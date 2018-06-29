.. _spec_v2:

Zarr CDF (ZCDF) storage specification version 0
===============================================

This document provides a technical specification of the protocol and format
used for storing Zarr CDF datasets. The key words "MUST", "MUST NOT", "REQUIRED",
"SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and
"OPTIONAL" in this document are to be interpreted as described in `RFC 2119
<https://www.ietf.org/rfc/rfc2119.txt>`_.

Status
------

This specification is the latest version. It should be referenced against the
underlying `Zarr storage specification version 2
<http://zarr.readthedocs.io/en/latest/spec/v2.html>`_.

Storage
-------

No changes relative to Zarr specification.

Arrays
------

No changes relative to Zarr specification.

Hierarchies
-----------

No changes relative to Zarr specification.

Attributes
----------

Custom attributes MAY be associated with arrays or groups as defined in the
Zarr specification. The ZCDF specification adds to the specification by adding
a REQUIRED attribute specifying the name of the dimensions.

Dimensions
~~~~~~~~~~

Each Array MUST include the attribute key: "_ARRAY_DIMENSIONS". The value of the
"_ARRAY_DIMENSIONS" attribute MUST be a list of strings equal in length to the
number of dimensions in the array.
