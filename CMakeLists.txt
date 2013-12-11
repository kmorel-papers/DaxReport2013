cmake_minimum_required(VERSION 2.8)

project(DaxReport2013 NONE)

include(UseLATEX.cmake)

set(images
  SANDimages/DOEbwlogo.pdf
  SANDimages/snllineblk.pdf
  SANDimages/SANDbackground.png
  images/DaxDiagram.pdf
  images/PackageHierarchy.pdf
  images/CellConnections.pdf
  images/WorkletExampleAnnotated.pdf
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