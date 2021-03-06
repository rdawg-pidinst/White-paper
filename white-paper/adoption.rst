Current, planned and potential adoption
=======================================

Helmholtz-Zentrum Berlin für Materialien und Energie (HZB)
----------------------------------------------------------

HZB minted four DOIs with DataCite for HZB instruments: two beamlines
at the neutron source BER II;\ [#hzb_e2]_\ :sup:`,`\ [#hzb_e9]_ one
beamline at the synchrotron light source BESSY II;\ [#hzb_nc_bl]_ and
one experimental station at BESSY II.\ [#hzb_nc_st]_ The DOIs resolve
to the respective instrument page from the HZB instrument database
that did already exist before and was thus not created for this
purpose.  One particularity with these instruments is that they are
custom built by HZB.  Thus, in the metadata HZB appears as Creator as
well as Contributor with property contributorType value
HostingInstitution.  It is noteworthy that one of the DOIs uses the
additional property fundingReference from the DataCite schema to
acknowledge external funding that HZB received for upgrading the
instrument.  This property was not considered in the PIDINST schema,
or in the DataCite mapping.  HZB plans to continue the adoption and to
mint DOIs for all its beamlines and experimental stations that are in
user operation in the near future.

British Oceanographic Data Centre (BODC)
----------------------------------------

The British Oceanographic Data Centre (BODC) is a national facility for
preserving and distributing oceanographic and marine data. BODC tested
the ePIC implementation in web-published, sensor technical metadata
descriptions encoded in the Open Geospatial Consortium’s (OGC)
`SensorML`_ open standards for conceptualising and integrating
real-world sensors. In an initial test case, a PID was minted for a
Sea-Bird Scientific SBE37 Microcat regularly deployed on fixed-point
moorings in the `Porcupine Abyssal Plain Sustained Observatory (PAP-SO)
<PAP-SO_>`_ in the north Atlantic. For further details see
:ref:`landing-page-encoding-swe`. BODC plan to continue adoption
identifying sensors on large research vessels owned by the Natural
Environment Research Council (NERC) and managed by the National
Oceanography Centre (NOC) and British Antarctic Survey (BAS). PIDs will
be used to manage sensor data and metadata workflows from ‘deck to
desktop’ as part of a UK initiative, I/Ocean.

EISCAT3D
--------

`EISCAT3D`_ will be an international research infrastructure, using
radar observations and the incoherent scatter technique for studies of
the atmosphere and near-Earth space environment above the
Fenno-Scandinavian Arctic as well as for the support of the solar system
and radio astronomy sciences. EISCAT3D will implement persistent
identification for instruments following the recommendations by PIDINST.
The radar is complex, more digital than previous radars, and is roughly
divided into a number of separate units. While software is a substantial
constituent of these units, they can be regarded as hardware units, each
persistently identified. Updates to the units will be primarily to
software and result in new unit versions with own PIDs. The radar itself
can also be persistently identified and the relation type HasComponent
can be used to relate to the persistently identified units.

SENSOR.awi.de and PANGAEA
-------------------------

The Alfred Wegener Institute Helmholtz Centre for Polar and Marine
Research (AWI) has been continuously committed to develop and sustain an
eResearch infrastructure for coherent discovery, view, dissemination,
and archival of scientific data and related information in polar and
marine regions. In order to address the increasing heterogeneity of
research platforms and respective devices and sensors along with varying
project-driven requirements, a generic and modular framework has been
built intended to support the flow of sensor observations to archives
(O2A).\ [#koppe2015]_ In this context, SENSOR.awi.de, available since
2015, is an O2A component dedicated to the registry of research
platforms, devices and sensors and in the meantime in use by several
international partners (e.g. MOSAiC project). SENSOR.awi.de has been
built using OGC SensorML standard and all individual records, to date
over 4000, are assigned a persistent identifier using UUIDs in the
handle syntax along with automated generation of a record
citation. Terminologies (e.g., controlled vocabularies) are used to
define sensor categories (NERC L05) as well as sensor types and models
(NERC L22). The data model of SENSOR.awi.de is compliant with the
PIDINST schema and the additional implementation of Datacite DOIS for
sensors is to date under evaluation.  The ultimate goal of SENSOR.awi.de
is to enhance the quality of published and archived data in PANGAEA by
providing complete metadata and persistent identifiers on instruments
and sensors used in the data acquisition process
(:numref:`fig-link-pangea`). Given that platforms and sensors evolve
in time (sensors are being calibrated, instrument payload changes,
etc), SENSOR.awi.de also supports record versioning by maintaining an
audit trail of changes in the XML record.

PANGAEA is a digital repository for environmental research data and the
dedicated long term archive within the O2A framework jointly operated by
the AWI and MARUM (University Bremen). Each dataset is made available
with its descriptive metadata, including the relations with research
resources (e.g., articles, funder, instrument and specimen, if
applicable). As a data provider, PANGAEA only curates limited
information of a device such as device name, identifier and type. As an
effort to standardize device type and name, currently the repository
applies external terminologies, in particular the NERC L05 device
category vocabulary and the L22 device catalogue. The repository has
developed tailor-made client applications to import these terminologies
in a periodic, incremental manner. For both the persistent
identification as well as for the detailed description of instruments,
PANGAEA thus relies on institutional instrument registries such as
SENSOR.awi.de and uses their issued PIDs to uniquely identify
instruments which have been used to acquire data archived at PANGAEA.
Since AWI and PANGAEA use the same vocabularies/terminologies as well as
PIDs to represent devices, they facilitate easy integration of datasets
in particular during transfer of near real time data from O2A raw data
staging areas via data quality control services etc to their final
destination, the PANGAEA data archive.\ [#koppe2015]_

ICOS
----

The Integrated Carbon Observation System (ICOS) is a pan-european
research infrastructure for quantifying and understanding the greenhouse
gas balance of the European continent. It conducts many continuous
in-situ measurements like gas concentrations, wind speed and direction,
humidity, temperature, etc. To deliver high quality measurement data,
ICOS considers the adoption of a persistent identifier for instruments a
must for documenting data provenance and tracking calibration history.


.. _SensorML:
   https://www.opengeospatial.org/standards/sensorml

.. _PAP-SO:
   https://projects.noc.ac.uk/pap/

.. _EISCAT3D:
   https://eiscat.se/business/eiscat3d7/

.. [#hzb_e2]
   https://doi.org/10.5442/NI000001

.. [#hzb_e9]
   https://doi.org/10.5442/NI000002

.. [#hzb_nc_bl]
   https://doi.org/10.5442/NI000003

.. [#hzb_nc_st]
   https://doi.org/10.5442/NI000004

.. [#koppe2015]
   Koppe, R., Gerchow, P., Macario, A., Haas, A., Schäfer-Neth, C.
   and Pfeiffenberger, H. (2015): O2A: A Generic Framework for Enabling
   the Flow of Sensor Observations to Archives and Publications, OCEANS
   2015 Genova. doi: 10.1109/OCEANS-Genova.2015.7271657
