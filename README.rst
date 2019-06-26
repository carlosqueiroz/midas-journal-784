ITKTwoProjectionRegistration
============================
https://discourse.itk.org/t/create-drr-image-from-chest-ct-scan/1370
.. image:: https://dev.azure.com/InsightSoftwareConsortium/ITKModules/_apis/build/status/InsightSoftwareConsortium.ITKTwoProjectionRegistration?branchName=master
    :target: https://dev.azure.com/InsightSoftwareConsortium/ITKModules/_build/latest?definitionId=13&branchName=master
    :alt: Build Status


Overview
--------

An `ITK <http://itk.org>`_-based implementation of intensity-based 2D/3D rigid
image registration for patient setup assessment in external beam radiotherapy.
The registration framework was designed to simultaneously register two
projection images to a 3D image volume. The projection geometry was set up to
simulate the X-ray imaging system that attached to a medical linear
accelerator for cancer treatment. The normalized correlation was used as the
similarity measure and the Powell's optimizer was used as the optimization
method. Siddon-Jacobs fast ray-tracing algorithm was implemented to compute
projection images from a 3D image volume.

A more detailed description can be found in the Insight Journal article::

  Wu, J.
  ITK-Based Implementation of Two-Projection 2D/3D Registration Method with an
  Application in Patient Setup for External Beam Radiotherapy
  The Insight Journal. July-December. 2010.
  http://hdl.handle.net/10380/3245
  http://www.insight-journal.org/browse/publication/784


Since ITK 4.10.0, this module is available in the ITK source tree as a Remote
module. To enable it, set::

  Module_TwoProjectionRegistration:BOOL=ON

in ITK's CMake build configuration.


License
-------

This software is distributed under the Apache 2.0 license. Please see
the *LICENSE* file for details.
