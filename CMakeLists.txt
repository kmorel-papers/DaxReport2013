cmake_minimum_required(VERSION 2.8)

project(DaxReport2013 NONE)

include(UseLATEX.cmake)

set(images
  SANDimages/DOEbwlogo.pdf
  SANDimages/snllineblk.pdf
  SANDimages/SANDbackground.png
  images/DaxDiagram.pdf
  images/Containers.pdf
  images/PackageHierarchy.pdf
  images/CellConnections.pdf
  images/WorkletExampleAnnotated.pdf
  images/CellConnectionsHexahedron.pdf
  images/CellConnectionsLine.pdf
  images/CellConnectionsQuadrilateral.pdf
  images/CellConnectionsTetrahedron.pdf
  images/CellConnectionsTriangle.pdf
  images/CellConnectionsVertex.pdf
  images/CellConnectionsVoxel.pdf
  images/CellConnectionsWedge.pdf
  images/GitActivity.png
  images/TransferVsExecution.pdf
  images/TimingThresholdPointMask.pdf
  images/TimingThresholdNoPointMask.pdf
  images/TimingMCManifold.pdf
  images/TimingMCSoup.pdf
  )

set(input_docs
  Summary.tex
  Introduction.tex
  Overview.tex
  Documentation.tex
  ProgressReport.tex
  Distribution.tex
  )

add_latex_document(DaxReport2013.tex
  INPUTS ${input_docs}
  IMAGES ${images}
  BIBFILES DaxReport2013.bib
  USE_INDEX
  )